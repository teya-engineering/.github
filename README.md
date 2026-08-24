# .github

Org-level configuration for [@teya-engineering](https://github.com/teya-engineering).

Nothing here is a project. This repo holds the files GitHub reads for the
organisation as a whole.

## What's in here

| Path                | What it does                                                                                                         |
|:--------------------|:---------------------------------------------------------------------------------------------------------------------|
| `profile/README.md` | The page shown at [github.com/teya-engineering](https://github.com/teya-engineering). This is the public front door. |
| `profile/assets/`   | Branded images for that page.                                                                                        |

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

Replace the exported PNG files in `profile/assets` and keep their names stable
so the links in `profile/README.md` continue to work. The artwork is rendered
at two times its display size. The banner is 2400 x 682 pixels, section headings
are 1760 x 200 pixels, the technology strip is 1330 x 78 pixels, and the hiring
panel is 1760 x 655 pixels.
