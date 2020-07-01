#  Design & 3D Print Topographic Map Models
![Workshop image](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/workshop.PNG)
A design workshop to learn how to model and print topographic maps in 3D.

## Dependencies
1. Generate a Terrain Map on [Terrain party](http://terrain.party/).

2. Download [Blender](https://www.blender.org/download/).
3. Download [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360/overview#banner).
4. Download the Slicing Software [Cura](https://ultimaker.com/en/products/ultimaker-cura-software).

## What is 3D printing?
 It is the process of taking a 3D digital model and making it a physical object, by forming successive layers of material under computer control.

## What can 3D printing be used for?
- Industrial Production
- Build Proof Of Concept (POC)
- Rapid Prototyping
- Marketing Samples
- Education
- Art
- Fashion
- Hobbyists

## What is topographic mapping?
A **topographic map** is a type of map characterized by large-scale detail and quantitative representation of relief, usually using contour lines. 

![topographic map](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/topographicmap.PNG)

## What can a topographic model be used for?
- A plastic model of terrain for school education
- A small-scale version of a national park
- A model that shows the overview of a real-world race track
- A tiny version of a mountain you climbed in the past as a souvenir. 

## Steps

1. Go to [terrain.party](http://terrain.party/) and choose location on StreetMap view > In Map View switch to USGS shaded relief view > Download the map as a zip file.

![step 2](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step2.PNG)

2. Open Blender > Go to Create > Plane > Open Modifiers > Select Subdivision Surface and change to simple design. Edit the subdivisions by increasing the View and Render options to control the level of detail in the plane through subdivisions.

![step 3](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step3.PNG)

3. Go to modifiers again > Displace the plane in order to add an image > Add new texture > Open image (merged) from folder saved from terrain.party.

![step 4](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step4.PNG)

4. Choose Image colour space > Select Linear.

![step 5](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step5.PNG)

5. Click modifiers > Adjust the Subdivisions again according to the level of detail required for the map until satisfied > Adjust the strength to control elevation of the map > Go to File > Export the model as an **.obj file**.

![step 6](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step6.PNG)

6.Launch AutoDesk Fusion 360 > Insert  > Insert Mesh > Select the .obj file saved from Blender in the previous step > Change unit type to centimeter > Centre the model > Flip Up Direction to have model Vertical with a -180˚ shift for the model to appear top side up for printing later on > Press OK. 

![step 8](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step8.PNG)

7. Go to Create > Select create form > Select the model > Go to utilities > Select Convert > Convert type should be set to “Quad Mesh to T-Spline” so that the imported mesh model can be converted to a T-spline model with a smooth surface > Press OK and wait for the model to process for 1-2 minutes > Press Finish Form.

![step 9](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step9.PNG)

8. Next the model requires a base. Go to Sketch > Select any shape for the base. An ellipse is shown base example is shown below. Press the shape > Select the plane to draw on > Draw the shape encompassing all parts of the model that are desired > Press Stop Sketch.

![step 10](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step10.PNG)

9. Next select the model and drag it above the shape depending on the desired thickness of the base > Press OK. 

![step 11](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step11.PNG)

10.  The base has to be extruded into the model > Select the base shape > Go to Create > Select extrude > Extend “To object” and then select the object which is the model > Press OK. 

![step 12](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step12.PNG)

11. Select the base shape again and Extrude > Change operation to “Intersect” > Change distance to a negative value until the entire model is intersected (shown by yellow region) > Press OK. 

![step 13](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step13.PNG)

12. To add text to the base, the XZ plane must be offset so that text does not get stuck inside the model since the model is centered. Go to Origins >  Right click the XZ plane and Select Offset Plane > Offset plane so that is in front of the model > Press OK.

![step 14](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step14.PNG)

13. To add text, Select the offset plane and Go to Sketch > Text > Add the text and rotate the text on the base according to the model > Adjust “Height” to change the size of the text > Press OK > Stop Sketch. 

![step 15](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step15.PNG)

14. Next select the text > Right click and Extrude > Start “from object” > Operation “cut” > Negative distance for extruding the text inside the base > Press OK.

![step 16](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step16-1.PNG)

15. The 3D topographical map model is now ready to be exported for 3D printing. Go to Make > Untick “send to 3D print utility” > Change refinement to “Medium” or “Low” as “High” takes time to render and has a larger file size. > Press OK to save as an .stl file. 

![step 22](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step22.png)

16. Open CURA and open the .stl file saved in the previous step. Here the 3D model can be scaled and rotated as well print settings can be altered. Slice the model and export to SD card for printing.

![step 23](https://github.com/ayeshaf9/3d_topographic_maps/blob/master/Images/step23.png)

## Credits

View the [tutorial](https://www.youtube.com/watch?v=bSNy9iUqDbI) made by Joe Brewer.
