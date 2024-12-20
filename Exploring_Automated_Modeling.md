# Exploring Automated Modeling

Several software tools can aid in the reconstruction of broken parts. Fusion 360, Blender, and Meshmixer offer various approaches, but **Fusion 360** was chosen for its educational license and powerful capabilities. The explored alternatives include:

**1.	Autodesk Fusion 360** – Alongside plugins like Automated Modeling and Netfabb, Fusion 360 is a robust modeling software that, paired with Netfabb, can analyze and repair broken parts. The combination leverages cloud-based AI tools for automatic repair and reconstruction.

**2.	Meshmixer** – Developed by Autodesk, Meshmixer is a free tool that allows users to edit, repair, and optimize meshes. It includes features for automatic repair of 3D models, making it suitable for reconstructing broken parts.

**3.	Materialise Magics** - This software is tailored for additive manufacturing and offers advanced mesh repair tools. It can automatically fix issues with 3D models, ensuring they are ready for printing or further processing.

**4.	ZBrush** - Primarily used for digital sculpting, ZBrush offers powerful tools for repairing and reconstructing 3D models. It uses Dynamesh to fill gaps and correct topology, which can be particularly useful for broken parts.

**5.	Geomagic Design X** - This software specializes in converting 3D scan data into CAD models. It offers automated and semi-automated tools for reconstructing damaged or incomplete components.

**6.	Blender with Add-ons** - Blender is an open-source 3D modeling tool that, with the aid of various add-ons, can perform mesh repair and reconstruction. Add-ons like Mesh Repair and 3D Print Toolbox enhance its capabilities in this regard.

**7.	RepairShop by trinckle** - An online service that can take STL files and provide repair and optimization services. It's user-friendly and suitable for those who need quick fixes to broken parts.

# Fusion 360 Automated Modeling
Fusion360’s Generative Design is a multi-objective design exploration tool that aids the user in new ways to designing parts with geometric, manufacturability, and performance constraints. Sadly, only select “tokens” for use are available through the educational license as well as a 14-day free trial. This being said, one feature that is free to use using the student license is the *Automate* feature within the Fusion360’s *SOLID* workspace. This tool has an automated modeling feature similar to the one used in Fusion 360’s Generative Design workspace.

  <img src="https://github.com/user-attachments/assets/e94892bb-64dc-4134-b1cf-2b4e060e06e9" alt="Preview of automated modeling feature within Fusion 360" width="1080"/>
</p>
                                      
                                          Preview of automated modeling feature within Fusion 360
                            
Upon selecting this tool, the automated modeling tab will open, consisting of an *Inputs* section as well as and an *Alternatives* section.
Within the inputs section, the user will have the option to select the faces within the model that are meant to be connected/ reconstructed, as well as bodies to avoid. In the operation tab, the user can also select whether the AI generated solution should be constructed as a new body or as a component.
 
  <img src="https://github.com/user-attachments/assets/0e47175e-199f-480a-a14f-947ab78eee22" alt="Preview of features within automated modeling tab" width="1080"/>
</p>

                                              Preview of features within automated modeling tab

After selecting surfaces to connect, the user will receive several (up to 6) alternatives on a generative design. The user can alternate the overall volume of the generated solution by a slider found at each generated alternative. This tool generates two main types of connection which will be viewed in detail in subsequent sections. One type of connection is a smooth connection, whereas the second one is a sharp connection. Alternatives 1 and 2 give out a smooth connection in most cases, whereas Alternatives 3 to 5 generate a body with a sharp connection.

 <img src="https://github.com/user-attachments/assets/158cf8ac-a044-44d9-9c8f-cf542928edd0" alt="Preview of AI generated alternatives for a demo of a broken piece modeled in Fusion 360" width="1080"/>
</p>

                            Preview of AI generated alternatives for a demo of a broken piece modeled in Fusion 360

Our goal was to fully test the limits of this tool in order to find out what it can do well, as well as areas where it encounters difficulties within reconstructing a part for our intended use case. For that purpose, we ran several scenarios of potential types of broken pieces a user might encounter with increasing levels of complexity, taking a look at each generated alternative. For the component which would be tested, we decided to go with a model similar to the broken lamp piece at the beginning of this report, due to the possibility of increasing the complexity of AI  alternative solutions generated by the automated modeling tool.

 <img src="https://github.com/user-attachments/assets/0e236f64-9ce2-451f-8bff-f1924b0a23d3" alt="CAD model of a component to be tested (lamp piece)" width="1000"/>
</p>

                                              CAD model of a component to be tested (lamp piece)
