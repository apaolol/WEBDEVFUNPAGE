# Valorant Agent Picks

A small static website where our group shares two favorite VALORANT agents per person. The landing page links to eight agent pages with portraits, roles, ability details, and personal notes or video links.

## Open the site

1. Open `index.html` in a browser.
2. Choose an agent card to open that agent's page.
3. Use the back link or page navigation to return to another page.

This is a static HTML and CSS project. It does not need `npm`, a build step, or a local server. An internet connection is needed for the external stylesheet, agent artwork and ability icons, and YouTube links.

## Project structure

```text
WEBDEVFUNPAGE/
├── index.html
├── README.md
├── assets/
│   └── images/
│       └── agent-placeholder.svg
├── css/
│   ├── universalStyles.css
│   ├── landing_page.css
│   └── agent_page.css
└── pages/
    ├── kyle_breach.html
    ├── kyle_reyna.html
    ├── charles-slot-1.html
    ├── charles-slot-2.html
    ├── joshua-slot-1.html
    ├── joshua-slot-2.html
    ├── symond-slot-1.html
    └── symond-slot-2.html
```

## Pages and styles

- `index.html` is the landing page. Each agent card links to its matching file in `pages/`.
- `css/universalStyles.css` contains shared styles such as headers, rows, columns, boxes, buttons, and agent profile sections.
- `css/landing_page.css` contains the landing page layout and the different colors for Kyle's Breach and Reyna cards.
- `css/agent_page.css` contains the shared agent page styling and each agent's portrait background color.
- Each agent page loads the shared stylesheet and the same `agent_page.css`, so spacing and layout stay consistent.

## Design references

The visual direction is neo-brutalist: square panels, visible borders, hard offset shadows, and bright accent colors. We adapted this style for a dark VALORANT theme instead of copying a complete page unchanged.

- [BRUT UI Kit](https://github.com/Unal-Inanli/brut-ui) — the landing page loads its `@sprtn/ui` stylesheet from jsDelivr and uses its `brut-btn` button classes. The kit's [examples page](https://unal-inanli.github.io/brut-ui/examples) includes a landing page and other ready-made compositions that informed the layout direction.
- [HyperUI neo-brutalism cards](https://www.hyperui.dev/components/neobrutalism/cards/) — reference for hard-edged cards and offset shadows.
- [HyperUI neo-brutalism buttons](https://www.hyperui.dev/components/neobrutalism/buttons/) — reference for bold buttons and hover styling.

The page structure, dark palette, agent colors, text, and final CSS were adapted for this project. The HyperUI pages are visual references; this project does not use their Tailwind code.

## AI assistance and group work

AI assistance created the initial backbone and wireframes, including a starting page structure, page links, and starter HTML and CSS. That was the starting point, not the finished project.

Our group coded and finalized the pages from that scaffold. We chose the agents and wrote and edited the final page content, selected and added the agent portraits and ability images, set up the navigation and video links, and customized the final dark colors and styles. We also built the page layouts with Flexbox using the row-and-column approach practiced in Sir's “Box-Box” activity. The `.row` and `.col` classes apply that lesson across the landing page and agent pages.

AI helped us get the project started, while the group made the content and design decisions and completed the final implementation.

## External media and project scope

- Agent portraits and ability icons are loaded from `media.valorant-api.com` URLs in the HTML pages.
- Video buttons open YouTube in a new tab; videos are not embedded in the page.
- The VALORANT logo is loaded from Wikimedia Commons.
- This site is a fan-made school project and is not an official VALORANT site.
