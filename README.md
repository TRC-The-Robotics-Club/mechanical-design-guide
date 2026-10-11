# Mechanical Design Guide

A practical, student-friendly guide to mechanical design: from first principles to CAD, materials, tolerances, manufacturing, and the mistakes everyone makes at least once.

## About this guide

Most students learn mechanics in theory and CAD in a lab, but rarely learn how the two meet on a real project. This guide fills that gap. It follows the path of a real part: define the need, design it, model it, choose a material, set tolerances, pick a manufacturing process, and check for mistakes before anything is built.

The goal is simple: **a part that works in CAD should also work when it is built.**

## What you will learn

- How to turn a vague need into measurable requirements
- How to size parts using basic stress and stiffness formulas
- How to set up and use SolidWorks, Fusion 360, FreeCAD, and Onshape
- How to choose materials for strength, weight, cost, and environment
- How to read and write fits, tolerances, and basic GD&T
- How to design for machining, sheet metal, casting, molding, and 3D printing
- How to avoid the most common design, CAD, drawing, and assembly mistakes
- How to work faster with shortcuts, habits, and rules of thumb

## Contents

| # | Topic | What you will learn | Best for |
|---|---|---|---|
| 01 | [Design Fundamentals](docs/01-design-fundamentals.md) | Design process, requirements, loads, factor of safety, DFM/DFA | Starting any project |
| 02 | [CAD Software](docs/02-cad-software.md) | SolidWorks, Fusion 360, FreeCAD, Onshape: setup, workflow, file formats | Setting up tools and modelling |
| 03 | [Materials Selection](docs/03-materials-selection.md) | Properties, metals, plastics, how to choose | Choosing what to make it from |
| 04 | [GD&T and Tolerances](docs/04-gdt-and-tolerances.md) | Fits, datums, feature control frames, stack-ups | Making drawings and parts that fit |
| 05 | [Manufacturing Processes](docs/05-manufacturing-processes.md) | Machining, sheet metal, casting, molding, 3D printing, joining | Deciding how to build it |
| 06 | [Common Mistakes](docs/06-common-mistakes.md) | What goes wrong and how to avoid it | Reviewing before release |
| 07 | [Tips and Tricks](docs/07-tips-and-tricks.md) | Shortcuts, workflow habits, rules of thumb | Quick reference |

## Who this is for

- Mechanical engineering students working on college projects
- Robotics and engineering club members building hardware
- Hobbyists and makers building robots, enclosures, and machines
- Beginners moving from "it looks right in CAD" to "it works when built"

No prior industry experience is needed. Basic knowledge of statics and strength of materials helps, but each topic explains the key ideas.

## Recommended learning path

| Stage | Read | Goal |
|---|---|---|
| 1. Foundation | 01 | Learn the design mindset and basic calculations |
| 2. Tools | 02 | Install and test your CAD software |
| 3. Design a part | 03, 04, 05 | Choose material, tolerances, and process for a real part |
| 4. Review | 06 | Catch mistakes before ordering or machining |
| 5. Improve | 07 | Work faster and cleaner on the next project |

## How to use this guide

1. Read 01 first to learn the design mindset.
2. Set up your tools using 02.
3. Use 03 to 05 while designing a real part.
4. Check 06 before you release any drawing or order any part.
5. Keep 07 open as a quick reference.

Tip: do not try to memorise everything. Read once, then come back to the relevant file when you hit that problem in your project.

## Repository structure

```
.
├── README.md
└── docs/
    ├── 01-design-fundamentals.md
    ├── 02-cad-software.md
    ├── 03-materials-selection.md
    ├── 04-gdt-and-tolerances.md
    ├── 05-manufacturing-processes.md
    ├── 06-common-mistakes.md
    └── 07-tips-and-tricks.md
```

## Software covered

| Tool | Cost for students | Runs on |
|---|---|---|
| SolidWorks | Free via student program | Windows |
| Fusion 360 | Free educational license | Windows, macOS |
| FreeCAD | Free, open source | Windows, Linux, macOS |
| Onshape | Free education plan | Any browser |

## Quick start

1. Clone or download this repository.
2. Open `docs/01-design-fundamentals.md` and read it end to end.
3. Follow `docs/02-cad-software.md` to install your CAD tools.
4. Pick a small part (a bracket or a motor mount) and design it using files 03 to 05.
5. Run through the checklist in `docs/06-common-mistakes.md` before you release it.

## Key terms

| Term | Meaning |
|---|---|
| DFM | Design for Manufacturing: designing so the part is easy and cheap to make |
| DFA | Design for Assembly: designing so the product is easy to put together |
| FoS | Factor of safety: failure strength divided by working stress |
| GD&T | Geometric Dimensioning and Tolerancing: symbols that control shape, orientation, and location |
| BOM | Bill of Materials: the list of every part and quantity in a product |
| FEA | Finite Element Analysis: computer simulation of stress, heat, and vibration |
| STEP | A neutral CAD file format used to share models between programs |

## Conventions

- Units are metric (mm, N, MPa, kg) unless stated otherwise.
- Numbers are typical values for guidance. Always check supplier datasheets and standards for your exact case.
- Part numbers, standards, and tolerances change by region and supplier, so verify before manufacturing.
- Examples use common stock sizes and fasteners, but availability varies by country.

## Disclaimer

This guide is for learning and general guidance. It does not replace engineering codes, standards, or professional review. For safety-critical designs (lifting, pressure, structures, medical, vehicles), follow the relevant standards and have the design reviewed by a qualified engineer.

## Roadmap

- [ ] Add worked examples (bracket, shaft, gearbox mount)
- [ ] Add fastener and bearing selection guide
- [ ] Add basic FEA workflow for each CAD tool
- [ ] Add a project notes template for documenting your own builds
- [ ] Add diagrams and CAD screenshots

## Contributing

Found an error or want to add a section? Contributions are welcome.

1. Fork the repository.
2. Create a branch for your change (for example `fix-tolerance-table`).
3. Keep the same style: short sections, tables where useful, and checklists at the end.
4. Open a pull request with a short description of what you changed and why.

You can also open an issue to suggest a topic or report a mistake.

