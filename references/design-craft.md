# Design craft - what makes a clip actually look good

Read this when you're building anything beyond a one-word clip - especially a multi-beat story
clip (`story-beats.html`). These are the rules that make the difference between "a random animation"
and "a clip that looks pro." The user never needs to know any of this - it's your craft, not theirs.

## 1. Brand kits (named looks - pick one FOR the user)

A "look" is just an accent color + a background + a vibe. Don't ask a non-techy person for a hex code.
Offer them a named look and pick a great default. Each look is drop-in values for any template's EDIT block.

**Bold Gold** (the default - premium, hype, looks great on everything)
```
ACCENT = "#F2C94C"   BG = "#070708"   TEXT = "#FFFFFF"
```

**Clean & Premium** (calm, expensive, "Apple-keynote" feel - light background)
```
ACCENT = "#D97757"   BG = "#F5F4EE"   TEXT = "#2A2925"
```
Use this only on the text-based templates (`story-beats`, `title-slam`, `kinetic-type`, `handle-reveal`).
The glow-on-black ones (`text-particles`, `glowing-chart`, `liquid-gradient`) need a dark background to
read, so keep those on Bold Gold or another dark look.

**Your Color** (their brand, instant rebrand)
The whole point of a kit: take ONE color from the user and the clip reskins. Convert their words to a
hex (gold `#F2C94C`, hot pink `#FF4FA3`, electric blue `#3AA0FF`, coral `#D97757`, mint `#46D9A0`),
set it as `ACCENT`, keep `BG` near-black `#070708` and `TEXT` white. Bright accent on dark always pops.

**The lesson:** same template, swap the kit -> totally different feel. Offer 2-3 named looks + "your color,"
never a blank "what colors?" question.

## 2. Think in beats (this is the big one)

A real "video" isn't one animation - it's a short list of **beats**. Each beat = one small caption + one
clear thing on screen, held ~2-3 seconds, then it crossfades to the next. That rhythm is what makes a clip
feel like a story instead of a flash.

When someone wants more than a single word (a mini-story, an explainer, "show my before/after," a hook ->
payoff), map their idea to 3-5 beats and use `story-beats.html`. A reliable beat shape:

- **Hook / problem** -> **turn / fix** -> **payoff / result.** (3 beats, dead simple, works for almost anything.)
- Stat version: **setup** -> **the number** -> **what it means.**
- Hype version: **who** -> **what they do** -> **the call to action.**

Example for a barbershop: `THE LOOK` / "FRESH FADES" -> `THE FEEL` / "WALK OUT NEW" -> `BOOK NOW` / "LINK IN BIO".

## 3. The six rules that make any clip read well

1. **One idea per beat.** More than one thing on screen at once = confusing. Keep each moment to a single point.
2. **A big caption that swaps per beat.** The viewer should always know what's happening with the sound off.
   Big bold line + a small kicker line above it.
3. **Crossfade, don't hard-cut.** A soft ~0.4s fade between beats feels smooth and intentional. (Built into `story-beats`.)
4. **End on the payoff and hold it.** The last beat is the point - let it sit ~2 seconds longer and pop it in the accent.
5. **One accent only.** Pick a single accent color and let it carry the highlights. Two accents fight.
6. **Always 1080x1920 (tall).** Every template is already this. Never go wide - these live on phones.

## 4. Which template for which job

| What they want | Template |
|---|---|
| A short story / explainer / before->after / hook->payoff (3-5 beats) | `story-beats.html` |
| A big number / stat / milestone | `glowing-chart.html` |
| A punchy line / hype / hook (a few words) | `title-slam.html` |
| A quote that builds word by word | `kinetic-type.html` |
| One powerful word bursting | `text-particles.html` |
| A name / handle intro or outro | `handle-reveal.html` |
| A dreamy moving background to lay footage/text on (classic b-roll) | `liquid-gradient.html` |

If they're not sure, a 3-beat `story-beats` clip in Bold Gold is the safest, most-impressive default.
