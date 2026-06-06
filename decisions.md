# Globetrotter — Decisions Log

## Milestone 0: Setup and Planning
- **Destination chosen:** Johannesburg, ZA
- **Primary audience:** First-time visitors from the U.S.
- **One design decision that reflects the destination:** Lots of red and yellow; Zulu, Sesotho, and Setwana phrases sprinkled throughout.
- **Wireframe format used (hand-drawn / Figma / other):** Figma

## Milestone 1: HTML Structure
- **HTML structure choice and why:** I used repeated `<article>` cards inside section containers (like `wireframe-row` and `gallery-tile`) so each attraction/food/gallery item is a self-contained content block with consistent structure.
- **One Claude-generated thing I changed:** The gallery originally used duplicated image cards for an infinite loop effect; I replaced that with a cleaner carousel structure and controls because duplicate content was harder to maintain.
- **Where my wireframe guided structure:** I kept the site-level layout as header + main content on every page and separated each page into clear thematic sections (home intro, attractions cards, guide cards, gallery sections) to match the wireframe hierarchy.

## Milestone 2: CSS Styling
- **Color/font choice and why it serves the destination:** I used warm/dark overlays with light text and accent yellow buttons to keep the site vibrant and readable, and paired `TajamukaScript` with `Montserrat` to reflect the destination's personality while keeping controls legible.
- **One Claude suggestion I rejected and why:** I tested `Montserrat` for the language area but switched the language label styling back to `TajamukaScript` so the header felt more aligned with the cultural tone I wanted.
- **One style that looked wrong at first and what I changed:** The "more info" food links looked like plain links, so I changed them into gray button-style links (`.info-button`) with hover/active states for clearer calls to action.

## Milestone 3: Flexbox Layout
- **One Flexbox property choice and why:** I used `display: flex` with `justify-content: space-between` and responsive wrapping/stacking on key sections (hero and header) so the layout can spread horizontally on desktop but still reorganize cleanly.
- **One place Claude layout did not match my plan and what I changed:** The home hero image initially sat above the "Discover Johannesburg" text; I restructured the hero and updated layout rules so the image sits to the right on larger screens.
- **One layout challenge that required HTML adjustment:** To support the side-by-side hero layout, I added a dedicated `.hero-copy` wrapper around the heading/paragraph/button so text and image could be controlled as separate flex items.

## Milestone 4: Responsive Design
- **Breakpoints used and why:** I used `900px` for major layout shifts (stacking feature rows and hero) and `768px` for phone-focused refinements (header wrapping, full-width search input, nav sizing).
- **One section where mobile needed to feel genuinely different:** The header/navigation needed a different mobile behavior, so I used the checkbox-triggered slide-out menu and reflowed controls (`search` and `language`) instead of shrinking the desktop layout only.
- **One Claude breakpoint suggestion I accepted/rejected and why:** I accepted moving key components to full width on smaller screens (like search input and nav list items) because it improves tap targets and readability in actual phone use.

## Stretch Features
- **Additional Media:** Implemented. I embedded a YouTube video on the home page to add non-image media tied to destination context.
- **Enhanced Layouts:** Implemented. I used CSS Grid in multiple sections (e.g., card rows and media feature layout) where grid provided better two/three-part alignment than basic flex rows.
- **Interactive Navigation:** Partially implemented. I built an interactive slide-out menu toggle, but I did not implement a nested dropdown submenu.
- **Custom Styling:** Implemented. I used custom fonts and additional effects (carousel controls, transitions, blur/overlay styling, and interactive button states) for a personalized look and feel.

Possible additional pages: famous people from joburg, fun facts about joburg