# Duty Limit Check

Static, offline-capable web app (`index.html`, `sw.js`, `manifest.webmanifest`, icons) served by GitHub Pages from `main`. Martin, a cabin manager, uses the live site on his phone.

## Workflow

- Never push straight to `main`: it is the live app. Make each change on its own branch and open a pull request for Annu to review and merge.
- When any file changes, bump `CACHE` in `sw.js` so installed copies refresh.
- Test at phone width (about 375px) and check the page never scrolls sideways.

## Product decisions so far

- Default duty limit 20h 30m, editable, remembered on the phone. Nothing else is saved (crew stay-or-leave decisions are planned for V2).
- Delays after sign-on and medical time count towards duty.
- Time on duty so far is counted from sign-on using the phone's clock; "Still to come" fields hold only future time.
- Sign-on and sign-off each have their own time zone. Sign-off times show in the destination zone. Time zone data comes from the phone's built-in `Intl` API.
