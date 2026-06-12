# Rendering a real MP4 (advanced / technical users only)

Most people should just screen-record (see `screen-record.md`) - it's instant and needs nothing installed. Only go here if the user is comfortable in a terminal and wants a clean MP4 file without screen-recording.

## What's happening

The templates are HTML pages that animate on a `<canvas>` using `requestAnimationFrame`. To turn one into a video file, you load it in a headless (invisible) browser and capture one frame at a time, then stitch the frames into an MP4 with ffmpeg.

## Option A - quick capture with a headless browser (no project setup)

Requires Node + a Chromium. Capture frames by advancing the animation clock and screenshotting, then encode with ffmpeg.

1. Install once: `npm i -g puppeteer` (downloads a Chromium).
2. Use a small script that, for each frame `n`, sets the page's animation start time so it renders the moment `n/60` seconds in, screenshots a 1080x1920 viewport, and saves `frame-0001.png …`.
3. Encode: `ffmpeg -framerate 60 -i frame-%04d.png -c:v libx264 -pix_fmt yuv420p -crf 18 out.mp4`

This is fiddly because each template uses `performance.now()` for timing - you have to override it so a given frame is deterministic. Screen-recording avoids all of this.

## Option B - rebuild it in Remotion (best for a real product)

If this is going to become a paid tool that outputs MP4s reliably, the right move is to port the animation logic into **Remotion** (React + `@remotion/renderer`), where every frame is a pure function of the frame number. Then `renderMedia()` produces a perfect MP4 at any size/fps, no screen-recording. This is how you'd scale the product into a premium, auto-export tier.

## Bottom line

- **Casual user → screen-record.** Always.
- **Building the paid product → Remotion render pipeline** so output is automatic and consistent.
