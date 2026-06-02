# Weekly Meal Plan

Context and history for a consistently built weekly meal plan, generated via Claude Code's `/weekly-menu` skill.

## How it works

1. Say "I'm ready for my meal plan" in Claude Code
2. Claude asks for on-hand ingredients and any preferences for the week
3. Claude generates a Mon–Thu plan, avoiding recipes used in the past 8 weeks
4. After confirmation, Claude saves to Obsidian, syncs to Google Sheets, and pushes the history update here

## Files

- `meal_history.md` — auto-updated log of every recipe used, week by week

## Meal plan rules (for reference)

- 2 women, Mon–Thu only
- P1: 8 × 5oz portions (lunch + dinner all 4 days)
- P2: 6 × 5oz portions (Mon L+D, Tue D, Wed D, Thu L+D)
- No same protein at lunch and dinner on the same day
- Each lunch = previous night's dinner leftovers
- Wednesday dinner is always a big-batch soup (covers Thu lunch too)
- Seafood on Mon or Tue; proteins rotate: chicken, beef, pork, seafood
- One featured recipe sourced from playswellwithbutter.com each week
- Seasonal vegetables, zero-waste rule (each veg in 2+ meals)
- Daily macro targets: 126g pro / 58g fat / 120g carbs
