
# CAD Setup on Windows: SolidWorks, Fusion 360, FreeCAD, Onshape

**Time needed:** About 1.5–2 hours, mostly downloads and installs. Keep your laptop plugged in.

## Before You Start

| Requirement | Details |
|---|---|
| RAM | 16 GB is recommended for SolidWorks. 8 GB works for FreeCAD, Fusion 360 and Onshape. |
| Storage | Keep at least 40 GB free on an SSD. SolidWorks alone needs about 30 GB. |
| OS | 64-bit Windows 10 or 11. |
| GPU | An NVIDIA or AMD graphics card with an up-to-date driver. Get the driver from nvidia.com or amd.com, or through Windows Update. |
| Account | Have your college email ready. It unlocks free student licenses for Fusion 360 and Onshape. |
| Backup | Save your important files first, just in case. |

### How to Check Your Specifications

| What to Check | Steps |
|---|---|
| RAM, processor and OS | Press the Windows key, type `System Information` and open it. It lists your RAM, processor and OS. |
| Graphics card | Settings → System → Display → Advanced display. |
| Free space | Settings → System → Storage. |

## Step 1: Update Windows and Drivers

| Task | Procedure |
|---|---|
| Update Windows | Open Settings → Windows Update → Check for updates, and install everything. |
| Restart | Restart your laptop after installing updates. |
| Update graphics driver | Update your graphics driver (NVIDIA, AMD or Intel) from the manufacturer's website. |

## Step 2: Make a Project Folder

Create a folder called `CAD` in your Documents. Inside it, make the following subfolders:

| Folder | Purpose |
|---|---|
| `SolidWorks` | SolidWorks project files |
| `Fusion360` | Fusion 360 project files |
| `FreeCAD` | FreeCAD project files |
| `Onshape` | Onshape-related project files |
| `Exports` | Exported CAD files |

This keeps files organised and makes backups easier.

## Step 3: Install FreeCAD (Free, Open Source)

| Step | Procedure |
|---|---|
| 1 | Go to [freecad.org](https://www.freecad.org/) and open the Downloads page. |
| 2 | Download the Windows installer (the stable release, not the development build). |
| 3 | Run the installer and accept the defaults. |
| 4 | Open FreeCAD and confirm the 3D view works. |

## Step 4: Set Up Onshape (Browser-Based, Free for Students)

| Step | Procedure |
|---|---|
| 1 | Install Google Chrome or Microsoft Edge if you don't have one. |
| 2 | Go to [onshape.com](https://www.onshape.com/) and find the Education plan. |
| 3 | Sign up with your college email. |
| 4 | Verify your email and log in. |
| 5 | Open a new document to test it. |

### Tips

| Tip | Details |
|---|---|
| Mouse | Use a mouse with a scroll wheel. Trackpads are awkward for 3D. |
| Hardware acceleration | Turn on hardware acceleration in your browser settings. |
| Browser performance | Close extra tabs when working on large assemblies. |

## Step 5: Install Fusion 360 (Free Educational License)

| Step | Procedure |
|---|---|
| 1 | Go to [Autodesk Education](https://www.autodesk.com/education) and create an Autodesk account with your college email. |
| 2 | Verify your student status when asked. |
| 3 | Find Fusion in the product list and choose the Education license. |
| 4 | Download the installer, run it, and sign in when prompted. |
| 5 | Wait for the first-launch setup to finish, which takes a few minutes. |

### Tips

| Topic | Details |
|---|---|
| Educational license | The educational license is non-commercial and renews each year. |
| License error | If you see a license error, sign out and back in. |
| Subscription check | Check your subscription at [manage.autodesk.com](https://manage.autodesk.com/). |
| Modeling orientation | In Preferences, set the default modeling orientation to Z up, which is the standard in mechanical CAD. |

## Step 6: Install SolidWorks (Windows Only)

| Step | Procedure |
|---|---|
| 1 | SolidWorks is paid software, but students can get it through the official student program. |
| 2 | Go to the SolidWorks student page on [solidworks.com](https://www.solidworks.com/). |
| 3 | Request access using your college email. |
| 4 | Fill in your details and generate a reference number. It is sent to your email. |
| 5 | Keep that email safe, since you need the reference number to download and activate the software. |
| 6 | Log in at [my.solidworks.com](https://my.solidworks.com/) and open the Downloads section. |
| 7 | Download the SolidWorks Installation Manager. |
| 8 | Close other apps. Pause your antivirus only if the installer fails. |
| 9 | Run the Installation Manager and choose Individual installation. |
| 10 | Enter the reference number or serial number from your email when asked. |
| 11 | Keep SolidWorks, Simulation and Toolbox selected. Deselect extras you don't need. |
| 12 | Click Install. It takes 30–60 minutes. |
| 13 | Restart when it finishes. |

### First Run

| Setting | Procedure |
|---|---|
| Units | Set the units to MMGS (millimetre, gram, second) under Tools → Options → Document Properties → Units. |
| Hardware acceleration | Make sure hardware acceleration is on under System Options → Performance. |

## Step 7: Make Apps Use Your Dedicated GPU

If your laptop has both integrated and NVIDIA graphics:

| Step | Procedure |
|---|---|
| 1 | Go to Settings → System → Display → Graphics. |
| 2 | Add SolidWorks, Fusion 360, FreeCAD and your browser. |
| 3 | Open Options for each and choose High performance. |

This fixes most slow-viewport complaints.

## Step 8: Test Everything

| Software | Test Procedure |
|---|---|
| FreeCAD | Create a new document and sketch a rectangle. |
| Onshape | Open a Part Studio and extrude a sketch. |
| Fusion 360 | Create a sketch and extrude a simple block. |
| SolidWorks | Open a new part, sketch on the Front Plane and extrude it. |

If all four work, you are done.

## Working Between Tools

| Format | Extension | Purpose |
|---|---|---|
| STEP | `.step` | The best format for moving models between CAD programs. |
| STL | `.stl` | Used for 3D printing, and also for meshes in robotics simulation. |
| IGES | `.igs` | An older exchange format, useful only if STEP fails. |
| Native files | `.sldprt`, `.f3d` | Keep the original SolidWorks or Fusion file as your master, and export copies for sharing. |

## Troubleshooting

| Problem | Fix |
|---|---|
| SolidWorks installer fails | Re-download it, free up 30+ GB, run as administrator, and pause antivirus temporarily. |
| SolidWorks is slow or laggy | Update the GPU driver and set the app to High performance in Graphics settings. |
| Fusion 360 license error | Sign out and in, then confirm your education subscription at [manage.autodesk.com](https://manage.autodesk.com/). |
| Fusion 360 won't launch | Restart, check for updates, and reinstall from your Autodesk account if needed. |
| FreeCAD 3D view is black or glitchy | Update the GPU driver and restart the app. |
| Onshape lags | Use Chrome or Edge, enable hardware acceleration, and close other tabs. |
| Not enough disk space | Run Disk Cleanup, including system files, and uninstall unused programs. |
