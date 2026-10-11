# Tips And Tricks

# 07. Tips and Tricks

## 1. Workflow habits

- **Sketch on paper first.** Five minutes with a pencil saves an hour in CAD.
- **Design top-down for assemblies.** Start with the layout (envelope, key interfaces), then detail each part.
- **Keep one master model** and export copies. Do not edit exported files.
- **Save versions often** (RevA, RevB) and keep a short change log.
- **Take screenshots and notes** of decisions and test results.
- **Do a design review** with a friend, classmate, or mentor before ordering anything.
- **Prototype cheap.** Cardboard, foam board, laser-cut acrylic, or a 3D print can reveal problems quickly.
- **Test the riskiest part first.** Find out early if the hardest idea works.

## 2. CAD habits

- Fully define sketches and start from the origin.
- Add fillets and chamfers last.
- Use global variables or design parameters for key dimensions (wall thickness, hole size, clearances).
- Use patterns and mirrors, not copy and paste.
- Name important sketches, features, and parts.
- Use configurations or variants for part families (for example bolt lengths).
- Reuse parts: build a personal library of standard brackets, holes, and fastener patterns.
- Use sections and cross-section views to check internal features.
- Use measure tools and mass properties to check dimensions, weight, and centre of mass.
- Check for interference before you release an assembly.

## 3. SolidWorks quick shortcuts

| Action | Shortcut |
|---|---|
| Shortcut bar | S |
| Rebuild | Ctrl + B |
| Force rebuild | Ctrl + Q |
| Zoom to fit | F |
| Previous view | Shift + Z (zoom in) / Z (zoom out) |
| Rotate view | Middle mouse drag |
| Pan | Ctrl + middle mouse drag |
| View orientation menu | Space bar |
| Normal to (selected face) | Ctrl + 8 |
| Select other (hidden face) | Right-click, then Select Other |
| Repeat last command | Enter |
| Hide / show | Tab / Shift + Tab (hover over a part in an assembly) |

SolidWorks also lets you customise shortcuts (Tools, Customize). Set your own for the commands you use most.

## 4. Fusion 360 tips

- Use the **timeline** to edit past steps, and drag the marker back to insert features.
- Start in the **Design** workspace and use **Components** (not just bodies) for assembly parts.
- Use **joints** instead of rigid groups for moving parts.
- Use **parameters** (Modify, Change Parameters) to drive dimensions.
- Use **Capture Design History** and keep it on.
- Use the **Manufacture** workspace for CAM toolpaths.
- Save to the cloud project, and export a STEP backup for important designs.

## 5. FreeCAD tips

- Work in the **Part Design** workbench with **bodies** and **sketches**.
- Use the **spreadsheet** to drive parameters.
- Avoid the topological naming problem by referencing sketches and datum planes instead of faces and edges (the 1.0 release improved this a lot, but it is still good practice).
- Use **TechDraw** for drawings and **FEM** for simulation.
- Save often. Enable auto-recovery in preferences.

## 6. Onshape tips

- Use **Part Studios** for parts, **Assemblies** for mates, and **Drawings** for prints.
- Use **versions and branches** like Git. Create a version before big changes.
- Use **variables** (#name) to drive dimensions.
- Share a link to let teammates view or edit live.
- Use **FeatureScript** custom features to add tools.
- Keep documents organised in folders and projects.

## 7. Engineering rules of thumb

| Topic | Rule |
|---|---|
| Fillets | Use the largest radius you can, since it reduces stress and machining cost |
| Wall thickness | Keep uniform, and avoid thick sections next to thin ones |
| Hole position | Centre at least 1.5 to 2 times the hole diameter from an edge |
| Thread engagement | About 1.5 times diameter in steel, 2 times in aluminium |
| Ribs vs thickness | Adding a rib is usually lighter and stiffer than thickening |
| Beam depth | Doubling depth gives about 8 times the bending stiffness |
| Tubes | Hollow sections are very efficient in bending and torsion |
| Shaft length | Long, thin shafts whip and deflect. Support them with bearings |
| Bearing spacing | Place bearings as far apart as practical for a stable shaft |
| Plastic screws | Use inserts for repeated assembly |
| Printed holes | Print slightly small, then drill or ream if precision is needed |
| Centre of mass | Keep heavy parts low and close to the centre for stable robots |
| Tolerance | Loosest that works. Tight tolerances cost money |
| Standard parts | Always check catalogues before designing a custom part |

## 8. Mechanical design hacks for projects and robots

- Use **aluminium extrusion (2020 or 3030)** for quick, adjustable frames.
- Use **laser-cut or waterjet plates** for flat brackets and bases.
- Use **heat-set inserts** in 3D prints for strong threads.
- Use **slots instead of round holes** for adjustment during assembly.
- Leave **mounting holes in standard patterns** (for example NEMA 17 motor pattern 31 mm spacing, 22 mm pilot).
- Add **cable routing** and **access panels** early in the design.
- Design **motor and gearbox mounts** with adjustable tension for belts and chains.
- Keep **electronics accessible** and ventilated, and label wires.
- Leave **clearance for tools** and for your fingers.
- Design a **test jig** if you need to test the same part many times.

## 9. Debugging mechanical problems

1. **Define the failure.** What happens, when, and how often?
2. **Check the basics.** Loose fasteners, misalignment, binding, wrong parts.
3. **Measure.** Use calipers and photos instead of guessing.
4. **Change one thing at a time.**
5. **Look for stress risers, wear marks, and cracks.**
6. **Compare with the CAD.** Is the real part what you modelled?
7. **Write down what you learned** and update the design.

## 10. Learning resources

- **Books:** Shigley's Mechanical Engineering Design, Machinery's Handbook, Engineering Drawing (N.D. Bhatt), Mechanics of Materials (Beer and Johnston).
- **Standards:** ISO 286 (fits), ISO 2768 (general tolerances), ASME Y14.5 (GD&T), ISO 898 (fastener properties).
- **Catalogues:** McMaster-Carr, Misumi, RS Components, Robu.in, and local suppliers.
- **Practice:** Redesign an everyday object, reverse-engineer a part, join a design team or competition, and build something every semester.
- **Communities:** r/MechanicalEngineering, r/SolidWorks, r/FreeCAD, r/Fusion360, and the Onshape and Autodesk forums.

## 11. Final advice

- Understand the physics, then use the software.
- Learn from manufacturing, because the shop floor teaches what textbooks do not.
- Keep designs simple. The best part is the one you do not need.
- Document everything, since future you will thank you.
- Build, test, break, and improve. That is how engineers learn.
