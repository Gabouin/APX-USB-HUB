![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Project](https://img.shields.io/badge/Project-Hardware-yellow.svg)
![Series](https://img.shields.io/badge/Series-APX-red.svg)
![Hackatime Badge](https://hackatime-badge.hackclub.com/U0A2SJ7B739/USB%20HUB)

# APX USB HUB

<table>
  <tr>
    <td width="70%">
      <img width=95% alt="image" src="https://github.com/user-attachments/assets/9b4e1c92-7d47-4f66-aab3-16fa35ab4673" />
    </td>
    <td>
      <p>
        USB HUB with 4 USB 2.0 ports, PTC to protect the board if there is a short circuit and LEDs to indicate which port the problem comes from. The USB ports are linked to a SL2.1A chip thanks to D- and D+ traces that are the same lenght to have the best signal possible ! The silkscreen is elaborate with cool drawings of Dinorpheus (Hack Club's mascot), PEPE the frog and a cool emoji that I love. There is also a QR CODE that link to my website.
      </p>
    </td>
  </tr>
</table>

---

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Repository Structure](#repository-structure)
- [Schematic](#schematic-on-easyeda)
- [PCB](#pcb-on-easyeda)
- [CAD](#cad)
- [Bill of Materials](#bill-of-materials)
- [License](#license)
- [Contributing](#contributing)

---

## About the Project

**APX USB HUB** is a 4-port USB hub designed with **per-port fault indication**: a **PTC fuse** helps protect the board in case of a short circuit, and **LEDs** help identify which port is causing the issue.

---

## Features

- **4 USB ports**
- **PTC protection** to help limit current during short circuits
- **Status LEDs** to quickly identify the faulty port

---

## Repository Structure

Main folders you should use (and keep stable):

- `src/easyeda/` — EasyEDA project sources
- `production/` for fabrication outputs
- `production/bom/` — BOM files (CSV/MD)
- `src/cad/` — mechanical CAD
- `src/cad/printing/` — enclosure CAD
- `images/` — images used in the README and documentation

---

## Schematic on EasyEDA

Source : `src/easyeda/schem/`  

<img width=90% alt="Schematic_USB-HUB_2026-04-30" src="https://github.com/user-attachments/assets/8b705584-d4ca-4481-b807-c388a4a429d1" />

---

## PCB on EasyEDA

Source : `src/easyeda/pcb/`  

<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=90% alt="Capture d&#39;écran 2026-04-30 224539" src="https://github.com/user-attachments/assets/530cfefe-2f57-424b-854e-35af1d31fe8d" /></td>
      <td valign="bottom"><img width=120% alt="Capture d&#39;écran 2026-04-30 224600" src="https://github.com/user-attachments/assets/2ccbf484-b775-496d-a6e4-b73c638ddd77" /> </td>
      <td valign="bottom"><img width=90% alt="Capture d&#39;écran 2026-04-30 224614" src="https://github.com/user-attachments/assets/5dff19da-bd89-4772-a423-34a431e05983" /></td>
  </table>
</div>
<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-04-28 222300" src="https://github.com/user-attachments/assets/406c1b7d-0544-4e32-b367-07517c7ed280" /></td>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-04-28 222439" src="https://github.com/user-attachments/assets/3a3d7d4b-6fa9-49ce-826e-584248bf74ac" /></td>
  </table>
</div>



---

## CAD

### The entire product - render
<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=100% alt="image" src="https://github.com/user-attachments/assets/c08d97f3-9e2e-4b57-b1db-f5c6ff6f3498" />
</td>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-05-03 000834" src="https://github.com/user-attachments/assets/43b00fa7-6010-416f-ac75-5c3624a461ec" /></td>
  </table>
</div>

- source: `src/cad/`  

### Parts to 3D print - render
<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=100% alt="image" src="https://github.com/user-attachments/assets/8b3ae70c-0c3f-41f7-b70e-9021f49e8d03" /></td>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-05-03 001811" src="https://github.com/user-attachments/assets/73842b73-bc4f-460b-9bf4-d9a2110d44aa" /></td>
  </table>
</div>

- source: `production/printing/`

---

## Bill of Materials

Source: `production/APX_USB_HUB-bom.csv`

| ID | Name | Designator | Footprint | Quantity | Manufacturer Part | Manufacturer | Supplier | Supplier Part | Price | Pins |
|---:|---|---|---|---:|---|---|---|---|---:|---:|
| 1 | 10uF | C1,C2,C3,C4,C5,C6,C7 | C0603 | 7 | CL10A106KP8NNNC | SAMSUNG(三星) | LCSC | C19702 | 0.008 | 2 |
| 2 | NSR0320MW2T1G | D1 | SOD-323_L1.8-W1.3-LS2.5-RD | 1 | NSR0320MW2T1G | onsemi(安森美) | LCSC | C48192 | 0.118 | 2 |
| 3 | SMD1206P050TF | F1,F2,F3,F4 | F1206 | 4 | SMD1206P050TF | RUILON(瑞隆源) | LCSC | C20799 | 0.08 | 2 |
| 4 | 19-21/BHC-AN1P2/4T | L1,L2,L3,L4 | LED0603-R-RD | 4 | 19-21/BHC-AN1P2/4T | EVERLIGHT(亿光) | LCSC | C2986002 | 0.069 | 2 |
| 5 | 1kΩ | R1,R2,R3,R4 | R0805 | 4 | RC0805FR-071KL | YAGEO(国巨) | LCSC | C95781 | 0.003 | 2 |
| 6 | SL2.1A | U1 | SOP-16_L10.0-W3.9-P1.27-LS6.0-BL | 1 | SL2.1A | CoreChips(和芯润德) | LCSC | C192893 | 0.235 | 16 |
| 7 | U-G-04DD-W-01 | USB1 | USB-A-TH_U-G-04WD-W-01 | 1 | U-G-O4DD-W-1 | 韩国韩荣 | LCSC | C98125 | 0.112 | 6 |
| 8 | USB-AF-90-14.4X13.6-H7.0-DIP | USB2,USB3,USB4,USB5 | USB-A-TH_C46407 | 4 | 903-131A1011D10100 | 精拓金 | LCSC | C46407 | 0.048 | 6 |

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions, improvements, and remixes are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guide to get started.
