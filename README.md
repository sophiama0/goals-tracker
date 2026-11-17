# Goals Tracker

A personal accountability repo. I text my agent from my phone with what I did
today and what I ate — it logs it here, tracks it against my goals, and keeps
me disciplined and motivated.

## How it works

1. I text the agent: "ran 3 miles, ate chicken burrito + a cookie"
2. The agent appends an entry to `logs/YYYY-MM-DD.md`, estimating calories
   when needed
3. It checks progress against `GOALS.md` and replies with a recap, streaks,
   and encouragement

(Texting integration: Slack — I message `@Devin` in a dedicated channel from
my phone; it starts a session, updates this repo, and replies in-thread.)

## Structure

- `TRACKER.md` — the grid: one row per day (exercise, food, kcal, work/study)
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
| Item | Calories |
|------|----------|
| Chicken burrito | ~650 |
| Cookie | ~150 |
| **Total** | **~800** |

## Notes
- Felt good, kept streak alive
```
