# C11 · Crunch Arcade — Game Development

> A free, open-source **12-week game-development track** for engineers (mostly Python users) who want to ship a small game they're proud of. From the game-loop primitives in pure Pygame to a polished 2D Godot game with sound, save states, and a deploy you can share with friends.

[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](LICENSE)
[![Python · Pygame · Godot](https://img.shields.io/badge/stack-Python_·_Pygame_·_Godot-DB2777.svg)](#stack)
[![Built in the open](https://img.shields.io/badge/built-in%20the%20open-DB2777.svg)](https://github.com/CODE-CRUNCH-CLUB)

C11 is **dedicated game-dev**. It used to share a code with C# Foundations; that course is now [C9 · Crunch Sharp](../C9-CRUNCH-SHARP/). C11 focuses on 2D indie game development with Python (Pygame) for the fundamentals and Godot 4 (GDScript) for the polished capstone.

We don't teach Unity here. Unity is excellent and lives under [C9 · Crunch Sharp](../C9-CRUNCH-SHARP/) where the C# ecosystem belongs. Choose the right one for your career goal.

---

## Pathway summary

- **Full-time:** 12 weeks · ~36 hrs/week · ~432 hours
- **Working-engineer pace:** 6 months · ~18 hrs/week
- **Evening / undergraduate pace:** 1 year · ~9 hrs/week

See [`SYLLABUS.md`](SYLLABUS.md).

---

## Standards & equivalency

> C11 stands in for a university's game design and development course, and for the used-not-derived half of its computer graphics course.

**University equivalent.** Two of them. **Game Design and Development** — `CAP 4053`, `CS 4455`, `CMS.611J`. Coverage: **full**. **Computer Graphics** — `CAP 4720`, `CS 4300`, `CS 148`. Coverage: **partial**.

Partial has a precise meaning against the graphics claim, and it is not "most of it". C11 teaches the pipeline *used* rather than *derived*. The learner moves sprites, tilemaps, cameras, animation curves, particles and post-process passes through a real engine, writes fragment shaders against real texture coordinates, and can say what each stage of the pipeline consumes and produces — but is never asked to derive the transform chain in homogeneous coordinates, to implement a rasteriser, or to compute a surface's colour from a light and a normal. Those are the four rows marked `lighter` below, and they are declared again at the end of this section. Against Game Design and Development there is no such reservation: every outcome is taught and assessed.

C11 carries no credit, no transcript entry, no accreditation and no proctored exam. The equivalence is one of **content and skill**: the outcomes below are taught here at the same depth or deeper except where a row says otherwise, and every one of them is assessed. What a registrar records is not something an open repository can give you.

| University outcome | Where this course teaches it | Depth |
| --- | --- | --- |
| **Game Design and Development** — implement the real-time loop of a game (input, update, render) and make motion independent of frame rate | [Week 01](curriculum/week-01-the-game-loop/) | deeper |
| **Game Design and Development** — detect collisions between moving bodies, resolve them, and integrate simple physics over time | [Week 02](curriculum/week-02-collisions-and-physics-lite/) | same |
| **Game Design and Development** — analyse and critique a design in the field's vocabulary: mechanics, dynamics, aesthetics, game feel | [Week 03](curriculum/week-03-game-design-vocabulary/) | same |
| **Game Design and Development** — playtest a build with real players and turn what you observe into changes you can defend | [Week 03](curriculum/week-03-game-design-vocabulary/) | same |
| **Game Design and Development** — represent levels as data, author them in an external editor, load them at run time, and drive a camera over a world larger than the screen | [Week 04](curriculum/week-04-tilemaps-and-levels/) | same |
| **Game Design and Development** — model character and enemy behaviour with finite state machines, including hierarchy and a state stack | [Week 05](curriculum/week-05-state-machines/) | deeper |
| **Game Design and Development** — animate a character and bind its presentation to its game state | [Week 06](curriculum/week-06-animation-and-juice/) | deeper |
| **Game Design and Development** — persist and restore game state across sessions | [Week 07](curriculum/week-07-save-and-load-systems/) | deeper |
| **Game Design and Development** — build and balance a game's audio: effects, music, and the mix that holds them together | [Week 08](curriculum/week-08-sound-and-music-systems/) | deeper |
| **Game Design and Development** — reason about networked play: the models, the transport, the latency budget, and the techniques that hide it | [Week 09](curriculum/week-09-multiplayer-fundamentals/) | same |
| **Game Design and Development** — produce visual effects with an engine's material and particle systems | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | same |
| **Game Design and Development** — build a project in a contemporary engine, using its nodes, scenes and scripting language | [Week 10](curriculum/week-10-shaders-and-visual-effects/) — Godot 4 from Week 09 onward | same |
| **Game Design and Development** — design a save format that survives shipping: versioning, validation, integrity, recovery | [Week 11](curriculum/week-11-save-systems-and-serialization/) | deeper |
| **Game Design and Development** — scope, produce and ship a complete playable build, and defend the scope decisions that got it there | [Week 12](curriculum/week-12-capstone-ship-a-complete-game/) | deeper |
| **Computer Graphics** — name the stages of the rendering pipeline and state what each one consumes and produces | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | same |
| **Computer Graphics** — texturing: sample an image with texture coordinates, and build sprite sheets, tilesets and look-up tables | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | same |
| **Computer Graphics** — colour, the alpha channel, and the blend stage that composites a fragment onto what is already in the framebuffer | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | same |
| **Computer Graphics** — render to an off-screen target and run a full-screen post-process pass over the result | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | same |
| **Computer Graphics** — scene representation: a hierarchy of objects, a camera, a viewport, and the transform between world and screen space | [Week 04](curriculum/week-04-tilemaps-and-levels/) | same |
| **Computer Graphics** — interpolation and parametric curves driving motion over time | [Week 06](curriculum/week-06-animation-and-juice/) | deeper |
| **Computer Graphics** — particle systems: emission, per-particle integration, and life-cycle over time | [Week 06](curriculum/week-06-animation-and-juice/) | deeper |
| **Computer Graphics** — write shader programs that run on the GPU, using uniforms, samplers and interpolated coordinates | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | lighter |
| **Computer Graphics** — transform geometry between object, world, view and screen space using matrices in homogeneous coordinates | [Week 04](curriculum/week-04-tilemaps-and-levels/) | lighter |
| **Computer Graphics** — rasterisation: turn geometry into fragments, with the sampling and coverage rules that implies | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | lighter |
| **Computer Graphics** — shading and lighting models: compute a surface's colour from a light, a material and a surface normal | [Week 10](curriculum/week-10-shaders-and-visual-effects/) | lighter |

The four `lighter` rows are the graphics gaps and nothing else. On the first, C11 writes real shader programs — Godot canvas-item fragment shaders with uniforms, samplers, `UV` and `TIME` — but no vertex shaders, no code written against a graphics API from first principles, and no lighting. On the second, C11 transforms between world and screen space with a camera offset and integer math rather than with a matrix in homogeneous coordinates. On the third and fourth it names the stage and stops there.

Every other row points at a week that **assigns work** on that outcome — an exercise, a challenge, homework, a quiz item or the week's mini-project — not merely a week that mentions it.

**The industry bar.** What an employer expects of somebody paid to build games, and where this course makes the learner do it. Two rows below say the course does not clear the bar; they say so rather than dressing up something else as it.

| What the job expects | Where this course does it |
| --- | --- |
| Work lands as a commit in a repository you own, not a file on your desktop | Every challenge and mini-project is specified as a folder inside a portfolio repository, with a commit at each working milestone — [`curriculum/week-01-the-game-loop/challenges/README.md`](curriculum/week-01-the-game-loop/challenges/README.md) |
| You read code you did not write and form a judgement on it | From Week 07 the exercises are handed over as reference implementations to read, run and modify, each with a published teardown — [`curriculum/week-09-multiplayer-fundamentals/exercises/SOLUTIONS.md`](curriculum/week-09-multiplayer-fundamentals/exercises/SOLUTIONS.md) — and Week 10 takes a stranger's shader off a public library, ports it, and asks what had to change: [`curriculum/week-10-shaders-and-visual-effects/challenges/challenge-01-port-a-shadertoy.md`](curriculum/week-10-shaders-and-visual-effects/challenges/challenge-01-port-a-shadertoy.md). C11 has no written code review of a defective module with ranked findings; the judgement it asks for is a port and a critique, not a review |
| Tests exist, and the command to run them is written down | Once, in Week 11, where a `pytest` suite the learner writes is a graded deliverable run with `python3 -m pytest test_migration.py` — [`curriculum/week-11-save-systems-and-serialization/mini-project/README.md`](curriculum/week-11-save-systems-and-serialization/mini-project/README.md). C11 ships no test suite of its own. Everywhere else the gate is the artifact's acceptance-criteria checklist plus a compile pass |
| You read a real error instead of guessing | Weeks 07 to 09 quote the exception text as captured — `OSError: [Errno 48] Address already in use` — with the cause and the fix under it: [`curriculum/week-09-multiplayer-fundamentals/exercises/SOLUTIONS.md`](curriculum/week-09-multiplayer-fundamentals/exercises/SOLUTIONS.md). Weeks 10 to 12 carry `Common pitfalls` lists that name the symptom in prose instead of quoting output, and Weeks 01 to 06 carry no such section at all |
| Dependencies are isolated per project | A virtual-environment and install block at the top of every exercise index — [`curriculum/week-04-tilemaps-and-levels/exercises/README.md`](curriculum/week-04-tilemaps-and-levels/exercises/README.md) |
| A formatter, a linter, and a pipeline that runs on every push | **Not met.** C11 configures no formatter, no linter and no continuous integration, and no week puts the work through a pipeline. The nearest thing is the per-file compile check written into each exercise index, `python -m py_compile exercise-XX-name.py`. Declared as a gap at the end of this section |
| Assets are licensed, and the licence is honoured | A `CREDITS.md` naming every asset, its author and its licence, mirrored into the in-game credits and the storefront page — [`curriculum/week-12-capstone-ship-a-complete-game/lecture-notes/03-the-itch-page-the-trailer-and-the-credits.md`](curriculum/week-12-capstone-ship-a-complete-game/lecture-notes/03-the-itch-page-the-trailer-and-the-credits.md) |
| The output is portfolio-grade: a stranger can open it and see what you can do | Four platform exports and a public storefront page written for somebody who has never met you — [`curriculum/week-12-capstone-ship-a-complete-game/lecture-notes/02-export-build-and-the-four-targets.md`](curriculum/week-12-capstone-ship-a-complete-game/lecture-notes/02-export-build-and-the-four-targets.md) |
| The practice is named, not implied | The `Standards this week meets` block at the top of every week |

**Beyond both bars.** Clearing the two floors is entry, not success. Open any of these and check it in under a minute.

| What we add | Which bar it beats | Where it lives |
| --- | --- | --- |
| From Week 07 on, every exercise carries a published teardown — what it teaches, what "done" looks like, the common bugs with symptom, cause and fix, and the lines worth a second read — visible from the first day of the week rather than after a deadline | both | [`curriculum/week-08-sound-and-music-systems/exercises/SOLUTIONS.md`](curriculum/week-08-sound-and-music-systems/exercises/SOLUTIONS.md) |
| A quiz in every week from Week 01 to Week 11, with its answer key published in the same file and worked rather than lettered | university | [`curriculum/week-10-shaders-and-visual-effects/quiz.md`](curriculum/week-10-shaders-and-visual-effects/quiz.md) |
| The learner finishes holding a public game — four platform builds, a storefront page, a thirty-second trailer — rather than a grade only a registrar can see | both | [`curriculum/week-12-capstone-ship-a-complete-game/lecture-notes/03-the-itch-page-the-trailer-and-the-credits.md`](curriculum/week-12-capstone-ship-a-complete-game/lecture-notes/03-the-itch-page-the-trailer-and-the-credits.md) |
| A millisecond frame budget printed in every week from Week 01 to Week 09 and revisited as each new system claims its row — performance held as a running constraint rather than an end-of-term topic | both | [`curriculum/week-02-collisions-and-physics-lite/README.md`](curriculum/week-02-collisions-and-physics-lite/README.md) |
| Two weeks sit past a game-development outcome set entirely: raw UDP sockets, snapshot interpolation and a jitter buffer measured against a real link, and a save format hardened with atomic writes, an HMAC-signed envelope and a hand-written MessagePack codec | university | [`curriculum/week-09-multiplayer-fundamentals/`](curriculum/week-09-multiplayer-fundamentals/) |
| Design work assessed as design: paper deliverables with their own rubrics — a cloud-save protocol, a fighting game's bus tree, a rollback-netcode sketch — graded as written arguments, with no code accepted in their place | both | [`curriculum/week-09-multiplayer-fundamentals/challenges/challenge-02-design-a-rollback-netcode-sketch.md`](curriculum/week-09-multiplayer-fundamentals/challenges/challenge-02-design-a-rollback-netcode-sketch.md) |

**Gaps we declare.** Four against the Computer Graphics claim, and they are the four the ledger records: C11 does not derive the transform pipeline in homogeneous coordinates, does not implement a rasteriser, teaches no shading or lighting model, and writes only 2D canvas-item fragment shaders inside an engine rather than shader programs written against a graphics API from first principles. Against the Game Design and Development outcome set we declare none. Separately, and as an industry-bar shortfall rather than a university gap: C11 configures no formatter, no linter and no continuous-integration pipeline, and the only tests in the course are the ones Week 11 asks the learner to write.

---

## What you will be able to do at the end of 12 weeks

- **Implement a game loop** from scratch: input, update, render, in the right order, at the right rate.
- **Reason about delta-time** so your game feels the same on a 60 Hz laptop and a 144 Hz desktop.
- **Build collisions** that don't lie: AABB, swept tests, separating-axis basics.
- **Animate sprites** properly: state machines, keyframes, easing.
- **Design tilemaps** and load them from data files, not hardcoded arrays.
- **Manage scenes** — title, gameplay, pause, game-over — with clean transitions.
- **Build a Godot 4 project** with nodes, scenes, signals, GDScript.
- **Ship a small game** end-to-end with sound effects, music, persistent save state, and a packaged build.
- **Playtest with structure** — five testers, three behaviors observed, two changes applied.
- **Read other people's small games** without intimidation.

---

## Who this is for

- **C1 graduate** who wanted to make games the whole time.
- **Self-taught Python user** ready for something more visual.
- **Computer-science learner** who wants to apply concepts (state machines, math, data structures) to something tangible.
- **Game-jam aspirant** preparing to ship under deadline.

Not for: people targeting AAA gamedev jobs (do C9 + Unity, or learn Unreal in C++; we don't teach those at scale), nor people focused on game *art* over game programming (this is the engineering side).

---

## Prerequisites

- **C1 Weeks 1–7** (Python, OOP).
- Comfortable terminal + git.
- A computer that can run Godot 4 (~modern; 4GB RAM minimum).
- Patience. Game polish is 80% of the work and 0% of the fun in the first hour.

---

## What you ship

By the end of the 12 weeks, your `crunch-arcade-portfolio-<yourhandle>` GitHub repo contains:

1. A **pure-Python game loop** drawing a moving circle (Week 1).
2. A **paddle / ball / bricks** game in Pygame with collision and scoring (Week 3).
3. A **2D platformer prototype** with a tilemap, jump physics, and one enemy (Week 5).
4. A **state-machine character** with idle / run / jump / hurt animations (Week 6).
5. A **save-load system** that survives a crash (Week 7).
6. A **Godot 4 port** of one of the earlier prototypes (Week 9).
7. A **sound-and-music integration** with at least three SFX and one looping track (Week 10).
8. A **playtest report** with five testers' notes and your three resulting changes (Week 11).
9. **Capstone:** a small polished 2D Godot game (15–20 minutes of gameplay), packaged for at least two platforms, with a public itch.io page (Week 12).

---

## Tools (all free, all open-source)

| Tool | Role |
|------|------|
| **Python 3.11+** | Foundations weeks |
| **Pygame** | Pure-Python game-loop work |
| **Pyxel / Arcade** *(optional)* | Mentioned as alternatives |
| **Godot 4** | The polished capstone |
| **GDScript** | Godot's scripting language (Python-like) |
| **Aseprite community** *(free)* or **Krita** *(free)* | Pixel art |
| **LMMS · Bosca Ceoil · ChipTone** | Free audio tools |
| **Tiled** | Free tilemap editor |
| **itch.io** | Free distribution platform |
| **OBS Studio** | Recording playtests / trailers |

Optional but useful: **a controller** (Xbox / 8BitDo) for testing real input. Most laptops have keyboard input; controllers reveal bugs.

---

## On art assets

Game polish needs art. C11 is not an art course. For all the curriculum's exercises and the capstone, we point at **public-domain or CC0 asset libraries**:

- **Kenney.nl** — extensive CC0 game-asset packs: <https://kenney.nl/>
- **OpenGameArt.org** — community-uploaded; check each asset's license.
- **itch.io free assets** — a wide community library; check each license.

Do NOT use copyrighted assets (Nintendo sprites, official Pokémon art, etc.) even "just to test." It feels safe; it isn't. Use Kenney's free packs as a default.

---

## Next track after C11

- **[C12 · Crunch 3D](../C12-CRUNCH-3D/)** — for 3D visualization and technical art.
- **[C9 · Crunch Sharp](../C9-CRUNCH-SHARP/)** — if your future is Unity / C# game dev.
- **[C16 · Crunch Pro Web Backend](../C16-CRUNCH-PRO-WEB-BACKEND/)** — if your game grows into a multiplayer service.

---

## License

GPL-3.0.

---

*C11 is part of the Code Crunch open-source curriculum.* [Master catalog ↗](../MASTER-CURRICULUM.md) · [Brand family ↗](../../assets/brand/BRAND-FAMILY.md)
