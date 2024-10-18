# Logic Diagram

For the purpose of simplifying and identifying key stages within the process pipeline, a **logic diagram** can be used for illustrating the multiple outcomes based on the part the user is scanning.

<p align="center">
  <img src="https://github.com/user-attachments/assets/fb4d32da-1a89-4354-808b-bab022c535bf" alt="Centered Image" width="1000"/>
</p>


                           Logic Diagram with different approaches (outcomes) based on the broken component 

Based on the logic diagram, the user can fix his broken component in a total of seven ways which at first may seem similar, but are all different in their own respective way. Generally, the further downwards the user goes down the logic diagram, the more time it takes to fix a component and the more complex these fixes get with respect to the necessary CAD knowledge and 3D scanning procedure.

**1. Downloading the file & printing** - This is by far the simplest and most desirable outcome for a user. (if the part exactly corresponds to that of the user’s needs). Due to the ever-growing maker community, the file may already be available online (Thingiverse, GrabCAD, MyMiniFactory, etc.). It is worth to note that in most cases, the most suitable file format for 3D printing is an stl. (stereolithography) file, hence the user should almost always (expect for when additional modeling is required) look for this format when searching online.

**2. 3D scanning after healing & printing** – If the part is missing geometry which can be healed (using clay, glue, epoxy, etc.), the user can “heal” this geometry and proceed with scanning it in its “healed” state. The corresponding scan should be feasible for 3D printing a repaired model of the broken component. 

**3. Designing in CAD and printing** – If the missing geometry cannot be healed using the methods above, the user should heal the damaged section of the component in CAD (after 3D scanning the object). 

**4. 3D scanning and & printing**  – If the part is complete and not missing any geometry, the user can proceed to 3D scan and print the part if:
a)	it is made up of geometric shapes and there are no intricate details which require high accuracy
b)	it is flat, thin, or very small and there are no intricate details which require high accuracy 


**5.	3D scan, remodel details & print** - If the part is complete with simple geometry, yet intricate details (which the 3D scanner may or may not capture), it is recommended for the user to remodel the details after scanning the part and print the newly redesigned component.

**6.	Designing in CAD using photo references for critical points** - This outcome is quite similar to outcome (5.) with the only difference being the inability of a 3D scanner (or any other image capturing device) to capture specific contours, curves, points within the component as opposed to small details (protrusions). Here, the user should take images of orthographic projections  of the object and use them as reference images when modeling in CAD as a reference for relevant angles and dimensions.

**7.	Designing in CAD from scratch with accurate measurements** - If the part does not have any critical curves, but is complex to the point where a scanner is unable to capture key dimensions or features with respect to the intended use of the part, it is recommended for the user to use measuring tools (digital calipers, angle gauge, etc.) to accurately measure the dimensions and model them in CAD. This outcome is the least desirable within the logic diagram as it requires a user with substantial CAD/ modeling knowledge and experience. 

With the goal of making this process as simple as possible for the user, we aim to automate as many steps (outcomes) of this process as possible.
