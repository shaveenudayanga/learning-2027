# learning-2027

26 weeks of deliberate practice: Python, DSA, backend, frontend and AI engineering. No AI on the exercises.

**9 Nov 2026 to 9 May 2027** · about 10 hours a week, next to my internship and final semester.

## Why

I build with AI tools every day. This repo is the other half: rebuilding the fundamentals by hand, so I understand and can defend every line I ship.

## Rules

1. **Exercises and DSA are written by hand.** AI can explain an idea after I have tried. It does not write the solution. (See [CLAUDE.md](CLAUDE.md).)
2. **Type every example.** No copy-paste from tutorials.
3. **Push every week.** A green week beats a perfect one.
4. **Explain it in 3 lines.** Every topic ends with a short note in my own words.
5. **Stuck 40 minutes? Ask for a hint, not an answer.**

## Structure

Organised by topic, so everything about one subject is in one place. The weekly log in `journal/` shows what I did and when.

```
learning-2027/
├── python/
│   ├── 01-basics/              # each topic folder: notes.md + exercise files
│   ├── 02-functions-files-modules/
│   ├── 03-oop/
│   ├── 04-generators-decorators-context-managers/
│   ├── 05-typing-pydantic-logging/
│   ├── 06-testing-packaging-async/
│   ├── 07-internals/           # descriptors, metaclasses, dis, profiling
│   └── fluent-python/          # chapter notes and exercises
├── sql/
├── javascript/
├── typescript/
├── react/
├── nextjs/
├── ai/                         # LLM APIs, RAG, agents, evals experiments
├── cloud/
├── dsa/
│   ├── arrays-hashing/         # one file per problem: pattern + key idea at the top
│   ├── two-pointers/
│   ├── sliding-window/
│   └── ...                     # one folder per NeetCode pattern
├── cs-fundamentals/            # one note per Friday topic (os, databases, networking)
├── system-design/
├── journal/
│   ├── week-01.md              # plan, what I did, DSA log, what confused me
│   └── ...
├── CLAUDE.md                   # rules for the AI tutor in this repo
└── .claude/settings.json       # blocks AI edits to code files
```

Folders are created when I reach that topic. Projects live in their own repos and are linked below when done.

## Plan

| Weeks | Dates | Phase | Finish with |
| --- | --- | --- | --- |
| 1 to 3 | 9 to 29 Nov | Python core refresh | P1: CLI expense tracker |
| 4 to 6 | 30 Nov to 20 Dec | Python upper-intermediate | P2: Library published on PyPI |
| 7 to 9 | 21 Dec to 10 Jan | SQL, PostgreSQL, backend | P3: Task tracker API in Docker |
| 10 to 14 | 11 Jan to 14 Feb | TypeScript and React | P4: React frontend for P3 |
| 15 to 17 | 15 Feb to 7 Mar | Next.js full-stack | P5: Clinic app in Next.js + TS |
| 18 to 21 | 8 Mar to 4 Apr | AI engineering | P6: RAG assistant with evals |
| 22 to 23 | 5 to 18 Apr | Cloud + Python internals | P5 and P6 live on AWS |
| 24 to 26 | 19 Apr to 9 May | System design, interviews | Mock interviews, applications |

Every week also: 4 DSA problems, 1 CS fundamentals topic, 1 hour of Python depth reading (Fluent Python, 2nd edition).

## Progress

- [ ] Week 1: Python basics
- [ ] Week 2: functions, files, modules
- [ ] Week 3: OOP · P1
- [ ] Week 4: generators, decorators, context managers
- [ ] Week 5: type hints, Pydantic, logging
- [ ] Week 6: pytest, packaging, async · P2
- [ ] Week 7: SQL and PostgreSQL
- [ ] Week 8: FastAPI deep
- [ ] Week 9: Docker and CI · P3
- [ ] Week 10: JavaScript
- [ ] Week 11: TypeScript
- [ ] Week 12: React 1
- [ ] Week 13: React 2
- [ ] Week 14: React testing · P4
- [ ] Week 15: Next.js
- [ ] Week 16: build P5
- [ ] Week 17: test and deploy · P5
- [ ] Week 18: LLM APIs, structured output
- [ ] Week 19: RAG
- [ ] Week 20: tool calling and agents
- [ ] Week 21: evals · P6
- [ ] Week 22: AWS
- [ ] Week 23: Python internals
- [ ] Week 24: system design
- [ ] Week 25: practical rounds
- [ ] Week 26: stories and applications

**DSA solved:** 0 / 100

## Projects

| # | Project | Repo |
| --- | --- | --- |
| P1 | CLI expense tracker | coming soon |
| P2 | Sri Lankan NIC parser (PyPI) | coming soon |
| P3 | Task tracker API | coming soon |
| P4 | React frontend for P3 | coming soon |
| P5 | Clinic appointment app (Next.js + FastAPI) | coming soon |
| P6 | RAG document assistant with evals | coming soon |

## Main resources

CS50P · Python official tutorial · Fluent Python (2nd ed.) · Python behind the scenes · SQLBolt · Use The Index, Luke · FastAPI docs · javascript.info · TypeScript Handbook · react.dev · Full Stack Open · Next.js Learn · NeetCode roadmap · OSTEP · System Design Primer