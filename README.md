# Goals Tracker

A personal accountability repo. This is a Slack integration with Devin and it logs it here, tracks it against my goals, and keeps
me disciplined and motivated.

## How it works

1. Integrate Slack with Devin and text the agent what you ate today. Text it any exercise and alcohol drank and also what you did to be productive.
2. The agent appends an entry to `logs/YYYY-MM-DD.md`, estimating calories
   when needed.
3. It checks progress against `GOALS.md` and replies with a recap, streaks,
   and encouragement.
4. It will notify you to log your day if you don't respond by 6PM.

(Texting integration: Slack — I message `@Devin` in a dedicated channel from
my phone; it starts a session, updates this repo, and replies in-thread.)

## See it live

**https://sophiama0.github.io/goals-tracker/** — dashboard that reads this
repo's data (grid, streak, heatmap, goals). Updates on every agent commit.

## Structure

- `TRACKER.md` — the grid: one row per day (exercise, food, kcal, alcohol, work/study)
- `GOALS.md` — my current goals and targets
- `logs/` — one markdown file per day, in `YYYY-MM-DD` format
- `AGENTS.md` — instructions for the agent that processes my texts

## Example daily log

See `logs/` for real entries. Format:

```markdown
# 2026-11-17

## Activity
- Ran 3 miles (~300 kcal)

## Food
| Meal | Item | Calories |
|------|------|----------|
| Lunch | Chicken burrito | ~650 |
| Snack | Cookie | ~150 |
| | **Total** | **~800** |

## Alcohol
- 2 glasses red wine — 2 drinks (~250 kcal)
- Week to date: 2 drinks

## Work / Study
- Finished all assignments

## Notes
- Felt good, kept streak alive
```
