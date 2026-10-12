# Learning Coach

A Claude skill that turns Claude into an adaptive learning coach for any subject. Instead of just explaining things, it gets you to **produce**: recall, predict, explain in your own words, and attempt the real task. That's what actually builds memory. It picks the right coaching role for the moment automatically, so you just say what you want to learn.

> Framework credit: **Nick Saraev**, from his video *"How to Learn Hard Things 99x Faster with AI"*. Check out his channel: [youtube.com/@nicksaraev](https://www.youtube.com/@nicksaraev)

## What it does

The coach switches between ten roles based on what you need right now:

| Role | When it shows up |
|---|---|
| **Interviewer** | You're starting something new and your goal or level isn't clear yet |
| **Mapmaker** | The subject feels shapeless and you need a route through it |
| **Explainer** | You tried and got stuck on one specific point |
| **Socratic Questioner** | You think you understand, and it checks how deep that goes |
| **Examiner** | "Quiz me", or the end of a module: questions get harder until you hit your edge |
| **Checker** | You share code, a proof, an essay or a calculation, and it reviews the process without rewriting it |
| **Listener** | You explain a topic back, and it grades you against the source |
| **Diagnostician** | You keep making the same kind of mistake, and it finds the shared cause |
| **Sparring Partner** | You're preparing for an interview, pitch, talk or timed exam, and it runs realistic practice |
| **Clerk** | It organizes your notes and makes flashcards and a review schedule |

It also:

- makes you try before it explains, and redo things without help afterwards
- asks one question at a time and adjusts difficulty to stay at the edge of your ability
- won't agree with half-right answers or make up sources
- suggests 2–3 concrete next steps at natural breakpoints
- offers spaced-repetition review schedules fitted to your deadline, and sets up reminders if your Claude setup supports scheduled tasks
- just answers when you only want the answer

You can always steer it yourself, for example "just explain it", "quiz me" or "be the interviewer".

## Install

**Claude apps (claude.ai, desktop, mobile):** download [`learning-coach.skill`](learning-coach.skill) and upload it in your skills settings on claude.ai. Skills enabled on your account also sync to Claude Code when you sign in with that account.

**Claude Code (local only):** copy the `learning-coach` folder into `~/.claude/skills/`. You'll end up with `~/.claude/skills/learning-coach/SKILL.md`.

## Try it

- "I want to learn statistics"
- "I have a Python coding interview in 3 weeks, timed LeetCode-style, I know the basics"
- "Quiz me on photosynthesis, I have a test on Friday"
- "Here's my explanation of how TCP handshakes work, did I get it? ..."
- "Turn these messy notes into flashcards"

## Files

```
learning-coach/
├── SKILL.md              # core method, role selection, next steps, scheduling
└── references/
    └── roles.md          # detailed playbook for each of the ten roles
learning-coach.skill      # packaged version for uploading
```

## License

[MIT](LICENSE). The learning framework itself is credited to Nick Saraev (see above).
