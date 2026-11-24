# A11 – Motor Selection

## Project Introduction
This project focuses on designing the motorized drive and support structure for a benchtop tensile tester with a 2 kN load capacity. The tester uses two lead screws to move a crosshead and pull a test specimen. By applying tension, the machine can help show how a material responds to load and how much it stretches before it yields or breaks.
Our team will select a motor, design motor mounts, choose or design a coupler, and develop a stable frame and specimen clamps. The design must support the required load with a safety factor of 4, keep the specimen and crosshead aligned, and fit within a practical bench-top size. The lead screw system must also meet the required travel-speed range of 1–50 mm/min and have a minimum lead screw length of 18 inches.
The final work will include CAD models of the engineered parts, supporting sketches and free-body diagrams, design calculations, and a bill of materials with estimated costs. This assignment documents the design process as well as the final design, including decisions, mistakes, and lessons learned.

<img width="245" height="334" alt="image" src="https://github.com/user-attachments/assets/c9f3c550-b344-4ed4-bf34-805d728e3ac9" />

## Motor Selection and Attachments -  Bryson Bare
We selected the MOONS’ AM34HD2403-07 hybrid stepper motor because the tester must move slowly while pulling a high load. The stepper motor can provide controlled movement at low speeds, and this model has a listed holding torque of 9.4 N · m. We assumed that one motor would drive each lead screw, so each screw carries half of the tester's 2 kN load. The holding torque helped us identify a candidate, but we use the speed-torque curve to check the torque while the motor is running.


<img width="351" height="392" alt="image" src="https://github.com/user-attachments/assets/d32d8b1a-966b-4d05-868e-475fbc5364ab" />

<img width="358" height="239" alt="image" src="https://github.com/user-attachments/assets/6ec1ebbd-4f45-4076-9fc5-4ef84ec884e8" />

## Motor Mount (Bryson)
After selecting the motor, we needed to design a motor mount to hold it. We designed a four-bolt motor mount to attach the motor securely to the tester frame. We calculated the force on each bolt from the motor’s reaction torque, checked the plates' bearing stress, and found the minimum thickness needed to meet the allowable stress. Because the minimum thickness was so thin, we selected a 10mm plate for a more practical and rigid mount. I also had to account for the thickness of the top of the frame when choosing the bolt lengths that will hold the mount to the frame. I chose 20 mm because the mount is 10 mm thick and the frame is 10 mm thick.

<img width="245" height="309" alt="image" src="https://github.com/user-attachments/assets/d2f1b986-0947-4695-bc15-4ad6b4f472e0" />

## Coupling Design (Bryson)
We selected the McMaster-Carr 2764K425 coupler because its 14mm and ½ in bores match the motor shaft and the lead screws nominal diameter. This would connect the motor to the lead screw. The coupler is rated for 89 in*lbf, which is higher than our design torque. Its speed rating also exceeds the leads screws max speed. The flexible discs help accommodate any slight misalignment between the shafts. For a secure fit, the screw end will need to be a smooth section where it enters the coupling. 

<img width="360" height="389" alt="image" src="https://github.com/user-attachments/assets/264f410c-926b-4cf0-84ec-a0b69a38d75b" />

## Total time Bryson: 5 hrs

## Analyze and design a Frame - Nolan

For analyzing the frame, I was tasked with running an FEA for the top of the frame and the vertical components of the frame, to ensure the frame will have very low deflections. 

Top of the frame

For the top of the frame, I loaded up the CAD assembly for our frame and started a new study. I then measured from the outside edge of the crosshead to the center of the leadscrew hole. 

<img width="362" height="227" alt="image" src="https://github.com/user-attachments/assets/c02d9711-ada1-4b17-983a-4656945b3407" />

I used this measurement to determine where to put the 1kN forces on the top of the frame. I also added this distance to it

<img width="362" height="233" alt="image" src="https://github.com/user-attachments/assets/be17d468-0a6d-4b1f-aa82-cc97bd258ae6" />

I then used this measurement to create a point on the surface of the beam that I could refer to when placing a force down. This did not work, which led me to having to sketch circles around the point. This also did not work, so I had to split the geometry for the face of the beam with the circles I sketched as seen here:

<img width="360" height="233" alt="image" src="https://github.com/user-attachments/assets/888c9980-ee46-4eaf-9523-75c1b8c4607d" />

I then realized that after a 50/50 chance, I did this on the side that was underneath for the assembly, leading me to having to redo this again. After all of this which took around an hour to learn how to put a single force on this one specific location, I had this:

<img width="248" height="323" alt="image" src="https://github.com/user-attachments/assets/0ba2e264-9d79-42ba-90dc-f6e95dd80887" />


I then realized although not stated in the canvas page, the analysis was supposed to be done for just the beam and not the whole frame and crosshead together. I created these forces and fixtures:

<img width="361" height="236" alt="image" src="https://github.com/user-attachments/assets/c4e36f25-6e1b-4a4f-90d6-37d7ae0b6919" />

After applying a material and running the study, I was left with these results:

## Von Misses

<img width="248" height="336" alt="image" src="https://github.com/user-attachments/assets/96e49d51-f650-4b73-9bfb-e98608c14565" />

## Safety Factor

