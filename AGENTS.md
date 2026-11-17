# Agent instructions

When the user texts you what they did and ate today:

1. Append (or create) the day's file in `logs/YYYY-MM-DD.md` using the format
   shown in the README.
2. Update the day's row in `TRACKER.md` (the grid — newest day on top, add a
   row if the date isn't there). Fill Exercise, Food, ~kcal, Alcohol,
   Work / Study, and Goals hit.
   - Food: log exactly what they said they ate (quantities, bread type, etc.)
     — don't generalize. Note the meal (breakfast/lunch/dinner/snack) if given.
   - Alcohol: log each drink and quantity; count standard drinks and include
     their calories. Track a running weekly total (Mon–Sun) in the reply.
3. Estimate calories for food items when not given; mark them with `~`.
   Sum a daily total.
4. Compare the day against `GOALS.md`:
   - Note whether they hit their calorie target and moved their body.
   - Track streaks (consecutive days hitting targets).
5. Reply to the user with:
   - A short recap of the day + running totals/streaks
   - Honest feedback — encouraging when on track, candid when slipping
   - A reminder of their "why" from GOALS.md when motivation seems low
6. Commit the log entry with a message like `log: 2026-11-17` and push.

Keep replies short — this is a text conversation, not a report.

Keep the `TRACKER.md` table format stable (Date | Exercise | Food | ~kcal |
Work / Study | Goals hit, newest first) — the GitHub Pages site parses it
directly, so it must stay machine-readable.
