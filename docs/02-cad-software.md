# Cad Software

Covers SolidWorks, Fusion 360, FreeCAD, and Onshape on Windows.

### 1. Which tool for what
Tool	Cost for students	Runs on	Strengths	Weak points
SolidWorks	Free via student program (reference number by email)	Windows only	Industry standard, strong assemblies, drawings, simulation	Heavy, Windows only
Fusion 360	Free educational license (renews yearly, non-commercial)	Windows, macOS	CAD + CAM + simulation in one, cloud collaboration	Needs internet, cloud-based file handling
FreeCAD	Free, open source	Windows, Linux, macOS	Parametric, scriptable, no license limits	Steeper learning curve, occasional bugs
Onshape	Free education plan	Browser (any OS)	Real-time collaboration, version control, no install	Needs internet, public documents on free plans (education plan allows private)

Practical advice: learn one tool deeply (SolidWorks or Fusion 360), and know a second one so you can open and share files.

### 2. Installation overview (Windows)

Check your system first: 64-bit Windows 10 or 11, 16 GB RAM recommended, SSD, dedicated GPU preferred, 40 GB free disk.

#### FreeCAD
Go to freecad.org and open Downloads.
Download the stable Windows installer.
Run it with default options.
Open it and check that the 3D view works.

#### Onshape
Use Chrome or Edge with hardware acceleration on.
Go to onshape.com and find the Education plan.
Sign up with your college email and verify it.
Create a document and test a sketch plus extrude.

#### Fusion 360
Go to autodesk.com/education and sign in with your college email.
Verify student status and pick the Education license.
Download and run the installer, then sign in.
Set the default modeling orientation (Z up is the mechanical standard) under Preferences.

#### SolidWorks
Go to the SolidWorks student page on solidworks.com.
Request access with your college email and generate a reference number, which is sent to your email.
Keep the email safe. You need the reference number to download and activate.
Log in at my.solidworks.com, open Downloads, and get the Installation Manager.
Run it, choose Individual installation, and enter the reference or serial number.
Keep SolidWorks, Simulation, and Toolbox selected. Deselect extras.
Install (30 to 60 minutes) and restart.
First run: set units to MMGS (Tools, Options, Document Properties, Units) and enable hardware acceleration (System Options, Performance).

### 3. The core CAD workflow (same idea in every tool)
Sketch on a plane (2D profile).
Constrain the sketch fully (dimensions plus geometric relations).
Feature: extrude, revolve, sweep, loft.
Modify: cut, hole, fillet, chamfer, shell, pattern, mirror.
Assemble parts with mates or joints.
Drawing with views, dimensions, tolerances, and a title block.
Export to the format you need.
Terms across tools
Concept	SolidWorks	Fusion 360	FreeCAD	Onshape
Part file	Part (.sldprt)	Component in Design,	Part Design body	Part Studio
Assembly	Assembly (.sldasm)	Assembly in Design	Assembly workbench	Assembly tab
Relation between parts	Mates	Joints	Constraints / joints	Mates
History	FeatureManager tree	Timeline	Model tree	Feature list
2D print	Drawing (.slddrw)	Drawing	TechDraw	Drawing

### 4. Sketching rules that save you pain
Fully define sketches. In SolidWorks, aim for black (fully defined), not blue (under-defined).
Start sketches from the origin so the part has a stable reference.
Use construction lines for symmetry and centre lines.
Use relations (coincident, tangent, equal, symmetric) before adding dimensions.
Keep sketches simple. Many small sketches are better than one huge one.
Dimension the way the part will be measured or manufactured.

### 5. Modelling best practices
Model the base shape first, then details (fillets, chamfers last).
Add fillets near the end. Early fillets cause rebuild errors when you edit.
Name important features and sketches.
Use design parameters or global variables for key dimensions (for example wall thickness).
Use patterns and mirrors instead of copying features.
Keep the part origin at a meaningful place (centre of a bore, corner of a base).
Avoid referencing edges or faces that may disappear when edited. Reference planes and sketches where possible.

### 6. Assembly best practices
Fix (ground) the first part, usually the base or frame.
Mate with real-world logic: concentric plus coincident for bolts, tangent for rollers.
Use sub-assemblies to keep large assemblies manageable.
Insert standard parts from the library (Toolbox in SolidWorks, McMaster-Carr or built-in content in Fusion 360 and Onshape).
Run interference or collision checks.
Check motion with mate limits or motion study.

### 7. Drawings
A good drawing has:
Correct title block (part name, number, material, scale, units, revision, author)
Front, top, and side views plus an isometric view
Section and detail views where needed
Complete dimensions, with no duplicates and no missing ones
Tolerances and GD&T on critical features (see 04)
Surface finish and general notes
BOM and balloons for assemblies

### 8. File formats and when to use them
Format	Use for
STEP (.step, .stp)	Best neutral CAD exchange, keeps solid geometry
IGES (.igs)	Older exchange format, use when STEP fails
STL (.stl)	3D printing, mesh only, no units stored
3MF (.3mf)	Modern 3D printing format with units and colour
DXF / DWG	2D profiles for laser cutting, waterjet, CNC plasma
PDF	Releasing drawings
Parasolid (.x_t)	Exchange with Parasolid-based systems
Native (.sldprt, .f3d, .FCStd)	Your master files, always keep these

Tip: for ROS or robotics simulation, export meshes as STL or DAE and keep scale and units consistent (mm versus m is a classic mistake).

### 9. Simulation and CAM options
SolidWorks Simulation: static, frequency, thermal, buckling (depending on package).
Fusion 360: simulation and CAM (toolpaths for CNC) in the same environment.
FreeCAD: FEM workbench (with CalculiX) and Path workbench for CAM.
Onshape: simulation and CAM via partners or add-ons depending on plan.

Always sanity check FEA with a hand calculation.

### 10. Project organisation
Project/
  01-Requirements/
  02-CAD/ Parts/Assemblies/
  03-Drawings/
  04-Exports/        (STEP, STL, DXF)
  05-Analysis/
  06-Manufacturing/  (quotes, G-code, orders)
  07-Docs/
Use a naming scheme like PRJ-001-Base-Plate-RevA.
Back up to cloud or Git (store CAD and exports, ignore temp files).
Do not rename or move referenced files outside the CAD program (use Pack and Go or Copy Project).

### 11. Hardware tips
Use a mouse with a scroll wheel. A 3Dconnexion SpaceMouse is a luxury but helpful.
Set apps to High performance GPU in Windows graphics settings.
Close heavy apps while working on large assemblies.
Save often. Turn on auto-recovery.
