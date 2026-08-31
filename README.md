# motion-brief

A Claude Agent Skill that turns a motion-graphics reference into a script and
direction document — *before* anything gets built.

A reference link is not a brief. "Make me something like this" plus a YouTube URL
is the most common way a motion project starts, and the most common way it ends
up rebuilt from scratch after the first render. This skill produces the document
a Remotion, HyperFrames, or After Effects build then follows.

## What it catches

Two failures sink these projects, and both happen before a single frame is built:

1. **The reference's palette is almost never the client's palette.** Copying it
   wholesale produces a film that looks great and belongs to someone else.
2. **Runtime gets budgeted from word count alone**, so the wordless beats — the
   holds, the breaths, the moments the reference is actually built around — get
   squeezed out and the pacing dies.

## How it works

Ten steps, in order:

| Step | What happens |
|---|---|
| 0 | Load the brand before watching anything |
| 1 | Get the file (YouTube, Vimeo, Pinterest, local) |
| 2 | Watch it as contact sheets |
| 3 | **Measure** the audio — loudness, instrumentation, arrangement. Don't guess |
| 4 | Name the register |
| 5 | The brand collision check (never skip) |
| 6 | Write the script |
| 7 | Budget runtime with wordless beats |
| 8 | Spec the sound from the measurements |
| 9 | Separate your calls from theirs |

The deliverable is a single direction document: script, beat sheet with
timings, sound spec, and an explicit list of what was inherited from the
reference versus what was decided for this brand.

## When it fires

- Someone shares a video reference and wants "something like this"
- A script, beat sheet, storyboard, treatment, or direction doc is requested for
  a promo, explainer, brand film, or sizzle reel
- A film needs its runtime, pacing, or sound specced
- A build is about to start from a one-line brief and a link

**Not** for building the film itself — that's the downstream framework's job.

## Install

Clone into your skills directory, or clone elsewhere and junction it:

```bash
git clone https://github.com/systoai-design/motion-brief.git ~/.claude/skills/motion-brief
```

## Related

Pairs with `motion-graphics-director` (which decides how much production
pipeline a piece needs) and the HyperFrames / Remotion skill families that
consume the brief.
