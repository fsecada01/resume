# Francis Secada

Backend engineer (Python, FastAPI, Django, PostgreSQL) based in New York, NY. Ten-plus years building APIs, data pipelines, and event-driven systems for financial services, healthcare, and media. I also run a small consultancy, and I write audio software and music tooling on the side.

**Resume:** [Francis-Secada-Resume.pdf](Francis-Secada-Resume.pdf) ([Markdown source](Francis-Secada-Resume.md))
**LinkedIn:** [linkedin.com/in/francissecada](https://www.linkedin.com/in/francissecada)

This repository holds the public copy of my resume. It leaves out my address, phone, and email on purpose. The sections below say where to reach me depending on what you want to talk about.

## Hiring and engineering roles

Message me on [LinkedIn](https://www.linkedin.com/in/francissecada). I am looking for senior and staff backend roles, and I work best on Python services, data-heavy systems, and regulated domains such as healthcare and finance. Code you can read is on my [GitHub profile](https://github.com/fsecada01).

Some of my recent work is in private repositories: Ouroboros, an LLM-driven Python-to-Rust optimization agent, and previz-engine, a batch image-generation harness for local ComfyUI. I cannot link them, but I am glad to walk through the design, the tests, and the numbers in an interview.

## Consulting: FJS Services Inc.

FJS Services Inc. is my consultancy. The work that fits best:

- **Performance and reliability rescue.** Slow, flaky, or overloaded services: find the actual bottleneck, fix it, and measure the result.
- **Regulated-domain engineering.** HIPAA/HITECH healthcare data and financial-services systems, where audit trails and access controls are part of the design.
- **Build and modernize.** New APIs and full-stack applications in Python, and incremental modernization of existing systems instead of a big-bang rewrite.
- **Practical AI features.** LLM features with audit logging, using whichever model suits the job: a frontier API, a self-hosted model, or a local open-weight one.

The first conversation is free. Start at [fjsservicesinc.com/contact](https://www.fjsservicesinc.com/contact).

## Music production and audio tools

I produce and mix music, and I write the tools I want to use. All three projects below are public.

| Project | What it is | Links |
|---|---|---|
| **bus_channel_strip** | A VST3 and CLAP plugin that replaces several inserts on a master or stem bus: console-style EQ, Airwindows-based compression, a passive tube EQ, a dynamic EQ with sidechain, a transformer stage, a stereo widener, and a loudness maximizer. Modules can be reordered, bypassed, and automated. Written in Rust with NIH-Plug and vizia. Builds for Windows, macOS, and Linux. | [Repository](https://github.com/fsecada01/bus_channel_strip) - [Docs and presets](https://fsecada01.github.io/bus_channel_strip/) |
| **midi-drums** | A Python system that generates drum tracks as MIDI, with genre and style presets, imitations of well-known drummers, humanization, configurable song structure, and EZDrummer 3-compatible mapping. It ships a command-line tool and Reaper integration. | [Repository](https://github.com/fsecada01/midi-drums) - [Docs](https://fsecada01.github.io/midi-drums/) |
| **reaper-scripts** | Lua scripts for REAPER covering audio restoration and first-pass mixing and mastering, distributed as a ReaPack repository. | [Repository](https://github.com/fsecada01/reaper-scripts) |

Reach out about these if you:

- have a bug report or feature request. Please open an issue on the project's repository so others can find it.
- want to use the plugin or the drum generator in your own workflow and have questions about setup.
- are working on something similar and want to compare notes or collaborate.

For anything that does not fit an issue, use the contact form on [francissecada.com/contact](https://francissecada.com/contact).

## Open-source Python libraries

- [TextSpitter](https://github.com/fsecada01/TextSpitter) ([PyPI](https://pypi.org/project/TextSpitter/)): text extraction from PDF, DOCX, CSV, and source-code files, with a Rust core.
- [SQLModel CRUD Utilities](https://github.com/fsecada01/SQLModel-CRUD-Utilities) ([PyPI](https://pypi.org/project/sqlmodel-crud-utilities/)): sync and async CRUD helpers for SQLModel and SQLAlchemy.
