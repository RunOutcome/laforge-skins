# Contributing a theme

The library collection gathers LaForge themes from the community. *Theme* and
*skin* mean the same thing; LaForge's command line says `la skin`.

## What a theme here must be

- **Original work.** Your own design, with no one else's trademarks, logos,
  characters or a franchise's recognisable look. Fan themes belong in your own
  repository, which anyone can add to LaForge by link.
- **Both modes.** Light and dark, each with readable contrast (text at 4.5:1 or
  better).
- **Licensed.** A `license` and an `author` in `skin.json` for your files, and
  the licence text of any font you bundle (SIL OFL or Apache-2.0 fonts only).
- **Data only.** Stylesheets, fonts and images, every rule scoped to
  `[data-skin='<name>']`. No scripts, HTML or links.
- **Clean.** `la skin check --strict skins/<name>` passes with no warnings.

## How

1. Start one with `la skin new <name> skins/<name>`, or follow the tutorial at
   https://getlaforge.com/themes/make-a-theme/. An agent can build it with the
   `laforge-theme` skill:
   https://github.com/RunOutcome/laforge/tree/main/.claude/skills/laforge-theme
2. Install it and look at it in both modes (`la skin install skins/<name>`).
3. Add `preview-dark.png` and `preview-light.png` to its folder (1400 wide) and
   an entry to `collection.json`:
   `{"name": "<name>", "label": "…", "description": "…", "path": "skins/<name>"}`.
4. Open a pull request with one theme per pull request.

The full reference is
[docs/skins.md](https://github.com/RunOutcome/laforge/blob/main/docs/skins.md).
