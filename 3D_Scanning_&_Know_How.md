# 3D Scanning Software & Know-How

## This section explains the tools used for scanning the broken parts, specifically focusing on the Revopoint MINI 2 3D Scanner and the Revo Scan 5 software, as well as relevant know-how accumulated throughout the research.

The used scanning equipment for during the research was the Revopoint MINI 2 3D Scanner. This scanner is a 912$ blue light scanner with precision of up to 0.02 mm, 16 fps scanning speeds and Wi-Fi 6/ USB Type-C connectivity.

The scanner comes with its own Revo Scan 5 proprietary software which is available for PC, Android and IOS devices. After installing the software (in this case for PC), the scanner can be connected to the PC using the Type-C cable, after which 2 screws need to be tightened, and a Type-A end connected to the PC (with PD). 

<p align="center">
  <img src="https://github.com/user-attachments/assets/bd319512-5726-4400-ae5e-a682a0972369" alt="Centered Image" width="1080"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/fe0a0f83-cb2a-40fa-9cfe-e969c6506661" alt="Centered Image" width="1080"/>
</p>

                                  Graphical representation of connecting PC to Revopoint MINI 2D

Subsequently, the user will be required to manually calibrate the scanner via the settings icon. The user is given instructions directly via the Revo Scan 5 software as to how to correctly calibrate the scanner. After successful calibration, the user will have the option to create a new project, and will be greeted with the following interface:

<p align="center">
  <img src="https://github.com/user-attachments/assets/2bfd08ba-1b24-4f04-bc26-629d21dbb102" alt="Centered Image" width="1080"/>
</p>

                                                             Revo Scan 5 UI

There are a total of 14 option available on the navigation bar: 
**(0)	Scan
(1)	One-click-editing;
(2)	Fusion;
(3)	Isolation;
(4)	Overlap;	        
(5)	Smooth;
(6)	Simplify; 
(7)	Mesh;
(8)	Isolation;
(9)	Fill Holes; 		 
(10)	Smooth;
(11)	Simplify;
(12)	Texture;
(13)	Merge;
(14)	Export**
On the left-hand side, the user will see a live feed of the object that is being scanned with options to adjust the exposure of the depth camera and RGB camera. On the right-hand side, the user will see an indicator bar regarding the distance from the scanner to the scanned object, ranging from too near, excellent, good, far, too far. The aim of the user should be to always position the object within the excellent range (between 120-250mm). Depending on the selected tool from the navigation bar, multiple options will be displayed on the right-hand side. The user can initiate a scan using the start option, cancel it and click complete scan after the table makes (at least) one full rotation. 

Keeping in mind that this whole process should be easily achievable for a user with little to no CAD experience, our aim is for the user to result to only the **(1) one-click editing tool** along with **(9) fill holes tool** (if there are any areas in which the point-cloud model is not connected as intended. 

## Revo Scan 5's one-click processing
Revo Scan 5’s one-click processing feature automatically performs fusion, meshing, and texturing (if a color scan was done) based on the best detected setting for the point cloud.

<p align="center">
  <img src="https://github.com/user-attachments/assets/9adfa22e-b9c1-496a-bca7-ea28dc817147" alt="Centered Image" width="720"/>
</p>

                                                      Preview of one-click editing tool
## Revo Scan 5's fill holes tool
After the (1) one-click processing has finished, there still may be some imperfections in the form of holes in the mesh which may be the result of the angle at which the scan was taken or the overexposure due to environmental lightning. In such cases, the user should opt to using the (9) fill holes tool. The detected holes will be detected with a red outline, after which the user should select in and proceed to fill the holes. Depending on the location of the hole, the user should select the *plane* option for holes on flat surfaces or the *curve* option for holes on curved surfaces:

<p align="center">
  <img src="https://github.com/user-attachments/assets/857385da-accb-426b-ba7c-af2854c95760" alt="Centered Image" width="720"/>
</p>

                                      Preview of model before and after use of hole filling tool

## Revo Scan 5 Shortcuts

<p align="center">
  <img src="https://github.com/user-attachments/assets/f6861145-f5ba-4d29-b0ec-294717f2deae" alt="Centered Image" width="1080"/>
</p>

## 3D Scanning Know-How
Based on several scans performed on different types of objects, we concluded that:

•	In the manual, the stated distance between scanner and scanned object should be 120-250mm. In actuality, this can be changed in the software between 120-320mm. Regardless, the optimal scanning distance is usually at least beyond 150+ millimeters.

•	Feature-rich objects (associated with complex geometry) is usually easier to scan since it has its own unique reference points for the scanner to track (edges, contours, curves, etc.)

•	Featureless objects (associated with simple geometry) requires the placement of a *marker topper* for successful scanning if the objects fits within the turntable.

•	Featureless objects which do not fit on the *marker topper* can be placed on a larger rectangular marker topper (but in this case, the object needs to be scanned by hand, or should be plastered with randomly arranged large markers all around its surface)

•	Scanning transparent objects, black objects, shiny or reflective objects is always problematic without proper pre-treatment. These kind of objects should be sprayed with scanning spray (or painted very neatly as to not let dry paint change the overall shape of the object) or plastered with markers as mentioned above (although it is always recommended to use scanning spray when encountering such objects)

•	Within the software, the (1) one-click-editing option works better, the better the external scanning conditions are. (having an enclosure including black/ reflective background, right distancing, correct placement of the object on turntable, as well as low external glare due to lighting)

•	Unwanted scanned areas can be removed with the (3) isolation tool. When doing the process manually, it is recommended to do this in the *Fused* (point-cloud) stage rather than the *Meshed* stage.

•	At the end of each scan, it is always necessary/ recommended to check for holes. If ones are found, the user should use the (9) Fill Holes tool. If an undesired opening is found, it needs to be selected it using right-click (selected area should change color after being selected from red to green) and proceed with the command.

•	Before exporting, it is almost always necessary to (11) Simplify the mesh (in most use cases 100%, or multiple simplifications), as the exported -.stl files are overly detailed/ complex for smooth follow up design/ reconstruction in any CAD software.

•	-SolidWorks (SW) experiences difficulties (crashes) with certain imported -.stl files even with simplification of the mesh (reducing the number of surfaces), hence it is recommended to import the files in Fusion360 or any other similar CAD software. 

•	If no modification is required, the user can directly open the -.stl file in the desired slicing software (Cura, Simplify3D, etc.)
