# RoomieSync v3 — Cycle 1

A mobile-first, single-browser prototype to help housemates coordinate cleaning, shopping, announcements, and optional shared-space plans.

## Run
Open `index.html` in a modern browser. No installation or server is required.

## Features
- Simple dashboard showing tasks, shopping essentials, and latest notice
- Real-name profile with optional nickname; automatic author names
- Household member list and assignee selection
- Cleaning tasks with completion and deletion
- Shared shopping list with completion and deletion
- House notices and guidelines
- Optional shared-space schedule (not mandatory reservations)
- Browser localStorage persistence

## Limitations
This is a **local prototype**: data is stored in the current browser and **does not synchronize between roommates' devices**. There is no authentication or backend. Previously stored v2 tasks and rules are imported when available; old mandatory reservations are not imported as optional plans.

## v2 → v3 design rationale
Classroom feedback: (1) homepage felt cluttered; (2) 'Booking' sounded inappropriate for a home; (3) workflows should be quick and intuitive; (4) repeated free-text names and nicknames made identity unclear; (5) mandatory shared-space reservations felt unnecessary. v3 responds with a simplified dashboard, optional shared schedule, profile and member list, and clearer navigation. The original time-overlap issue was rechecked and was not reproducible; it is not presented as a confirmed defect.

## Suggested testing
1. Set profile with real name and nickname. Confirm both appear in House.
2. Add a housemate and assign a cleaning task from the dropdown.
3. Add and check off a shopping item.
4. Post a notice and confirm it appears on Home.
5. Add two overlapping optional plans. Confirm both remain visible (plans are not reservations).
6. Refresh the page and confirm data remains in the same browser.
