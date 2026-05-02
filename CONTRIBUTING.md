# Contributing to APX USB HUB

Thanks for your interest in contributing! This is a hardware project, so contributions can include electronics, PCB layout, mechanical design, documentation, and manufacturing improvements.

---

## Table of Contents

- [What Contributions Are Welcome](#what-contributions-are-welcome)
- [Project Structure (Where to Put Files)](#project-structure-where-to-put-files)
- [How to Contribute](#how-to-contribute)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Reporting Issues](#reporting-issues)
- [Code of Conduct](#code-of-conduct)

---

## What Contributions Are Welcome

### PCB
- Schematic improvements (LEDs light up only when port used, ESD, filtering, power distribution).
- PCB layout improvements (routing, grounding, test points, silkscreen clarity).
- Suggestions for better fault detection / LED indication behavior.
- Alternative PTC values or protection approaches (with justification).

### CAD
- Different enclosure designs, mounting features, cable strain relief.
- Improvements for the actual version that is too simple
- Improvements for printability and robustness.

### Documentation
- Fixing typos, improving clarity in README and add build steps.
- Adding diagrams, annotated images, and assembly photos.
- Adding manufacturing notes (Gerber export settings, recommended fab settings).

---

## Project Structure (Where to Put Files)

Please follow these conventions to keep the repo clean:

- `src/easyeda/` — EasyEDA project sources (schematic, PCB)
- `src/easyeda/pcb/` — EasyEDA PCB source file
- `src/easyeda/schem/` — EasyEDA schematic source file
- `production/pcb/` — PCB fabrication outputs (Gerbers, BOM CSV, Pick & Place)
- `production/cad/` — 3D-printing files (.3mf)
- `src/cad/` — mechanical CAD sources (.f3z, .step)
- `images/` — images used by the README

Try to avoid committing random exports to the root folder.

---

## How to Contribute

### 1. Fork the repository
Use the **Fork** button on GitHub.

### 2. Clone your fork
```bash
git clone https://github.com/<your-username>/APX-USB-HUB.git
cd APX-USB-HUB
```

### 3. Create a new branch
Use a descriptive name:
```bash
git checkout -b feat/add-esd-protection
# or
git checkout -b fix/silkscreen-labels
# or
git checkout -b docs/add-build-photos
```

### 4. Make your changes
- For EasyEDA: keep the main sources in `src/easyeda/` and place fabrication exports in `production/pcb/`.
- For documentation: update `README.md` and/or add images under `images/`.
- For CAD/3D printing: keep sources under `src/cad/` and print files under `production/cad/`.

### 5. Commit your changes
```bash
git add .
git commit -m "feat: add test points for USB power rails"
```

### 6. Push and open a Pull Request
```bash
git push origin feat/add-esd-protection
```
Then open a PR targeting the default branch.

---

## Submitting a Pull Request

To keep PRs easy to review:
- Keep PRs focused on a single topic.
- Include screenshots/renders when modifying PCB/CAD.
- If you change the BOM, update the BOM file(s) under `production/pcb/`.
- If you change file locations, update links in `README.md`.

---

## Reporting Issues

If you find a problem, open an issue and include:
- What you expected vs what happened
- Steps to reproduce (if applicable)
- Photos/screenshots/renders if relevant
- Your context (fab, printer settings, assembly details)

---

## Code of Conduct

Be respectful and constructive. Everyone is welcome regardless of skill level.
