# Websites

Published at https://netanyar.github.io/websites/

## Projects

- [Where to stay](stays/) — 30 neighbourhood reports across Asia and Europe.

- [Meridian — Learn history](history/) — six introductory lessons about Europe, 1789–1991, a shared historical datastore and self-assessed spaced review.

Each project lives in its own folder with an index.html and its assets. Add each new project to the directory in the root index.html. Keep project links relative so they work on GitHub Pages.

The stay guide lives under stays/; the old city URLs redirect to the corresponding nested reports, preserving query strings and fragments.

GitHub Pages deploys main from the repository root. This repository and its published pages are public.

## History data and progress

`history/data.json` is the source of truth for course entries, stable question IDs, key ideas, prerequisites, locator places and sources. Each initial entry forms a short lesson with three ideas and two recall questions. Keep IDs stable when editing content so saved review history continues to work. Broader coverage and historical border polygons are future additions; the map currently locates cities on coastlines only.

Learning progress is separate from content, stored in browser localStorage under `meridian-progress-v1`, with JSON export/import. Missed answers return in 10 minutes, partial answers in 1 day, and correct answers in 3 days, increasing by 2.2 after consecutive successes (maximum 180 days). Completion tracks exploration rather than mastery. No account or API key is required.

Locator coastlines are derived from Natural Earth 1:110m land, public domain (https://www.naturalearthdata.com/). Optional Google Fonts fall back to local system fonts. Sources for lesson content are linked within each entry.
