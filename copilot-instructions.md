# Copilot Instructions

This repository uses AI-assisted design and development to build a social bingo web app.

## Design Guide

When working on UI and styling, follow these principles:

- Aim for a strong visual identity: pick a theme and carry it consistently across the lobby, grid, and victory state.
- Use the existing CSS utility file at `socops/src/main/resources/static/css/app.css` to add or extend styles.
- Keep layout responsive and readable, especially for the 5×5 bingo grid.
- Prefer distinct UI states for inactive tiles, selected tiles, free-space tile, and bingo victory.
- Use animation sparingly: focus on entrance effects, button hover feedback, and victory celebration.
- If you redesign the interface, update the instructions here and keep the design rationale clear.

## Project files relevant to design

- `socops/src/main/resources/templates/game.html` — main page structure and component layout
- `socops/src/main/resources/static/css/app.css` — application styling utilities and theme definitions
- `socops/src/main/java/com/socops/service/BoardAssembler.java` — game logic can influence UI state, but style changes belong in HTML/CSS

## Suggested workflow

1. Start with a design plan in chat.
2. Apply visual changes in `game.html` and `app.css`.
3. Run the app locally to review the new theme.
4. Add or update this document when the visual direction changes.

## Notes

- Keep the experience playful and accessible.
- Use color, spacing, and typography to reinforce the theme.
- Avoid adding heavy third-party libraries for the frontend; prefer CSS-based effects.
