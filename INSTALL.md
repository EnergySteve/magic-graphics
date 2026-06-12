# Installing Magic Graphics (2 minutes)

Magic Graphics is a **skill** for Claude. To use it you need **Claude Code**, or a version of
Claude that supports Skills. If you can chat with Claude in a terminal or app and it can read
files on your computer, you're good.

---

## Fastest way - let Claude install it for you

Download Magic Graphics, then open Claude and paste this one line:

> **Install the Magic Graphics skill I just downloaded: find the `magic-graphics` folder (the one with `SKILL.md` inside) in my Downloads, copy it into `~/.claude/skills/`, then make me a quick test clip.**

That's it. Claude finds the folder, installs it, and makes you a clip to prove it works.
Start a new chat afterward and say "make me some b-roll for my video."

Prefer to do it yourself? Use one of the two manual ways below.

---

There are two ways to install by hand. Pick one.

---

## Option A - Drop in the folder (simplest, always works)

1. Find your Claude skills folder. On Mac or Linux it's:
   ```
   ~/.claude/skills/
   ```
   On Windows it's usually:
   ```
   C:\Users\<you>\.claude\skills\
   ```
   If the `skills` folder isn't there yet, just create it.

2. Copy the **`magic-graphics`** folder (the one with `SKILL.md` inside it) from this download
   into that `skills` folder. When you're done it should look like:
   ```
   ~/.claude/skills/magic-graphics/SKILL.md
   ~/.claude/skills/magic-graphics/assets/...
   ~/.claude/skills/magic-graphics/references/...
   ```

3. Start a **new** Claude chat (so it picks up the new skill).

Done.

---

## Option B - Install the packaged file

This repo also includes **`magic-graphics.skill`** - the same skill, zipped into one file.
If your version of Claude lets you install a `.skill` file directly, use that. If you're not
sure, just use Option A above - it always works.

(A `.skill` file is really a `.zip`. If you ever want to peek inside, rename it to
`magic-graphics.zip` and unzip it - you'll see the same folder from Option A.)

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
