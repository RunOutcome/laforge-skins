# LaForge skin library

More skins for [LaForge](https://github.com/RunOutcome/laforge), beyond the
official ones released with it (those live in LaForge's own `skins/` folder).

## Install

In the theme panel: **Themes → Get more → LaForge library**, then Install on
a skin, or Install all. From a terminal:

```sh
la skin browse library           # what is here
la skin install library/NAME     # one skin
la skin install library          # all of them
```

## Add a skin

1. Make it as LaForge's `docs/skins.md` describes, in `skins/<name>/`:
   `skin.json`, stylesheets, fonts and images only. No code.
2. It draws **both light and dark**.
3. Original work only: no trademarks, logos or a franchise's look. Fonts
   under the SIL OFL or Apache-2.0, bundled with their licence.
4. Add it to `collection.json`, check `la skin install ./skins/<name>`, and
   open a pull request.

Skins here are Apache-2.0 unless their folder says otherwise.
