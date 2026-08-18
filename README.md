# .github

Org-level configuration for [@teya-engineering](https://github.com/teya-engineering).

Nothing here is a project. This repo holds the files GitHub reads for the
organisation as a whole.

## What's in here

| Path | What it does |
| :-- | :-- |
| `profile/README.md` | The page shown at [github.com/teya-engineering](https://github.com/teya-engineering). This is the public front door. |
| `profile/assets/` | Banner images for that page, in light and dark, plus the SVG sources they were rendered from. |

Note that `profile/README.md` is the one that renders publicly. This root file
is only visible to people who open the repo directly.

## Listing projects on the profile

The profile page does not list individual repositories. Public repos in the org
already show up on the organisation page on their own, ordered by GitHub, and
each one carries its own description and topics.

If you later want a curated list instead, pin the repos you care about from the
organisation page, or add a table to `profile/README.md` above **How we build**.
Keep any such list to one plain sentence per project, describing the problem it
solves. Anyone skimming the page is deciding whether to click, not reading
documentation.

## Changing the banner

The images are rendered from the SVGs next to them, so edit the SVG rather than
the PNG:

```sh
cd profile/assets
rsvg-convert -w 2400 -o banner-dark.png banner-dark.svg
rsvg-convert -w 2400 -o banner-light.png banner-light.svg
```

`rsvg-convert` comes from `librsvg` (`brew install librsvg`). Any SVG renderer
works, as long as the output stays 2400px wide so the banner is sharp on retina
screens.

Swapping in artwork from the brand team is fine too. Keep both a light and a
dark variant, since the profile page picks one based on the visitor's GitHub
theme, and keep the file names the same so the links in `profile/README.md`
keep working.
