# Hispanic Heritage — 30 People

A web edition of the classroom deck *Hispanic Heritage: 30 People, Dynamic Edition*, built for
grades 9–12 English learners. Thirty bilingual biography profiles, each with a discussion question
and a sentence-frame language support, plus the four classroom projects that follow the profiles.

Published under [radan55.github.io](https://radan55.github.io) as part of the EL Publishing
resource ecosystem.

## What's here

```
hispanic-heritage/
├── index.html        the whole site — markup, styles, script, and profile data inline
├── profiles.json     the same 30 profiles as data, for reuse in other tools
├── images/           full-size illustrations (900px, ~200 KB each)
├── thumbs/           grid thumbnails (420px, ~50 KB each)
└── README.md
```

No build step and no dependencies. Fonts load from Google Fonts; everything else is local.

## Live address

`radan55.github.io/hispanic-heritage/`

## What the page does

- **Grid of 30** with illustration, name, and roles.
- **Filter chips** by field — science and health, justice and community, arts and music, words and
  learning, sports — plus a search box that matches names, roles, and fields.
- **Language toggle** for Both, EN only, or ES only. Set it to ES for a newcomer and hand them the
  Chromebook.
- **Profile view** with the English text, the Spanish text, the discussion question, the sentence
  frame, and a link to the source used for that biography. Arrow keys move between profiles.
- **Projects section** with the four assignments: two lives one connection, the research feature,
  the classroom gallery, and evidence of learning.
- **Print** drops the controls and prints the grid three across.

## Editing content

All thirty profiles live in one place: the `<script id="data">` block near the bottom of
`index.html`. Each entry looks like this.

```json
{
  "n": 1,
  "name": "Ellen Ochoa",
  "roles": "Engineer, Astronaut, Leader",
  "en": "…",
  "es": "…",
  "q": "What preparation might a space mission require?",
  "source": "https://…",
  "support": "Ellen Ochoa contributed by ___. This matters because ___.",
  "image": "images/01-ellen-ochoa.jpg",
  "thumb": "thumbs/01-ellen-ochoa.jpg",
  "cat": "Science, Space & Health"
}
```

Edit that block to change wording. Keep `profiles.json` in sync if you use it elsewhere. To add a
person, append an entry, drop the two image sizes into `images/` and `thumbs/`, and use one of the
existing `cat` values so the filter chips still work.

## About the illustrations

The portraits are AI-generated interpretations, not photographs. That is stated in the teacher
notes on the page, and it should be said out loud whenever the images are displayed. Facts come
from the linked source on each profile; students verifying a claim should go to the source, not
the picture.

## The original deck

The PowerPoint file is roughly 65 MB, which is too large to commit comfortably. Keep it in Drive
and link to it, or store it with Git LFS if you want it in the repo.

## Reuse

Written by Richard A. Daniel, M.Ed., ENL/EL Specialist, Laurel High School. Other educators are
welcome to adapt this for their own buildings.

Contact: rdaniel@laurelschools.org
