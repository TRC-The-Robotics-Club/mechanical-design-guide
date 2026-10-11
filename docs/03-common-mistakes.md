# Common Mistakes

Every engineer makes these. The goal is to make them on paper, not on the shop floor.

## 1. Design mistakes

| Mistake | Why it hurts | Fix |
|---|---|---|
| Starting CAD without clear requirements | You design the wrong thing | Write measurable requirements first |
| Falling for the first idea | Misses simpler or cheaper options | Sketch at least three concepts |
| Skipping hand calculations | You trust the software blindly | Check the critical load by hand |
| Ignoring fatigue and vibration | Parts crack after thousands of cycles | Design for cyclic loads, use fillets, avoid stress risers |
| Sharp internal corners | Stress concentration and hard to machine | Add fillets and radii |
| Thinking stronger material means stiffer | All steels have about the same E | Increase section depth or add ribs |
| Using too small a factor of safety | Unknown loads cause failure | Use 2 to 3 or more when unsure |
| Over-engineering | Heavy, costly, slow to build | Design to requirements, not fear |
| Not considering thermal expansion | Binding, loosening, cracking | Allow for expansion, especially between different materials |
| Forgetting buckling in slender members | Collapse below yield | Check Euler buckling for long compression members |

## 2. CAD mistakes

| Mistake | Why it hurts | Fix |
|---|---|---|
| Under-defined sketches | Geometry moves unexpectedly | Fully constrain sketches |
| Fillets and chamfers added early | Rebuild errors when editing | Add them last |
| Referencing edges and faces that may change | Broken references | Reference planes, origins, and sketches |
| One giant sketch | Impossible to edit | Use several simple sketches |
| Unnamed features and parts | Nobody can follow the model | Name key features and use a naming scheme |
| Ignoring units | Parts come out 25.4 times wrong | Set units at the start (mm, g, s) |
| Wrong scale in STL for simulation or print | Robot or part is 1000 times too big or small | Check mm versus m on export and import |
| Not saving versions | Lose work or cannot go back | Save revisions and use cloud or Git backups |
| Moving CAD files outside the CAD program | Assemblies lose references | Use Pack and Go or Copy Project |
| Overusing mates in assemblies | Over-defined assembly and slow rebuild | Mate only what you need |
| Interferences not checked | Parts collide in real life | Run interference detection |
| Model looks fine but is not buildable | Cannot be machined or assembled | Review with DFM and DFA rules |

## 3. Drawing and tolerance mistakes

| Mistake | Why it hurts | Fix |
|---|---|---|
| Tolerances too tight everywhere | Cost explodes | Tolerate only critical features |
| Tolerances too loose on fits | Parts rattle or do not assemble | Choose fits from function (see 04) |
| Chain dimensioning | Errors accumulate | Dimension from a datum |
| Missing or duplicate dimensions | Machinist has to guess | Check each feature has exactly one dimension |
| No material, finish, or general tolerance | Wrong part is made | Fill in the title block and notes |
| Datums that do not match assembly | Part passes inspection but does not fit | Choose datums from mating features |
| Not checking tolerance stack-up | Assembly fails when parts vary | Do worst case or RSS check on critical gaps |
| Using GD&T you do not understand | Confusing or wrong requirements | Learn the basics or use plain dimensions |

## 4. Material and manufacturing mistakes

| Mistake | Why it hurts | Fix |
|---|---|---|
| Choosing material without checking availability | Delays and extra cost | Check stock forms and suppliers |
| Ignoring galvanic corrosion | Joints corrode in wet conditions | Isolate dissimilar metals |
| Using plastics for long-term loads without checking creep | Parts deform over time | Use lower stress or choose a better material |
| Printing parts in a bad orientation | Layers split under load | Orient layers along the load path |
| Forgetting 3D print clearances | Parts will not fit together | Add 0.2 to 0.3 mm for sliding fits and test |
| Thin walls and tiny features | Break or cannot be made | Respect minimum wall thickness for the process |
| Deep narrow pockets | Tool breaks or deflects | Keep depth under about 4 times tool diameter |
| Tiny internal radii in machined parts | Needs tiny, slow tools | Use generous radii |
| Sheet metal holes too close to bends | Holes deform | Keep holes at least 2 times thickness plus bend radius away |
| No draft on cast or molded parts | Part sticks in the mold | Add 1 to 3 degrees of draft |
| Non-uniform wall thickness in cast or molded parts | Warping, sink marks, cracks | Keep walls uniform or transition gradually |
| Welding without distortion plan | Frame ends up twisted | Weld in sequence, machine after welding if precision is needed |
| Skipping deburring notes | Sharp, dangerous edges | Add "break all sharp edges" note |

## 5. Fastener and assembly mistakes

| Mistake | Why it hurts | Fix |
|---|---|---|
| No room for a wrench or screwdriver | Cannot assemble | Check tool access in CAD |
| Bolts loaded in shear instead of using pins | Threads wear, bolts loosen | Use dowel pins for location and shear |
| No locking in vibration | Fasteners back out | Use nylon-insert nuts, thread locker, or spring washers |
| Holes too close to the edge | Edge tears out | Keep centre at least 1.5 to 2 times hole diameter from edge |
| Threads directly in soft plastic or thin aluminium | Strip easily | Use inserts, nuts, or thicker sections |
| Too many different fastener sizes | Inventory and assembly mess | Standardise on a few sizes |
| Parts can be assembled backwards | Mistakes in assembly | Add asymmetric features or locating pins |
| Not planning for maintenance | Parts cannot be replaced | Design for easy access |

## 6. Process mistakes

| Mistake | Fix |
|---|---|
| Ordering parts without a design review | Do a review with a checklist or a friend |
| Not talking to the manufacturer | Ask early about capability and cost |
| Skipping a prototype | Print or cut a cheap version first |
| Changing design without updating drawings | Use revision control |
| Not recording decisions | Keep a design log |
| Leaving everything until the deadline | Plan time for ordering, delivery, and rework |
| Only testing the ideal case | Test misuse, overload, and extreme conditions |


- [ ] BOM complete with standard parts
- [ ] Files saved with revision and backed up
