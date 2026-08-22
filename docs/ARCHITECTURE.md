# Architecture

## MVP now

The GitHub Pages app is local-first. It stores working inventory, deals and the draft plan in browser localStorage so the interface can be tested immediately from iOS without authentication.

The repository JSON files remain the canonical examples for future persisted/shared data.

## Planning layers

### Deterministic
- quantities and units
- inventory subtraction
- nutrition totals
- Thermomix share
- minimum fish/vegetarian constraints
- dates and week state
- grocery gaps

### AI-assisted
- identify produce from photos
- interpret flyer screenshots and URLs
- normalize recipe ingredients
- estimate missing nutrition
- rank candidate recipes
- propose substitutions
- explain why a meal was suggested

## Cookidoo

Official Cookidoo recipes should remain references/links. New or adapted recipes should be stored in `cookidoo-bridge`, rendered to an importable public recipe page, then imported into Cookidoo.

## Next integrations

1. GitHub persistence from iOS using a fine-grained token.
2. Share Sheet / Shortcut input for normalized JSON.
3. Photo intake workflow for Tuesday farm basket and garden harvest.
4. Weekly flyer normalization.
5. Nutrition engine and household portions.
6. Recipe scoring and swap alternatives.
7. Cookidoo action panel for official links and Cookidoo Bridge imports.
