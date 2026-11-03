# 6-Month Software Engineer Roadmap

9 Nov 2026 to 9 May 2027 · about 10 hours a week, next to the BooleenLab internship and the final semester.

Rebuild Python to an advanced level, add TypeScript and React for full-stack work, then AI engineering, cloud and interview prep. Each phase ends with a project and a "done when" check, and every week names exactly what to learn from. A Python depth track runs alongside, with a CPython internals track for after May.

## Weekly rhythm

About 10 hours a week: 5 on the current phase, 2.5 on DSA, 1.5 on CS fundamentals, 1 on the Python depth track. If a week is busy, cut the phase hours first and keep DSA and Python depth going.

| Slot | Hours | What |
| --- | --- | --- |
| Mon and Wed evening | 2 x 1 h | Phase work: learn from the resource listed for that week |
| Tue and Thu evening | 2 x 1.25 h | DSA: 2 problems each night |
| Friday | 1.5 h | One CS fundamentals topic from the schedule |
| Saturday | 3 h | 1 h Python depth reading, then 2 h building the week's exercise or project part |
| Sunday | 1 h | Finish, push to GitHub, write 3 lines on what you learned |

- Push something to GitHub every week. A green week is the goal, not a perfect one.
- Write what confused you and how you solved it in `journal/week-NN.md`. These notes become interview stories and LinkedIn posts.

## How to learn: the loop for every topic

