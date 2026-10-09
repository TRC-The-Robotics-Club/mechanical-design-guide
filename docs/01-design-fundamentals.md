# Design Fundamentals
CAD Setup on Windows: SolidWorks, Fusion 360, FreeCAD, Onshape

Time needed: About 1.5-2 hours, mostly downloads and installs. Keep your laptop plugged in.

Before you start
RAM: 16 GB is recommended for SolidWorks. 8 GB works for FreeCAD, Fusion 360 and Onshape.
Storage: Keep at least 40 GB free on an SSD. SolidWorks alone needs about 30 GB.
OS: 64-bit Windows 10 or 11.
GPU: An NVIDIA or AMD graphics card with an up-to-date driver. Get the driver from nvidia.com or amd.com, or through Windows Update.
Account: Have your college email ready. It unlocks free student licenses for Fusion 360 and Onshape.
Backup: Save your important files first, just in case.

To check your specs, press the Windows key, type “System Information” and open it. It lists your RAM, processor and OS. 
Your graphics card is under Settings → System → Display → Advanced display. Free space is under Settings → System → Storage.

#### Step 1: 
Update Windows and drivers
Open Settings → Windows Update → Check for updates, and install everything.
Restart.
Update your graphics driver (NVIDIA, AMD or Intel) from the manufacturer’s website.

#### Step 2:
Make a project folder
Create a folder called CAD in your Documents. Inside it, make subfolders: SolidWorks, Fusion360, FreeCAD, Onshape and Exports. This keeps files organised and makes backups easier.

#### Step 3:
Install FreeCAD (free, open source)
Go to freecad.org and open the Downloads page.
Download the Windows installer (the stable release, not the development build).
Run the installer and accept the defaults.
Open FreeCAD and confirm the 3D view works.

#### Step 4: 
Set up Onshape (browser-based, free for students)
Install Google Chrome or Microsoft Edge if you don’t have one.
Go to onshape.com and find the Education plan.
Sign up with your college email.
Verify your email and log in.
Open a new document to test it.

#### Tips:
Use a mouse with a scroll wheel. Trackpads are awkward for 3D.
Turn on hardware acceleration in your browser settings.
Close extra tabs when working on large assemblies.
Step 5: Install Fusion 360 (free educational license)
Go to autodesk.com/education and create an Autodesk account with your college email.
Verify your student status when asked.
Find Fusion in the product list and choose the Education license.
Download the installer, run it, and sign in when prompted.
Wait for the first-launch setup to finish, which takes a few minutes.

#### Tips:

The educational license is non-commercial and renews each year.
If you see a license error, sign out and back in. Then check your subscription at manage.autodesk.com.
In Preferences, set the default modeling orientation to Z up, which is the standard in mechanical CAD.

#### Step 6:
Install SolidWorks (Windows only)
SolidWorks is paid software, but students can get it through the official student program.
Go to the SolidWorks student page on solidworks.com.
Request access using your college email.
Fill in your details and generate a reference number. It is sent to your email.
Keep that email safe, since you need the reference number to download and activate the software.
Log in at my.solidworks.com and open the Downloads section.
Download the SolidWorks Installation Manager.
Close other apps. Pause your antivirus only if the installer fails.
Run the Installation Manager and choose Individual installation.
Enter the reference number or serial number from your email when asked.
Keep SolidWorks, Simulation and Toolbox selected. Deselect extras you don’t need.
Click Install. It takes 30-60 minutes.
Restart when it finishes.

#### First run:
Set the units to MMGS (millimetre, gram, second) under Tools → Options → Document Properties → Units.
Make sure hardware acceleration is on under System Options → Performance.

#### Step 7: 
Make apps use your dedicated GPU
If your laptop has both integrated and NVIDIA graphics:
Go to Settings → System → Display → Graphics.
Add SolidWorks, Fusion 360, FreeCAD and your browser.
Open Options for each and choose High performance.
This fixes most slow-viewport complaints.

#### Step 8:
Test everything
FreeCAD: Create a new document and sketch a rectangle.
Onshape: Open a Part Studio and extrude a sketch.
Fusion 360: Create a sketch and extrude a simple block.
SolidWorks: Open a new part, sketch on the Front Plane and extrude it.

If all four work, you are done.

Working between tools
STEP (.step): The best format for moving models between CAD programs.
STL (.stl): Used for 3D printing, and also for meshes in robotics simulation.
IGES (.igs): An older exchange format, useful only if STEP fails.
Native files: Keep the original SolidWorks (.sldprt) or Fusion (.f3d) file as your master, and export copies for sharing.
Troubleshooting
Problem	Fix
SolidWorks installer fails	Re-download it, free up 30+ GB, run as administrator, and pause antivirus temporarily.
SolidWorks is slow or laggy	Update the GPU driver and set the app to High performance in Graphics settings.
Fusion 360 license error	Sign out and in, then confirm your education subscription at manage.autodesk.com.
Fusion 360 won’t launch	Restart, check for updates, and reinstall from your Autodesk account if needed.
FreeCAD 3D view is black or glitchy	Update the GPU driver and restart the app.
Onshape lags	Use Chrome or Edge, enable hardware acceleration, and close other tabs.
Not enough disk space	Run Disk Cleanup, including system files, and uninstall unused programs.
