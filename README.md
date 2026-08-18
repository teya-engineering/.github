# .github

Org-level configuration for [@teya-engineering](https://github.com/teya-engineering).

Nothing here is a project. This repo holds the files GitHub reads for the
organisation as a whole.

## What's in here

| Path | What it does |
| :-- | :-- |
| `profile/README.md` | The page shown at [github.com/teya-engineering](https://github.com/teya-engineering). This is the public front door. |
| `profile/assets/` | Branded images for that page, plus the SVG sources they were rendered from. |

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

## Changing profile artwork

The images are rendered from the SVGs next to them, so edit the SVG rather than
the PNG. Render every asset at its source size:

```sh
cd profile/assets
for source in *.svg; do
  rsvg-convert -o "${source%.svg}.png" "$source"
done
```

`rsvg-convert` comes from `librsvg` (`brew install librsvg`). Any SVG renderer
works, as long as the output keeps the dimensions declared in each SVG. The
artwork is rendered at two times its display size, except for the banner, which
is 2400px wide.

Figtree must be installed before rendering because the profile artwork uses it.
Keep the image names stable so the links in `profile/README.md` continue to
work.
