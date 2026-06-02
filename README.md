# Weekly Meal Plan

A structured, repeatable meal planning system for two, generated weekly via Claude Code. This repo stores the rules, constraints, and history that keep every plan consistent and non-repetitive.

---

## How it works

1. Say **"I'm ready for my meal plan"** in Claude Code
2. Claude asks two questions:
   - What do you have on hand this week? *(proteins, produce, pantry items to use up)*
   - Any preferences or constraints? *(e.g. "no chicken", "want something Thai", "light meals — traveling Thursday")*
3. Claude generates a full Mon–Thu plan, avoiding any recipe used in the past 8 weeks
4. You review and confirm (or adjust)
5. Claude saves to Obsidian, syncs to Google Sheets, and pushes the updated history here

---

## Who this is for

Two women eating lunch and dinner Monday through Thursday.

| Person | Portions per week |
|--------|------------------|
| P1 | 8 × 5oz — lunch + dinner all 4 days |
| P2 | 6 × 5oz — Mon L+D, Tue D, Wed D, Thu L+D |

---

## Meal plan rules

### Structure
- Each lunch is the **previous night's dinner as leftovers** — no separate lunch prep
- **Wednesday dinner is always a big-batch soup** — covers Wed dinner + Thu lunch for both
- No same protein at lunch and dinner on the same day

### Proteins
- Rotate through: **chicken, beef, pork, seafood**
- Seafood must fall on **Monday or Tuesday**

### Vegetables
- Seasonal only
- **Zero-waste rule** — every vegetable appears in at least 2 meals
- Amounts specified in every cell of the plan

### Featured recipe
- One recipe sourced each week from [playswellwithbutter.com/weeknight-recipes](https://playswellwithbutter.com/occasion/weeknight-recipes/)
- Must fit constraints: no pasta, no noodles, no taco shells
- Good formats: bowls, sheet pan, stir-fry, skillet, curry

### Macros
- Daily target: **126g protein / 58g fat / 120g carbs**
- Breakfast is assumed at 30g pro / 5g fat / 35g carbs
- Lunch + dinner tracked against remaining: **96g pro / 53g fat / 85g carbs**

---

## Weekly output

Every confirmed plan produces:

1. **Protein Tracker** — portion counts per person
2. **Meal Plan table** — each cell includes protein, veg, sauce, amounts, and prep steps
3. **Daily Macro Summary** — L+D actuals vs. remaining targets
4. **Vegetable Audit** — flags any single-use veg before finalizing
5. **Grocery List** — proteins in lbs, produce, pantry pull
6. **Prep Notes** — batch cook instructions and timing

Saved to:
- Obsidian: `Health/Meal Plans/Week of YYYY-MM-DD.md`
- Obsidian: `Health/Meal Plans/Grocery List - Week of YYYY-MM-DD.md`
- Google Sheets (via webhook)
- This repo: `meal_history.md` (auto-updated)

---

## Recipe history

`meal_history.md` is automatically updated after every confirmed plan. It logs the four dinners + featured recipe for each week. Claude uses this to enforce an **8-week non-repeat window** — no recipe is reused until it has been out of rotation for at least 8 weeks.

---

## Files

| File | Description |
|------|-------------|
| `meal_history.md` | Auto-updated weekly recipe log |
| `README.md` | This file — rules, structure, and workflow reference |