Safety factor was 7.7 everywhere.

This safety factor was well above the project's given 4 value, so I decided it was good to move on to the Side of the frame.

## Vertical Frame

To check the vertical frame, I ensured that the frame could withstand the 1000N from the leadscrew, as well as the torque from the lead screw (calculated to be 16.6 N*m). Here are my forces and constraints:


<img width="371" height="233" alt="image" src="https://github.com/user-attachments/assets/5a0f1b84-ff37-4804-836a-1a9eecd6cece" />


I then ran the study and got these results:

## Von Misses

<img width="379" height="272" alt="image" src="https://github.com/user-attachments/assets/ce367206-d899-45de-a19d-fdb913e40214" />

<img width="377" height="275" alt="image" src="https://github.com/user-attachments/assets/dca0e987-cfa9-4e9a-b748-8ef9249839f2" />

I got back a calculated safety factor of 12. This was way above the safety factor of 4, so I decided to deduct that this frame was built strong enough to not need any changes to the overall design. 


## Total time Nolan: 2 hours 

## Design floating Bearing Mount - Brandon Hudson

I first started designing the motor mount with the dimensions Bryson came up with in the math above. Below is the sketch of the motor mount. 

<img width="430" height="316" alt="Screenshot 2026-11-23 200152" src="https://github.com/user-attachments/assets/9b57c2e0-2daf-4411-909d-08e42961c2c7" />

After doing the sketch I completed the extrude which was a total of 10mm. I then created the 4 holes on the mount and dimensioned them to the correct dimensions given to me by Bryson.  Below is the motor mount after this extrude and the holes inserted. 


<img width="542" height="368" alt="Screenshot 2026-11-23 202241" src="https://github.com/user-attachments/assets/e48c825d-ada6-4ac9-917c-52024748173f" />

After completing the extrude and holes I finished up the motor mount. Below is the final product of the motor mount. 


<img width="464" height="314" alt="Screenshot 2026-11-23 204523" src="https://github.com/user-attachments/assets/fac62a38-6d32-4b7c-984f-fe568c3b536b" />

I then moved onto the assembly by downloading the couplings, motor, and screws needed to fully assemble the motor and frame. I got all the parts needed and began assembling the finished product. Below is the final assembly. 

<img width="314" height="353" alt="Screenshot 2026-11-24 005830" src="https://github.com/user-attachments/assets/b349471b-dd4e-4078-bc59-e2681d51c43b" />

<img width="337" height="344" alt="Screenshot 2026-11-24 010018" src="https://github.com/user-attachments/assets/ae4535c6-3d1a-4fe5-a23d-c7b84e01bd51" />

## Bill of materials and labor costs - Brandon Hudson

Below is the bill of materials.

| Item # | Quantity | Name | Cost/item | Cost | Link |
|:---|:---:|:---|---:|---:|:---|
| AM34HD2403-07 | 2 | Hybrid Stepper Motor | $198.00 | $396.00 | [MOONS' - AM34HD2403-07](https://www.moonsindustries.com/p/am-series-standard-hybrid-stepper-motors/am34hd2403-07-000004611110010745) |
| 2764K425 | 2 | Shaft Coupling | $118.34 | $236.68 | [McMaster-Carr](https://www.mcmaster.com/2764K425/) |
| 91274A141 | 1 pack (50) | Socket Head Screw | $10.63 / 50 | $10.63 | [McMaster-Carr](https://www.mcmaster.com/91274A141/) |
| 98940A305 | 2 | Lead Screw | $28.64 | $54.56 | [McMaster-Carr](https://www.mcmaster.com/98940A305/) |
| 97790A110 | 2 | Flange Nut | $178.60 | $357.20 | [McMaster-Carr](https://www.mcmaster.com/97790A110/) |
| 92316A540 | 4 | Socket Head Screw | $10.02 / 50 | $10.02 | [McMaster-Carr](https://www.mcmaster.com/92316A540/) |
| 47065T882 | 1 | Frame | $125.63 | $125.63 | [McMaster-Carr](https://www.mcmaster.com/47065T882-47065T752/) |
| **Total Cost** | | | | **$1,190.72** | |



## Lessons Learned – Engineering Design
Throughout this project, I improved my CAD modeling and mechanical assembly skills by designing a motor mount and developing a complete assembly that included motors, couplings, bolts, and mounting components. A major part of the project involved creating and modifying CAD geometry to ensure that all components fit together accurately. I gained experience working with individual part models, positioning components, and using assembly constraints to establish the correct relationships between parts.
One of the more challenging aspects was designing portions of the supporting frame to ensure the motor would fit correctly. I had to determine the necessary dimensions, create mounting features, position holes, and modify the frame geometry to accommodate the motor mounts and other components. This required repeatedly checking component clearances, alignment, and positioning to ensure the assembly functioned as an integrated mechanical design.
This project taught me the importance of developing accurate and organized CAD models while considering how individual components interact within a larger assembly. I also gained a better understanding of how to approach custom part design, troubleshoot assembly interference, and make dimensional modifications without compromising the overall design. Overall, the project strengthened my ability to translate mechanical design requirements into detailed 3D CAD models and complete assemblies.



## Total time Brandon: 8 hours

## CAD Files- A11 - Google Drive 




























