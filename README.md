![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Project](https://img.shields.io/badge/Project-Hardware-yellow.svg)
![Series](https://img.shields.io/badge/Series-APX-red.svg)
![Hackatime Badge](https://hackatime-badge.hackclub.com/U0A2SJ7B739/USB%20HUB)

<table>
  <tr>
    <td width="18%">
      <!-- Replace this later with your hero image -->
      <img width="100%" alt="APX-USB-HUB preview" src="docs/images/hero/placeholder.png" />
    </td>
    <td>
      <h1>APX USB HUB</h1>
      <p>
        Cool USB HUB with 4 USB ports, PTC to protect the board if there is a short circuit and LEDs to indicate which port the problem comes from.
      </p>
    </td>
  </tr>
</table>

---

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Repository Structure](#repository-structure)
- [Bill of Materials](#bill-of-materials)
- [KiCad / Electronics](#kicad--electronics)
- [CAD / Enclosure](#cad--enclosure)
- [3D Printing](#3d-printing)
- [Manufacturing](#manufacturing)
- [Build Notes](#build-notes)
- [Roadmap](#roadmap)
- [License](#license)
- [Contributing](#contributing)

---

## About the Project

**APX-USB-HUB** is a 4-port USB hub designed with **per-port fault indication**: a **PTC fuse** helps protect the board in case of a short circuit, and **LEDs** help identify which port is causing the issue.

> This repository is structured so you can add files progressively (images, BOM, CAD, KiCad) without having to reorganize later.

---

## Features

- **4 USB ports**
- **PTC protection** to help limit current during short circuits
- **Status LEDs** to quickly identify the faulty port
- Documentation-first repo layout (BOM, manufacturing exports, images, etc.)

---

## Repository Structure

Main folders you should use (and keep stable):

- `kicad/` — KiCad project sources + `kicad/exports/` for fabrication outputs
- `bom/` — BOM files (CSV/MD)
- `cad/` — enclosure/mechanical CAD
- `3d-printing/` — print-ready files (STL/3MF) and print notes
- `docs/images/` — images used in the README and documentation
- `hardware/datasheets/` — component datasheets

---

## Bill of Materials

- CSV: `bom/apx-usb-hub_bom.csv` *(to be added)*
- Optional readable BOM: `bom/apx-usb-hub_bom.md`

> For now you can add an empty placeholder file, then fill it later.

---

## KiCad / Electronics

KiCad sources will live in:

- `kicad/APX-USB-HUB.kicad_pro`
- `kicad/APX-USB-HUB.kicad_sch`
- `kicad/APX-USB-HUB.kicad_pcb`

Exports (generated files) should go to:

- `kicad/exports/schematics/` (PDF/PNG)
- `kicad/exports/gerbers/`
- `kicad/exports/assembly/` (CPL / pick&place, positions, etc.)

---

## CAD / Enclosure

- CAD sources: `cad/enclosure/`
- Additional mechanical files: `cad/misc/`

Add preview renders to:

- `docs/images/pcb/`
- `docs/images/hero/`

---

## 3D Printing

Print-ready files should go to:

- `3d-printing/stl/`
- `3d-printing/3mf/`

Recommended: add printer/slicer settings in `3d-printing/README.md`.

---

## Manufacturing

Manufacturing notes and supplier links can go to:

- `docs/manufacturing/`

If you produce a panel or use an assembly service, keep the outputs under:

- `kicad/exports/gerbers/`
- `kicad/exports/assembly/`

---

## Build Notes

Add photos and step-by-step documentation here:

- `docs/images/build/`
- `docs/wiring/`

---

## Roadmap

- [ ] Add schematic export (PNG/PDF) in `kicad/exports/schematics/`
- [ ] Add PCB renders in `docs/images/pcb/`
- [ ] Add BOM in `bom/apx-usb-hub_bom.csv`
- [ ] Add enclosure CAD + print files
- [ ] Add assembly/build photos

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions, improvements, and remixes are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guide to get started.
