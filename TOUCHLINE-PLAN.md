# Touchline — agreed project plan

## Overall goal
Create one website combining:
- A football manager simulator inspired by the structure and depth of FC Manager Career.
- A football database for six competitions: Premier League, English Championship, La Liga, Bundesliga, Serie A and Ligue 1.

## Interface direction
- Dark interface, white text, green highlights.
- Clean, modern, easy to navigate, responsive on desktop and mobile.
- Main areas: Home, Leagues, Transfers, Fixtures, Squads, Tactics, Match Centre and Database.
- Home hub should make the next match and club status easy to find.

## Career mode requirements
- Choose a club from the six supported competitions when starting a career.
- Editable starting XI and formations.
- Searchable transfer market.
- Transfer activity restricted to the correct real-world/season transfer windows.
- Fixtures and league tables update as matches are played.
- Match viewing uses a 2D pitch with dots for players and a ball. Similar-colour teams must use clearly distinguishable shades.
- Club badges/crests should be supported.
- Career saves must remain separate from updates to the real-world database.

## Football database requirements
- Cover all six competitions.
- Keep club membership, squads, fixtures, results, standings and confirmed transfers.
- Prioritise official league and club sources, with reliable corroboration.
- Separate confirmed information from rumours/unconfirmed reports.
- Date-stamp data and show when information was last checked.
- Flag stale, missing or conflicting information rather than silently guessing.

## Data refresh workflow
- Initial workflow: prepare a reviewed update file and import it into Touchline.
- Design the database so automatic data-provider integration can be added later.
- A scheduled weekly research report is separate from the website; it does not automatically edit the website or its local files.
- Never overwrite an existing career save when importing updated real-world data.

## Technology direction
- Front end: React + TypeScript + Vite.
- Source control: GitHub.
- Hosting: Vercel (not Netlify).
- Future backend: a database service can be selected once the local prototype and data structure are settled.

## Current prototype status
- The first runnable starter is included in this project.
- It has a basic responsive interface, sample clubs/player records, club selection, basic career state, squad position editing, tactics formation board, searchable transfer market, a simple match result generator, local save/load, and JSON import/export.
- The included football records are sample data and are not verified 2026/27 facts.
- The match engine, accurate live database, complete six-league club lists, proper fixtures/table calculations, multi-save system, and online accounts remain to be built.
