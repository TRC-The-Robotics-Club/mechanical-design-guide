
# CAD Setup and Mechanical Design Guide

Covers SolidWorks, Fusion 360, FreeCAD, and Onshape on Windows.

## 1. Which Tool for What

| Tool | Cost for Students | Runs On | Strengths | Weak Points |
|---|---|---|---|---|
| SolidWorks | Free via student program (reference number by email) | Windows only | Industry standard, strong assemblies, drawings, simulation | Heavy, Windows only |
| Fusion 360 | Free educational license (renews yearly, non-commercial) | Windows, macOS | CAD + CAM + simulation in one, cloud collaboration | Needs internet, cloud-based file handling |
| FreeCAD | Free, open source | Windows, Linux, macOS | Parametric, scriptable, no license limits | Steeper learning curve, occasional bugs |
| Onshape | Free education plan | Browser (any OS) | Real-time collaboration, version control, no install | Needs internet, public documents on free plans (education plan allows private) |

**Practical advice:** Learn one tool deeply (SolidWorks or Fusion 360), and know a second one so you can open and share files.

---

## 2. Installation Overview (Windows)

### System Requirements

| Requirement | Recommendation |
|---|---|
| Operating System | 64-bit Windows 10 or 11 |
| RAM | 16 GB recommended |
| Storage | SSD |
| Graphics | Dedicated GPU preferred |
| Free Disk Space | 40 GB |

### FreeCAD

