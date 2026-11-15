# Websites project

This repository is Netanya's shared home for assorted personal websites, reports and tools.

## Repository and publishing

- Repository: Netanyar/websites.
- Live directory: https://netanyar.github.io/websites/
- GitHub Pages deploys the main branch from the repository root.
- Use the connected GitHub tools to inspect and change this repository when available. They also work when the local shell cannot reach GitHub.
- Read the current repository state before editing. Preserve unrelated work and use current commit/blob SHAs for writes.
- For requests to build or update a published website, implement, validate and publish the requested changes unless the user asks for a draft or local-only work.
- After publishing, check the GitHub Pages deployment result and return the relevant live URL. Report verification limits accurately.

## Site structure

- The root index.html is a directory of hosted projects. Keep it as the collection homepage.
- Give each independent website its own descriptive folder containing index.html and its assets.
- Add each new website to the root directory with a concise title and description.
- The existing stay recommendations website lives at stays/ with its map and 30 city reports across Asia and Europe.
- Stay report paths follow stays/<city>/, such as stays/bangkok/.
- Keep city navigation within the stay website and provide a link from its homepage back to the root directory.
- Legacy root city URLs redirect to the nested stay reports. Preserve these redirects and their query-string/fragment handling.
- Use relative internal links and asset paths compatible with the /websites/ GitHub Pages prefix.
- Prefer simple static HTML, CSS and JavaScript when sufficient for the request.

## Quality and maintenance

- Keep pages concise, easy to scan, responsive and accessible.
- Check internal navigation and asset paths after moving pages.
- Preserve existing content and functionality unless the requested change calls for editing them.
- Keep README.md current when project structure or publishing instructions change.
- This repository and its published pages are public. Do not commit credentials or private personal information.
