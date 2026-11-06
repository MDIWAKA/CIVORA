# CIVORA: Smart City & Smart Village Platform

> Smarter Services. Connected Communities. Better Living.

CIVORA is a working front-end prototype of a civic management platform. It has two connected portals: a **Citizen Portal** for residents and an **Authorities Portal** for officials. Actions in one portal show up in the other, for example a complaint reported by a citizen appears on the officer dashboard, and an officer's status update sends the citizen a notification.

This is a prototype with demo data. There is no real backend, and all data is stored only in the visitor's own browser (`localStorage`).

## Main features

### Citizen Portal
- **Zero-Mile:** find nearby e-Sevai centres, hospitals and offices; search by service or specialist; see online vs visit-needed services, document checklists, specialist availability and directions.
- **City Memory:** report road, drainage, water, waste and streetlight problems with a map location and photo; duplicate-complaint check; status tracker; repair history; confirm or reject a fix.
- **Q-Less:** live queue length and wait estimate, digital tokens, appointment slots, arrival planning, "your turn is near" alerts, and news or tips while waiting.
- **Reverse Route:** request services that are hard to reach, see mobile service van schedules, and register before the van arrives.

### Authorities Portal (role-based, demo PIN `1234`)
- **Overview:** statistics, charts and department performance.
- **City Memory:** complaint map, filters, recurring-problem detection, assignment, status and priority updates, repair notes and completion photos.
- **Q-Less:** per-centre dashboards, counter and service-time settings, call next token, walk-ins, pause/resume and peak-hour demand.
- **Reverse Route:** village demand map, recommended next stop, route order, visit planning and publishing to citizens, coverage report.
- **Zero-Mile:** manage centres, hours, holidays, online services, specialists and document checklists.

### Shared
Notifications, role-based access (five demo roles), a responsive layout for phones, tablets and desktops, large touch targets, and light/dark mode that follows the device setting.

## Technologies used
- HTML5, CSS3 and vanilla JavaScript (no framework, no build step)
- Inline SVG for maps and icons
- Google Fonts: *Atkinson Hyperlegible* (loaded online, falls back to system fonts)
- Browser `localStorage` for demo data

## Folder structure
```
civora/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── README.md
├── LICENSE
└── .gitignore
```

## Installation and running locally
No installation is needed.

1. Download or clone this repository.
2. Double-click `index.html` to open it in a browser, **or** run a small local server from the project folder: `python3 -m http.server 8000` and open `http://localhost:8000`.

## Deploy with GitHub Pages
1. Create a new public repository on GitHub and upload all the files, keeping the `css` and `js` folders.
2. Open the repository **Settings**, then **Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose branch **main** and folder **/ (root)**, then **Save**.
4. Wait one or two minutes. Your site will be live at `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY-NAME/`.

## Demo sign-in
- **Citizen:** any name and a 10-digit number.
- **Authorities:** pick a role and use PIN `1234`.
- **Reset demo data:** button on the sign-in screen.

## Known limits
- The map is a simplified schematic, not real map tiles.
- Queue movement is simulated every few seconds.
- No real accounts, SMS or server. Data does not sync between devices.

## Credits and contributors
- Concept and product brief: Diwakar
- Prototype built with the help of Claude (Anthropic)
- Contributors: add your name here

## License
See the `LICENSE` file. By default this project is **All Rights Reserved**. If you want others to be able to reuse it, replace the file with an open-source license of your choice, such as MIT, using GitHub's "Add file > Create new file > LICENSE" license picker.