1. **Read or watch (about 30% of the time).** Only the chapter or page listed. Do not open a second tutorial on the same topic.
2. **Type every example yourself.** Change one thing and predict what will happen before you run it. Use [Python Tutor](https://pythontutor.com/) to see what Python does step by step.
3. **Do the exercises without AI.** Exercism, LeetCode or the exercise at the end of the chapter.
4. **Build the week's project part.** This is where it sticks.
5. **Explain it in 3 lines in your notes,** as if to a first-year student. If you cannot, go back to step 1 for that part only.

**When stuck**

- 20 minutes stuck: re-read the exact error message, then search the error text.
- 40 minutes stuck: ask Claude for a hint (see the hint ladder in `CLAUDE.md`), not the code.
- Still stuck at the end of the day: write the question in the journal, skip it, and come back on Sunday.

## Python depth track

Main book: **Fluent Python, 2nd edition** (Luciano Ramalho, O'Reilly, 24 chapters). Paid, so check the USJ library first. If you cannot get it, the free column covers the same ideas. Read in the Saturday depth hour; weeks marked "phase" use the phase hours. Run each chapter's code from the [example repo](https://github.com/fluentpython/example-code-2e).

| Weeks | Fluent Python chapters | Free alternative or extra |
| --- | --- | --- |
| 1 to 3 | None yet: finish the basics first | Paste your week's code into [Python Tutor](https://pythontutor.com/) and watch it run |
| 4 (phase) | 1 The Python Data Model, 9 Decorators and Closures | [Data model reference](https://docs.python.org/3/reference/datamodel.html), sections 3.1 to 3.3 |
| 5 (phase) | 8 Type Hints in Functions, 5 Data Class Builders | [mypy cheat sheet](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html) |
| 6 (phase) | 13 Interfaces, Protocols, and ABCs | [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/) |
| 7 to 9 | 2 An Array of Sequences, 3 Dictionaries and Sets | [How Python dictionaries work](https://tenthousandmeters.com/blog/python-behind-the-scenes-10-how-python-dictionaries-work/) |
| 10 to 11 | 6 Object References, Mutability, and Recycling | [How variables are implemented in CPython](https://tenthousandmeters.com/blog/python-behind-the-scenes-5-how-variables-are-implemented-in-cpython/) |
| 12 to 14 | 7 Functions as First-Class Objects, 10 Design Patterns with First-Class Functions | Real Python articles on closures and first-class functions |
| 15 to 17 | 11 A Pythonic Object, 12 Special Methods for Sequences | [How the object system works](https://tenthousandmeters.com/blog/python-behind-the-scenes-6-how-python-object-system-works/), [How attributes work](https://tenthousandmeters.com/blog/python-behind-the-scenes-7-how-python-attributes-work/) |
| 18 to 19 | 14 Inheritance, 16 Operator Overloading | Data model reference, section 3.3.8 onwards |
| 20 to 21 | 17 Iterators, Generators, and Classic Coroutines, 18 with, match, and else Blocks, 19 Concurrency Models | [How the CPython VM works](https://tenthousandmeters.com/blog/python-behind-the-scenes-1-how-the-cpython-vm-works/) |
| 22 | 20 Concurrent Executors, 21 Asynchronous Programming | [How async/await works](https://tenthousandmeters.com/blog/python-behind-the-scenes-12-how-asyncawait-works-in-python/), [The GIL](https://tenthousandmeters.com/blog/python-behind-the-scenes-13-the-gil-and-its-effects-on-python-multithreading/) |
| 23 (phase) | 22 Dynamic Attributes and Properties, 23 Attribute Descriptors, 24 Class Metaprogramming | [Descriptor HowTo Guide](https://docs.python.org/3/howto/descriptor.html), [How bytecode is executed](https://tenthousandmeters.com/blog/python-behind-the-scenes-4-how-python-bytecode-is-executed/), [How the import system works](https://tenthousandmeters.com/blog/python-behind-the-scenes-11-how-the-python-import-system-works/) |
| 24 to 26 | 15 More About Type Hints, 4 Unicode Text versus Bytes, then reread 1 | [How the compiler works](https://tenthousandmeters.com/blog/python-behind-the-scenes-2-how-the-cpython-compiler-works/) (optional) |

**Done when (May):** you can explain, without notes, what happens when Python runs `obj.attr`, why a dict lookup is fast, what a decorator really returns, and why threads do not speed up CPU work in normal CPython.

## Phase 1: Python core refresh (weeks 1 to 3, 9 to 29 Nov)

Goal: write normal Python again without looking things up every line. Folder: `python/01-basics/` to `python/03-oop/`. Main resources: [CS50P](https://cs50.harvard.edu/python/), the [official Python tutorial](https://docs.python.org/3/tutorial/) and the [Exercism Python track](https://exercism.org/tracks/python).

**Week 1: basics, fast**

- Variables, types, strings and f-strings, `if`, loops, `range`, `enumerate`, `zip`
- Lists, tuples, dicts, sets: when to use each, and their time cost (list lookup O(n), dict and set O(1))
- Slicing, unpacking, `in`, `sorted` with `key=`
- **Learn from:** CS50P lectures 0, 1 and 2 at 1.5x speed. Python tutorial chapters 3 and 5.
- **Practise:** CS50P problem sets 0 to 2, plus 5 Exercism easy exercises.

**Week 2: functions and structure**

- Functions: default args, `*args`, `**kwargs`, keyword-only args, return values
- Comprehensions (list, dict, set) and when a plain loop is clearer
- Exceptions: `try/except/else/finally`, raising your own errors
- Files with `with open`, `pathlib`, reading JSON and CSV
- Modules, packages, `if __name__ == "__main__"`, virtual environments with `venv` or `uv`
- **Learn from:** CS50P lectures 3, 4 and 6. Python tutorial chapters 4, 6, 7 and 8.
- **Practise:** CS50P problem sets 3, 4 and 6.

**Week 3: OOP**

- Classes, `__init__`, instance vs class attributes, methods, `@property`
- Inheritance vs composition, `super()`
- Dunder methods: `__repr__`, `__eq__`, `__len__`, `__iter__`
- `@dataclass`
- **Learn from:** CS50P lecture 8. Python tutorial chapter 9.
- **Practise:** CS50P problem set 8, then build Project 1.

**Project 1:** a command-line expense tracker. Add, list and summarise expenses, saved to a JSON file, with `argparse`. About 200 lines.

**Done when:** you can solve Exercism Python "easy" exercises without help, and explain the difference between a list and a dict lookup.

## Phase 2: Python upper-intermediate (weeks 4 to 6, 30 Nov to 20 Dec)

Goal: write Python the way a professional library does: typed, tested, packaged and published.

**Week 4: the Pythonic toolkit**

- Iterators and generators, `yield`, generator expressions, `itertools`
- Decorators (with and without arguments), `functools.wraps`, `lru_cache`
- Context managers: `with`, writing your own with `contextlib`
- `collections`: `Counter`, `defaultdict`, `deque`
- **Learn from:** Fluent Python chapters 1 and 9. Python docs for [`itertools`](https://docs.python.org/3/library/itertools.html), [`functools`](https://docs.python.org/3/library/functools.html), [`contextlib`](https://docs.python.org/3/library/contextlib.html) and [`collections`](https://docs.python.org/3/library/collections.html).
- **Practise:** write a `@retry(times=3)` decorator, a generator that reads a big file line by line, and a `timer()` context manager. Test all three.

**Week 5: types and data**

- Type hints: `list[int]`, `Optional`, `Union`, `TypedDict`, generics, `Protocol`
- Run `mypy --strict` on your code and fix what it finds
- Pydantic models and validation (FastAPI is built on it)
- `logging` instead of `print`
- **Learn from:** Fluent Python chapters 8 and 5. [mypy cheat sheet](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html). [Pydantic docs: Models](https://docs.pydantic.dev/latest/concepts/models/). [Logging HOWTO](https://docs.python.org/3/howto/logging.html).
- **Practise:** add full type hints to Project 1 until `mypy --strict` passes.

**Week 6: testing, packaging and async basics**

- pytest: fixtures, `parametrize`, `monkeypatch`, mocking with `unittest.mock`, coverage
- Project layout with `pyproject.toml`, `ruff` for linting and formatting, semantic versioning
- `async` and `await` basics: event loop, `asyncio.gather`, why FastAPI uses it
- **Learn from:** Fluent Python chapter 13. [pytest: Get started](https://docs.pytest.org/en/stable/getting-started.html), then its "How to use fixtures" and "How to parametrize" pages. [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/). Real Python "Async IO in Python: A Complete Walkthrough".
- **Practise:** build Project 2.

**Project 2: a real library on PyPI.** A Sri Lankan NIC number parser: accept the old (9 digits + V or X) and new (12 digits) formats, validate them, and return birth date and gender. Typed, documented, 90% test coverage, `ruff` and `mypy` clean, GitHub Actions running tests on Python 3.11 to 3.13, published first to TestPyPI and then to PyPI. Check the package name is free before you start.

**Done when:** someone can `pip install` your library, you can write a decorator and a generator from memory, and you can explain what `async` gives you and what it does not.

## Phase 3: SQL, PostgreSQL and backend (weeks 7 to 9, 21 Dec to 10 Jan)

Goal: build a real backend service you could hand to a team.

**Week 7: SQL properly**

- `SELECT`, `JOIN` types, `GROUP BY`, `HAVING`, subqueries, window functions (`ROW_NUMBER`, `RANK`)
- Schema design: primary and foreign keys, normalisation to 3NF, when to denormalise
- Indexes: B-tree basics, reading `EXPLAIN ANALYZE`
- Transactions and isolation levels (read committed vs serializable)
- **Learn from:** [SQLBolt](https://sqlbolt.com/) (all lessons, one evening). [PostgreSQL tutorial: window functions](https://www.postgresql.org/docs/current/tutorial-window.html). [Use The Index, Luke](https://use-the-index-luke.com/), chapters 1 and 2. [PostgreSQL docs: transaction isolation](https://www.postgresql.org/docs/current/transaction-iso.html).
- **Practise:** [PostgreSQL Exercises](https://pgexercises.com/): Basic, Joins and Aggregates sections. Run PostgreSQL in Docker.

**Week 8: FastAPI deep**

- Routers, dependency injection, Pydantic request and response models, error handling
- SQLAlchemy 2.0 or SQLModel with PostgreSQL, Alembic migrations
- Auth: password hashing, JWT access and refresh tokens, role checks
- Pagination, filtering, background tasks
- **Learn from:** [FastAPI Tutorial - User Guide](https://fastapi.tiangolo.com/tutorial/), especially "Bigger Applications", "SQL (Relational) Databases" and the Security pages (OAuth2 with JWT). [SQLAlchemy 2.0 Unified Tutorial](https://docs.sqlalchemy.org/en/20/tutorial/). [Alembic tutorial](https://alembic.sqlalchemy.org/en/latest/tutorial.html).
- **Practise:** start Project 3: models, migrations and auth first.

**Week 9: ship it**

- Docker and Docker Compose (API + Postgres)
- Integration tests against a real test database
- GitHub Actions: lint, type check, test, build image
- REST design: status codes, idempotency, versioning
- **Learn from:** [Docker: Get started](https://docs.docker.com/get-started/). [FastAPI: Testing](https://fastapi.tiangolo.com/tutorial/testing/). [GitHub Actions: Building and testing Python](https://docs.github.com/en/actions/use-cases-and-examples/building-and-testing/building-and-testing-python). [Zalando RESTful API Guidelines](https://opensource.zalando.com/restful-api-guidelines/) (skim the MUST rules).
- **Practise:** finish Project 3.

**Project 3:** a task tracker API (users, projects, tasks, comments) with auth, migrations, tests and Docker. README with a diagram and setup in 3 commands.

**Done when:** you can design a schema for a new idea on paper, explain why a query is slow, and run the whole service with `docker compose up`.

## Phase 4: TypeScript and React (weeks 10 to 14, 11 Jan to 14 Feb)

Goal: build a working frontend on your own. Learn React first; Next.js comes after. Main resources: [javascript.info](https://javascript.info/), the [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html), [react.dev Learn](https://react.dev/learn) and [Full Stack Open](https://fullstackopen.com/en/).

**Week 10: JavaScript you actually need**

- `let`/`const`, arrow functions, destructuring, spread, modules
- Arrays: `map`, `filter`, `reduce`, `find`
- Promises, `async`/`await`, `fetch`, the event loop
- **Learn from:** javascript.info sections "JavaScript Fundamentals", "Objects: the basics", "Data types" (arrays, destructuring), "Promises, async/await" and "Modules". Skip the rest.
- **Practise:** rewrite 5 of your old DSA solutions in JavaScript.

**Week 11: TypeScript**

- Types, interfaces, unions, narrowing, generics, utility types (`Partial`, `Pick`, `Omit`)
- `strict` mode on from day one
- Typing API responses (same idea as Pydantic models)
- **Learn from:** TypeScript Handbook pages "The Basics", "Everyday Types", "Narrowing", "More on Functions", "Object Types", "Generics" and the "Utility Types" reference. Full Stack Open part 9.
- **Practise:** write typed functions that call your Project 3 API and parse its responses.

**Weeks 12 to 13: React**

- Components, props, state with `useState`, `useEffect` and when not to use it
- Lists and keys, forms, controlled inputs, lifting state up
- Fetching data with TanStack Query, loading and error states
- Routing with React Router, basic CSS with Tailwind
- **Learn from:** react.dev Learn: "Describing the UI", "Adding Interactivity", "Managing State" and "Escape Hatches" (read "You Might Not Need an Effect" twice). Full Stack Open parts 1 and 2. [TanStack Query](https://tanstack.com/query/latest) quick start.
- **Practise:** start Project 4.

**Week 14: React testing and polish**

- Vitest and React Testing Library
- Accessibility basics: labels, keyboard use, contrast
- **Learn from:** Full Stack Open part 5 (testing React apps). [Testing Library: React](https://testing-library.com/docs/react-testing-library/intro/). [web.dev Learn Accessibility](https://web.dev/learn/accessibility).
- **Practise:** finish Project 4 with tests.

**Project 4:** a React + TypeScript frontend for your Project 3 API: login, list, create, edit tasks.

**Done when:** you can build a form with validation and an API call from a blank file, and explain why a component re-rendered.

## Phase 5: Next.js full-stack project (weeks 15 to 17, 15 Feb to 7 Mar)

Goal: one polished full-stack app. Upgrade the clinic appointment app instead of starting something new.

**Week 15: learn Next.js**

- App Router: server vs client components, layouts, route handlers, server actions
- Data fetching and caching, environment variables
- **Learn from:** the free [Next.js Learn course](https://nextjs.org/learn) (App Router dashboard course, all chapters). [Next.js docs: Getting Started](https://nextjs.org/docs/app/getting-started).

**Week 16: build**

- Rebuild the clinic app pages in Next.js + TypeScript (`strict`), calling the FastAPI backend
- Auth with sessions or JWT from your FastAPI backend
- **Learn from:** your Project 4 code and the Next.js docs pages for whatever you are building that day.

**Week 17: test, deploy, show**

- Playwright end-to-end tests for the main flows, running in CI
- Deploy the frontend on Vercel and the backend on a container host
- Record a new 2-minute demo video
- **Learn from:** [Playwright docs: Writing tests](https://playwright.dev/docs/writing-tests). [Vercel: deploying Next.js](https://vercel.com/docs/frameworks/nextjs).

**Project 5 (flagship):** the clinic app frontend rebuilt in Next.js + TypeScript, connected to the FastAPI backend, with Playwright tests in CI, live on the web, and a demo video in the README.

**Done when:** a stranger can open the live link and book an appointment, and you can explain every layer from the button click to the database row.

## Phase 6: AI engineering (weeks 18 to 21, 8 Mar to 4 Apr)

Goal: build AI features that are tested and trustworthy, not demos.

**Week 18: LLM API basics done well**

- Calling Gemini or Claude APIs from Python, streaming, retries, timeouts, cost and token limits
- Structured output: make the model return JSON that a Pydantic model validates
- Prompt design: system prompts, examples, asking instead of guessing
- **Learn from:** [Gemini API docs](https://ai.google.dev/gemini-api/docs) (text generation and structured output pages). [Claude prompt engineering guide](https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview).
- **Practise:** a script that turns a messy email into a validated Pydantic object, with tests for 10 sample emails.

**Week 19: RAG**

- Embeddings, chunking, vector search with pgvector in PostgreSQL
- Retrieval quality: hybrid search, re-ranking, citing the source chunk
- **Learn from:** [pgvector README](https://github.com/pgvector/pgvector). [Anthropic: Contextual Retrieval](https://www.anthropic.com/news/contextual-retrieval).
- **Practise:** start Project 6: load documents, chunk, embed, search.

**Week 20: tool calling and agents**

- Tool calling, simple agent loops, when a fixed workflow beats an agent
- Guardrails: input checks, output validation, human approval for risky actions
- **Learn from:** [Building effective agents (Anthropic)](https://www.anthropic.com/research/building-effective-agents). [Claude docs: tool use](https://docs.claude.com/en/docs/agents-and-tools/tool-use/overview). [Hugging Face Agents Course](https://huggingface.co/learn/agents-course) (units 1 and 2).
- **Practise:** add 1 or 2 tools to Project 6.

**Week 21: evals**

- A test set of 30 to 50 questions with expected answers
- Automatic scoring in pytest, tracking scores when you change a prompt or model
- **Learn from:** [Hamel Husain: Your AI Product Needs Evals](https://hamel.dev/blog/posts/evals/).
- **Practise:** finish Project 6 with an eval suite in CI.

**Project 6:** a document Q&A assistant with RAG, citations, one or two tools, an eval suite in CI and a short write-up of what failed and how you fixed it.

**Done when:** you can show a number that proves your change made the AI better, not just a screenshot.

## Phase 7: Cloud, deployment and Python internals (weeks 22 to 23, 5 to 18 Apr)

**Week 22: AWS and operations**

- AWS free tier: EC2 or ECS, RDS for PostgreSQL, S3, IAM users and roles (never use the root account)
- Secrets in environment variables or AWS Secrets Manager, never in Git
- Logs, health checks, basic monitoring and alerts
- CI/CD: GitHub Actions builds and deploys on merge to `main`
- **Learn from:** [AWS Skill Builder](https://skillbuilder.aws/): the free "AWS Cloud Practitioner Essentials" course (compute, database, storage and security modules). The AWS getting-started guide for each service you use.
- **Practise:** deploy Projects 5 and 6. Set a billing alarm first.

**Week 23: Python internals**

- Concurrency: the GIL, threads vs processes vs `asyncio`, when each is right
- Bytecode: use `dis` to see what your functions compile to
- The data model: descriptors, `__slots__`, how `@property` works, metaclasses and `__init_subclass__`
- Profiling with `cProfile` and fixing a slow function
- **Learn from:** Fluent Python chapters 22, 23 and 24. [Descriptor HowTo Guide](https://docs.python.org/3/howto/descriptor.html). Python docs for [`dis`](https://docs.python.org/3/library/dis.html) and [the profilers](https://docs.python.org/3/library/profile.html).
- **Practise:** build a tiny "mini-Pydantic": a `Model` base class where typed fields are validated by descriptors. Then profile one slow part of Project 3 and make it faster.

**Done when:** both projects run on AWS with CI/CD, you can explain why an I/O-heavy API uses `asyncio` but CPU-heavy work needs processes, and how your mini-Pydantic validates a field.

## Phase 8: System design and interview prep (weeks 24 to 26, 19 Apr to 9 May)

**Week 24: system design basics**

- Load balancers, caching (Redis), queues, database replicas and sharding, CDNs, rate limiting
- Practise 3 classic designs out loud: URL shortener, chat app, notification system
- Design your own projects on one page each: what breaks at 10x users?
- **Learn from:** [System Design Primer](https://github.com/donnemartin/system-design-primer): "System design topics: start here", then its URL shortener (Pastebin/Bit.ly) solution. The free ByteByteGo videos on YouTube for anything still unclear.

**Week 25: practical rounds**

- Timed practical tasks: extend an API, debug unfamiliar code, parse and validate data
- Review AI-generated code for bugs under time pressure
- 2 mock DSA interviews with a friend, or recorded alone with a 45-minute timer
- **Practise:** take an open-source Python repo you have never seen, pick a "good first issue", and fix it in 90 minutes.

**Week 26: stories and applications**

- 6 STAR stories from your projects, BooleenLab and university (a bug you fixed, a disagreement, a deadline, a failure)
- Update resume, LinkedIn and GitHub READMEs with Projects 2 to 6
- Apply to 10 to 15 roles with tailored resumes
- **Learn from:** [Tech Interview Handbook](https://www.techinterviewhandbook.org/): the behavioural interview pages.

**Done when:** you can explain any project for 10 minutes and answer "why did you choose X over Y" for every major choice.

## All 26 weeks: DSA and CS fundamentals

About 4 DSA problems a week, roughly 100 by May, mostly Easy and Medium. Solve them in Python. Follow the [NeetCode roadmap](https://neetcode.io/roadmap) order. Save each in `dsa/<pattern>/`.

| Weeks | DSA pattern | Problems | CS fundamentals (one Friday topic each week) |
| --- | --- | --- | --- |
| 1 to 3 | Arrays and hashing | 12 Easy | Stack vs heap memory, Big-O, processes vs threads |
| 4 to 5 | Two pointers, sliding window | 8 | CPU scheduling, race conditions, locks, deadlock |
| 6 to 7 | Stack, binary search | 8 | Virtual memory and paging, file systems and I/O |
| 8 to 9 | Linked lists | 8 | DB indexes, transactions, ACID, isolation levels |
| 10 to 12 | Trees (DFS, BFS, BST) | 12 | SQL vs NoSQL, TCP/IP layers, TCP vs UDP |
| 13 to 14 | Heaps, intervals | 8 | DNS and "what happens when you type a URL", HTTP and TLS |
| 15 to 17 | Graphs (BFS, DFS, topological sort, union-find) | 12 | REST vs gRPC vs WebSockets, sessions vs JWT vs OAuth2, OWASP Top 10 |
| 18 to 19 | Backtracking | 8 | Caching layers, message queues |
| 20 to 22 | Dynamic programming (1D, then 2D) | 12 | CAP and consistency, Git internals, Linux processes and permissions |
| 23 | Greedy | 4 | Containers: namespaces and cgroups |
| 24 to 26 | Mixed timed review, 45 min per problem | 10 | Review your Friday notes |

CS fundamentals resources: [OSTEP](https://pages.cs.wisc.edu/~remzi/OSTEP/) (operating systems), [High Performance Browser Networking](https://hpbn.co/) (networking), [Use The Index, Luke](https://use-the-index-luke.com/) (databases), [The Missing Semester](https://missing.csail.mit.edu/) (Git, shell, Linux).

- After each problem, write the pattern name and the one idea that cracked it at the top of the file. Re-solve any problem you could not do 2 weeks later.
- Stuck for more than 30 minutes: read the solution, close it, write it again from memory the next day.
- Big tech still tests DSA heavily. Many startups and remote companies use practical rounds instead, so do not grind Hard problems.

## Rules for learning with Claude Code

1. **Exercises and DSA: no AI code.** Claude explains and hints only (see `CLAUDE.md`).
2. **Projects (in their own repos): Claude Code can write most of the code, but you write the spec, the tests and the review.** You must be able to explain every file.
3. **Rebuild one small part of each project by hand** (for example, the auth flow or one React page).
4. **Read every diff before you accept it.** If you cannot explain a line, ask why, then decide.
5. **Keep applying the whole time.** Each finished project goes on the resume and LinkedIn that week.
6. **If you fall behind, skip forward, do not stop.** Mark the skipped topic and come back in the Phase 8 review weeks.

## After May: CPython internals track (about 12 weeks)

| Weeks | Topic | Learn from | Build |
| --- | --- | --- | --- |
| 1 to 2 | Build CPython from source, run its tests, find your way around the repo | [Python Developer's Guide](https://devguide.python.org/), the `InternalDocs` folder in the [CPython repo](https://github.com/python/cpython) | A Python build from `main` |
| 3 to 4 | Compiler and VM: parser, AST, bytecode, the evaluation loop | [How the CPython compiler works](https://tenthousandmeters.com/blog/python-behind-the-scenes-2-how-the-cpython-compiler-works/), [Stepping through the CPython source](https://tenthousandmeters.com/blog/python-behind-the-scenes-3-stepping-through-the-cpython-source-code/). Optional paid book: CPython Internals (Anthony Shaw) | Step through `a + b` in a debugger |
| 5 to 6 | Objects and memory: `PyObject`, reference counting, the GC, ints, strings | [How integers work](https://tenthousandmeters.com/blog/python-behind-the-scenes-8-how-python-integers-work/), [How strings work](https://tenthousandmeters.com/blog/python-behind-the-scenes-9-how-python-strings-work/) | Notes: the life of one object |
| 7 to 8 | C extensions | [Extending and Embedding the Python Interpreter](https://docs.python.org/3/extending/) | A C extension for one hot function, benchmarked |
| 9 to 10 | Rust extensions | [PyO3 user guide](https://pyo3.rs/), [maturin](https://www.maturin.rs/) | Rewrite the NIC parser's core in Rust, ship wheels |
| 11 to 12 | Free-threaded Python and contributing | [Python support for free threading](https://docs.python.org/3/howto/free-threading-python.html), the devguide's contributing pages | One merged pull request in CPython, FastAPI or Pydantic |
