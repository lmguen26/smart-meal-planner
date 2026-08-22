# Smart Meal Planner

Personal weekly meal-planning system combining food inventory, garden and farm produce, grocery specials, nutrition targets, Cookidoo recipes, custom recipes, meal approval, and grocery planning.

## Core flow
1. Capture pantry/freezer/garden/farm-basket inventory.
2. Normalize useful weekly grocery offers.
3. Maintain nutrition and planning targets.
4. Collect candidate recipes from Cookidoo, Cookidoo Bridge, and ordinary meals.
5. Score and propose a balanced week.
6. Human approves or swaps meals.
7. Generate grocery requirements after subtracting inventory.
8. Send new/adapted Thermomix recipes through `cookidoo-bridge`; retain official Cookidoo links for direct use.

## MVP
- `data/inventory/current.json`
- `data/offers/current.json`
- `data/targets.json`
- `data/recipes.json`
- `data/plans/current.json`
- `schema/`
- `app/`

AI handles fuzzy interpretation and suggestions. Deterministic code owns quantities, inventory, nutrition totals, grocery subtraction, dates, IDs and constraint checking.
