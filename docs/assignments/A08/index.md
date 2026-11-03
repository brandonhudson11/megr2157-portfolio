# A8 – Gears

## Objective

Design a gearbox that can be easily assembled and disassembled using spur gears with a gear ratio of 24:9, as specified in the provided resources. The gearbox must deliver an output torque of 1.25 in-lbf at a relative speed of 1100 rpm. The input and output shafts must each be 1 inch long, with diameters of 0.125 inches for the input pinion shaft and 0.25 inches for the output gear shaft. Use the appropriate empirical equations from the Machinery’s Handbook to complete the design. The main components to consider are the shafts and journal bearings, ensuring the gearbox is properly supported and functional.


## Part 1- Shaft Design

For this part of the assignment, I was responsible for designing the gearbox’s input and output shafts using the specified dimensions and design requirements.

<img width="756" height="1002" alt="0" src="https://github.com/user-attachments/assets/1ea689ac-f478-4547-830e-1e2a2b5137fd" />


## Part 2 Journal Bearing

For this part of the assignment, the objective was to calculate the PV value, compare it with the values provided in the reference table to select an appropriate material, and determine the required thickness.

<img width="771" height="1002" alt="0" src="https://github.com/user-attachments/assets/4558faee-6179-4329-85bb-633998a3e012" />


## Part 3 Sketch

Before creating the CAD model, I made a preliminary sketch of the top and bottom sections of the gearbox. This provided a starting point for the housing design and helped determine the placement of the gears, shafts, bearings, and mounting holes. I then used these sketches as a reference when developing the individual 3D components.

<img width="1908" height="964" alt="0" src="https://github.com/user-attachments/assets/ec37677f-ee8a-4a9e-bd2b-ed1d29e79659" />


## CAD

I downloaded the selected gears and bearings from McMaster-Carr and imported their CAD models into my design. This allowed me to work with their exact dimensions and shapes, making it easier to design the shafts and gearbox housing to properly accommodate each component.

<img width="415" height="253" alt="Screenshot 2026-11-03 070556" src="https://github.com/user-attachments/assets/d8aba007-7e04-4ef9-984c-c9c3459e4896" />

## Output Shaft

The next step in the design process was creating the input and output shafts using the dimensions provided in the assignment. I began by creating a circular sketch for each shaft, making sure to use the correct diameter for the input and output sides. Once the sketches were complete, I used the extrusion feature to give both shafts their required length of 1 inch. After establishing the basic shaft geometry, I added a 45-degree chamfer to the ends that would connect to the gear hubs. This angled edge provides a smoother lead-in when inserting the shafts into the gears and helps make the press-fit assembly process easier. I also made sure the shaft dimensions and features matched the selected gear components so that everything would fit together correctly when the gearbox was assembled.

<img width="599" height="359" alt="Screenshot 2026-11-03 061530" src="https://github.com/user-attachments/assets/2a31249a-7757-4948-90bd-99073139ab54" />

<img width="797" height="350" alt="Screenshot 2026-11-03 061508" src="https://github.com/user-attachments/assets/162ef3c1-ab73-460a-9c7c-c80bb9e78771" />

## Input Shaft

<img width="674" height="364" alt="Screenshot 2026-11-03 061809" src="https://github.com/user-attachments/assets/2223667f-13be-48ce-bad5-b4174d7ae1b7" />

<img width="723" height="156" alt="Screenshot 2026-11-03 062134" src="https://github.com/user-attachments/assets/740b4af6-e952-48bf-8bfb-5043d637ef11" />

## Gearbox

After completing the shafts and selecting the necessary components, I moved on to designing the gearbox housing. I began with the bottom half of the housing by creating a rectangular sketch measuring 4 inches by 3 inches. I then extruded the shape to create enough internal space for the gears and shafts to rotate without making contact with the housing. Once the main shape was established, I used construction lines and measurements to locate the center of the housing and calculate the correct offsets for the shaft openings. I used these reference points to position the holes accurately so that the shafts would line up properly with the gears inside the gearbox. I repeated this process when creating the top half to ensure that both sections would align correctly when assembled. Finally, I added mounting holes around the outer edges of the housing. These holes allow the top and bottom sections to be fastened together with screws or bolts, keeping the gearbox securely assembled while still allowing it to be taken apart when maintenance or adjustments are needed.


<img width="552" height="323" alt="Screenshot 2026-11-03 070001" src="https://github.com/user-attachments/assets/2fc68440-e44f-4955-9824-fdfc3dd2b88d" />

<img width="512" height="313" alt="Screenshot 2026-11-03 070114" src="https://github.com/user-attachments/assets/b6c6cb82-5222-4892-a79c-0136d39fecf5" />

## Final Part

<img width="434" height="361" alt="Screenshot 2026-11-03 073117" src="https://github.com/user-attachments/assets/b518025f-5d1e-4c09-856b-ad94b54551ac" />

Once I finished modeling both pieces of the gearbox housing, I moved on to putting the entire assembly together. I started by positioning the bearings inside the housing and making sure they were seated in the correct locations. From there, I inserted the input and output shafts through the bearings and attached the selected spur gears to their respective shafts. I had to pay close attention to the placement of each component to ensure the gears lined up correctly and had enough space to rotate without hitting the inside of the housing.

After getting the main components in place, I applied assembly constraints to keep everything properly positioned. I also set up the gear connection to maintain the required 24:9 ratio, allowing the input gear to drive the output gear in the correct direction. Since the gears mesh directly with one another, their rotation directions are opposite. Once everything was aligned, I attached the top half of the housing to the bottom half and checked that the screw holes matched up.

To finish the assembly, I checked the movement of the shafts and gears to make sure there were no clearance issues or unwanted contact between parts. I also wanted to verify that turning the input shaft would cause the output shaft to rotate as expected. This final assembly process brought all the individual components together into one gearbox design that can be taken apart and reassembled when needed.

## Lessons Learned

Throughout this project, I learned how important it is to consider both the individual components and how they work together when designing a mechanical system. One of the biggest things I took away from this assignment was the importance of using accurate measurements and dimensions when creating CAD models. Using the actual CAD files from McMaster-Carr made the design process easier because I could build the shafts and gearbox housing around the selected gears and bearings instead of estimating their sizes.

I also gained a better understanding of how shafts, spur gears, and journal bearings work together in a gearbox. Calculating the required dimensions, selecting materials based on the PV value, and determining the proper thickness helped me connect the calculations from class to an actual mechanical design. I learned that even small dimensional differences can affect how components fit and operate once everything is assembled.

Another important lesson was the value of planning before starting the CAD model. Creating initial sketches helped me visualize the housing and determine where each component needed to be located. I also learned how important proper alignment and clearance are when assembling gears and shafts. If the components are not positioned correctly, the gears may not mesh properly or the shafts may experience unwanted interference.

Overall, this project gave me more experience with mechanical design, CAD modeling, component selection, and assembly. It helped me understand the amount of planning and attention to detail required to design a functional gearbox. I also learned that designing a part is only one step of the process; making sure all the parts fit together, operate correctly, and can be assembled and disassembled is just as important.

## Files

<a href="https://drive.google.com/drive/folders/1253am3DxTlZm73rnt-mUodxzAsZr4yRw?usp=drive_link">A8</a>










