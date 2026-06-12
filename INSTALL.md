# Installing Magic Graphics (2 minutes)

Magic Graphics is a **skill** for Claude. To use it you need **Claude Code**, or a version of
Claude that supports Skills. If you can chat with Claude in a terminal or app and it can read
files on your computer, you're good.

---

## Fastest way - paste one line, download nothing

Open Claude and paste this:

> **Install the Magic Graphics skill for me: download it from https://github.com/EnergySteve/magic-graphics and put it in my Claude skills folder so that the file `~/.claude/skills/magic-graphics/SKILL.md` exists. Then make me a quick sample clip so I know it's working.**

That's it. Claude downloads everything from GitHub, installs it, and makes you a clip to prove
it works. Start a new chat afterward and say "make me some b-roll for my video."

Prefer to do it yourself? Manual steps below.

---

## Do it by hand

1. Find your Claude skills folder. On Mac or Linux it's:
   ```
   ~/.claude/skills/
   ```
   On Windows it's usually:
   ```
   C:\Users\<you>\.claude\skills\
   ```
   If the `skills` folder isn't there yet, just create it.

2. Get the files from GitHub: go to https://github.com/EnergySteve/magic-graphics, click the
   green **Code** button → **Download ZIP**, and unzip it (or `git clone` it if you know how).

3. Put the files into a folder called `magic-graphics` inside your skills folder, so that
   `SKILL.md` ends up here:
   ```
   ~/.claude/skills/magic-graphics/SKILL.md
   ~/.claude/skills/magic-graphics/assets/...
   ~/.claude/skills/magic-graphics/references/...
   ```
   (If your unzipped folder is named something like `magic-graphics-main`, just rename it to
   `magic-graphics`.)

4. Start a **new** Claude chat (so it picks up the new skill).

Done.

---

## Check that it worked

Start a fresh chat and say:

> make me some b-roll for my video

Magic Graphics should jump in, explain what b-roll is, and start walking you through making a clip.
If nothing happens, make sure the folder is in the right place (Option A, step 2) and that you
started a **new** chat after installing.

---

## Using it

You don't need to learn anything. Just talk:

- "make me a cool clip for my Instagram"
- "I need a hype intro for my barbershop reel"
- "make a stat clip that says over 500 members"

It asks a few simple questions, makes the clip, opens it for you, and shows you how to turn it
into a video you can post. If you're ever unsure, just say "you pick" and it'll choose for you.

Have fun. ✨