| Step | Procedure |
|---|---|
| 1 | Go to [freecad.org](https://www.freecad.org/) and open Downloads. |
| 2 | Download the stable Windows installer. |
| 3 | Run it with default options. |
| 4 | Open it and check that the 3D view works. |

### Onshape

| Step | Procedure |
|---|---|
| 1 | Use Chrome or Edge with hardware acceleration on. |
| 2 | Go to [onshape.com](https://www.onshape.com/) and find the Education plan. |
| 3 | Sign up with your college email and verify it. |
| 4 | Create a document and test a sketch plus extrude. |

### Fusion 360

| Step | Procedure |
|---|---|
| 1 | Go to [autodesk.com/education](https://www.autodesk.com/education) and sign in with your college email. |
| 2 | Verify student status and pick the Education license. |
| 3 | Download and run the installer, then sign in. |
| 4 | Set the default modeling orientation (Z up is the mechanical standard) under Preferences. |

### SolidWorks

| Step | Procedure |
|---|---|
| 1 | Go to the SolidWorks student page on [solidworks.com](https://www.solidworks.com/). |
| 2 | Request access with your college email and generate a reference number, which is sent to your email. |
| 3 | Keep the email safe. You need the reference number to download and activate. |
| 4 | Log in at [my.solidworks.com](https://my.solidworks.com/), open Downloads, and get the Installation Manager. |
| 5 | Run it, choose Individual installation, and enter the reference or serial number. |
| 6 | Keep SolidWorks, Simulation, and Toolbox selected. Deselect extras. |
| 7 | Install (30 to 60 minutes) and restart. |

**First run configuration:**

| Setting | Procedure |
|---|---|
| Units | Set units to MMGS (Tools → Options → Document Properties → Units). |
| Hardware Acceleration | Enable it under System Options → Performance. |

---

## 3. The Core CAD Workflow (Same Idea in Every Tool)

| Step | Operation | Description |
|---|---|---|
| 1 | Sketch | Sketch on a plane (2D profile). |
| 2 | Constrain | Constrain the sketch fully (dimensions plus geometric relations). |
| 3 | Feature | Extrude, revolve, sweep, loft. |
| 4 | Modify | Cut, hole, fillet, chamfer, shell, pattern, mirror. |
| 5 | Assemble | Assemble parts with mates or joints. |
| 6 | Drawing | Create views, dimensions, tolerances, and a title block. |
| 7 | Export | Export to the format you need. |

### Terms Across Tools

| Concept | SolidWorks | Fusion 360 | FreeCAD | Onshape |
|---|---|---|---|---|
| Part file | Part (.sldprt) | Component in Design | Part Design body | Part Studio |
| Assembly | Assembly (.sldasm) | Assembly in Design | Assembly workbench | Assembly tab |
| Relation between parts | Mates | Joints | Constraints / joints | Mates |
| History | FeatureManager tree | Timeline | Model tree | Feature list |
| 2D print | Drawing (.slddrw) | Drawing | TechDraw | Drawing |

---

## 4. Sketching Rules That Save You Pain

| Rule | Explanation |
|---|---|
| Fully define sketches | In SolidWorks, aim for black (fully defined), not blue (under-defined). |
| Start from the origin | Start sketches from the origin so the part has a stable reference. |
| Use construction lines | Use construction lines for symmetry and centre lines. |
| Apply relations first | Use relations (coincident, tangent, equal, symmetric) before adding dimensions. |
| Keep sketches simple | Many small sketches are better than one huge one. |
| Dimension correctly | Dimension the way the part will be measured or manufactured. |

---

## 5. Modelling Best Practices

| Practice | Explanation |
|---|---|
| Base shape first | Model the base shape first, then details (fillets, chamfers last). |
| Add fillets near the end | Early fillets cause rebuild errors when you edit. |
| Name features | Name important features and sketches. |
| Use design parameters | Use design parameters or global variables for key dimensions (for example, wall thickness). |
| Use patterns and mirrors | Use patterns and mirrors instead of copying features. |
| Meaningful origin | Keep the part origin at a meaningful place (centre of a bore, corner of a base). |
| Stable references | Avoid referencing edges or faces that may disappear when edited. Reference planes and sketches where possible. |

---

## 6. Assembly Best Practices

| Practice | Explanation |
|---|---|
| Fix the first part | Fix (ground) the first part, usually the base or frame. |
| Real-world mates | Mate with real-world logic: concentric plus coincident for bolts, tangent for rollers. |
| Use sub-assemblies | Use sub-assemblies to keep large assemblies manageable. |
| Standard parts | Insert standard parts from the library (Toolbox in SolidWorks, McMaster-Carr or built-in content in Fusion 360 and Onshape). |
| Interference checks | Run interference or collision checks. |
| Motion checks | Check motion with mate limits or motion study. |

---

## 7. Drawings

A good drawing has:

| Requirement | Details |
|---|---|
| Title Block | Correct title block (part name, number, material, scale, units, revision, author). |
| Views | Front, top, and side views plus an isometric view. |
| Section and Detail Views | Section and detail views where needed. |
| Dimensions | Complete dimensions, with no duplicates and no missing ones. |
| Tolerances and GD&T | Tolerances and GD&T on critical features (see 04). |
| Surface Finish | Surface finish and general notes. |
| BOM and Balloons | BOM and balloons for assemblies. |

---

## 8. File Formats and When to Use Them

| Format | Extension | Use For |
|---|---|---|
| STEP | `.step`, `.stp` | Best neutral CAD exchange, keeps solid geometry. |
| IGES | `.igs` | Older exchange format, use when STEP fails. |
| STL | `.stl` | 3D printing, mesh only, no units stored. |
| 3MF | `.3mf` | Modern 3D printing format with units and colour. |
| DXF / DWG | `.dxf`, `.dwg` | 2D profiles for laser cutting, waterjet, CNC plasma. |
| PDF | `.pdf` | Releasing drawings. |
| Parasolid | `.x_t` | Exchange with Parasolid-based systems. |
| Native | `.sldprt`, `.f3d`, `.FCStd` | Your master files, always keep these. |

**Tip:** For ROS or robotics simulation, export meshes as STL or DAE and keep scale and units consistent (mm versus m is a classic mistake).

---

## 9. Simulation and CAM Options

| Tool | Available Options |
|---|---|
| SolidWorks Simulation | Static, frequency, thermal, buckling (depending on package). |
| Fusion 360 | Simulation and CAM (toolpaths for CNC) in the same environment. |
| FreeCAD | FEM workbench (with CalculiX) and Path workbench for CAM. |
| Onshape | Simulation and CAM via partners or add-ons depending on plan. |

**Important:** Always sanity check FEA with a hand calculation.

---

## 10. Project Organisation

### Recommended Folder Structure

```text
Project/
├── 01-Requirements/
├── 02-CAD/
│   ├── Parts/
│   └── Assemblies/
├── 03-Drawings/
├── 04-Exports/
│   ├── STEP/
│   ├── STL/
│   └── DXF/
├── 05-Analysis/
├── 06-Manufacturing/
│   ├── Quotes/
│   ├── G-code/
│   └── Orders/
└── 07-Docs/
```

### Project Management Practices

| Practice | Explanation |
|---|---|
| Naming scheme | Use a naming scheme like `PRJ-001-Base-Plate-RevA`. |
| Backups | Back up to cloud or Git (store CAD and exports, ignore temp files). |
| File references | Do not rename or move referenced files outside the CAD program (use Pack and Go or Copy Project). |

---

## 11. Hardware Tips

| Topic | Recommendation |
|---|---|
| Mouse | Use a mouse with a scroll wheel. |
| 3D Navigation | A 3Dconnexion SpaceMouse is a luxury but helpful. |
| GPU | Set apps to High performance GPU in Windows graphics settings. |
| Performance | Close heavy apps while working on large assemblies. |
| Saving | Save often. |
| Auto-Recovery | Turn on auto-recovery. |
