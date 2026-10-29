# DUSQ Coach Brief

A working prototype I built as a proposal for DUSQ, the sleep regulation wearable.

**Live demo:** https://samadritar.github.io/dusq-coach-brief/

## The problem

DUSQ offers a 30 day money back guarantee, and its own FAQ says the clearest sleep gains show up around week two. That leaves a short window where a user either feels the result or sends the device back.

Sleep coaching is DUSQ's strongest lever inside that window. Each user gets a long intake and weekly check ins for the first six weeks. That work grows one for one with every device sold, which gets heavy as the US rollout scales.

## What Coach Brief does

Before every call, it reads the user's recent nights and drafts the coach's prep:

- **Changed:** what moved against the user's own baseline
- **Ask:** nights worth a question, like a very late sleep onset
- **Flag:** device issues, like stimulation spiking or the patch losing contact
- **Return risk:** whether the user is on track before the refund window closes
- **Story:** a verified win the user might agree to share

Every line names the exact nights behind it. If no nights support a line, it does not appear. The coach approves the brief before anything is used.

## How it decides

- Nights 1 to 3 set each user's baseline
- Each brief reads the last seven nights
- Wakeups count as improved when they fall to 75% of baseline or lower
- Stimulation is flagged above 2x baseline (fit issue) or below 35% of baseline (lost contact)
- A story is suggested from day 10 once deep sleep is up 20% or more

## Try it

Open the demo and start with User 0412 at day 14, the improving user. Then switch to User 0587, who is slipping, and drag the day slider to watch the brief change.

## Notes

All users and nights are synthetic. Nothing here uses DUSQ data. It is a single HTML file with no dependencies beyond Google Fonts.

Built by Samadrita Roy Chowdhury · [github.com/SamadritaR](https://github.com/SamadritaR)
