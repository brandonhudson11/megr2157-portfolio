# A10 – Lead Screw Translating System

## Lead screw Diameter (Bryson)
I began by assuming steel with a yield strength of 310 MPa for the lead screws. This gave me a starting point for estimating the minimum diameter before selecting an actual screw. Assuming the two screws share the 2 kN load equally, each screw supports 1,000 N. I used axial stress and a safety factor of 4 to calculate a minimum diameter of approximately 4.05 mm. This represents the minimum diameter needed for axial strength under my assumed material properties and helped guide my selection of a commercially available lead screw.

<img width="382" height="378" alt="image" src="https://github.com/user-attachments/assets/d5805a56-7a14-44de-814e-10879e992ce4" />

After estimating the minimum diameter, I selected a 1/2"-10 lead screw and used its dimensions to calculate the required rotational speed and torque. With 10 threads per inch and a single-start thread, the screw advances 2.54 mm per revolution. Dividing the required crosshead speeds of 1–50 mm/min by this lead gave me a rotational speed range of approximately 0.39–19.68 rpm. Using the 1,000 N load per screw, an assumed friction coefficient of 0.2, and the dimensions shown in my calculations, I obtained an estimated torque of 1,695.831 N·mm per screw. These calculations connected the selected screw’s geometry to the motion and driving torque required for the tensile tester.

<img width="332" height="372" alt="image" src="https://github.com/user-attachments/assets/5d72fef2-ddbc-407f-a198-2a2f626d2e5e" />

## Nut and Flange (Bryson)
Next, I researched McMaster-Carr’s recommended nuts and flanges for the lead screw I selected. I chose a 1/2"-10 flanged nut made from 932 bearing bronze to match the screw’s thread size. I calculated the number of engaged threads (N_t) by dividing the thread engagement length of 44.45 mm by the pitch of 2.54 mm, resulting in 17.5 engaged threads. I then used this value to calculate the thread bearing and bending stresses under the 1,000 N load per screw. Using a bronze yield strength of 124 MPa and a safety factor of 4, I calculated an allowable stress of 31 MPa. My calculated bearing stress of approximately 1.253 MPa and thread bending stress of approximately 4.229 MPa were below this value. Based on the dimensions and assumptions used in this analysis, the selected nut met the calculated thread-strength requirement.

<img width="293" height="368" alt="image" src="https://github.com/user-attachments/assets/5aa5d26e-b8de-41b4-a6b8-bba1822f8809" />


## Total time Bryson = 2.5 hrs

## Crosshead (Nolan)
The project parameters allowed us to design a crosshead with a lot of freedom. I did some research, and found that a 300mm crosshead (length) would work nicely. I then had to choose the material and thickness of the crosshead. I chose ASTM A36 steel for its high stiffness and a base width of 60mm. I then modeled the crosshead as a beam supported at both ends with a load in the center (as explained in lecture). I then found where the shear force = 0 (max moment location) and then found the max moment equation to equal PL/4. 

<img width="482" height="170" alt="image" src="https://github.com/user-attachments/assets/be4bb7d2-7cf3-4983-b0fb-f34bb65855c3" />

To perform a stress analysis, I did some algebra with the equations for stress due to bending on a beam, moment of inertia, and neutral axis to POI (c). I ended up with a derived equation for the minimum allowed height of the crosshead due to normal stress (due to bending) and plugged in the numbers to obtain a value of 15.49mm.


<img width="480" height="104" alt="image" src="https://github.com/user-attachments/assets/ba11cd43-7fa2-4c7d-b6ff-2ffba85f4df8" />

To determine the minimum height of the crosshead in terms of deflection, I first took a cut of the left hand side of the beam, and determined the moment equation in terms of x. I then integrated twice to get the deflection and slope equation, and solved to finish my derivation of max deflection for the beam. Although this information is available online, I decided to derive it to get a better understanding for how these equations come to fruition. Using this equation, I derived an expression for the minimum height for the cross section of the crosshead, and got 22.41mm due to deflection. This would designate the true height since 22.41 is larger than the 15.49 due to stress. I rounded to 25 mm for ease during the CAD modeling and design process. 

<img width="473" height="215" alt="image" src="https://github.com/user-attachments/assets/41dc8f70-898b-4239-b025-6fc9131ba0cb" />

## Hand Sketch (Nolan)
For the handsketch, I only had one small decision to make. I made the holes cut for the leadscrew to pass through an inch in diameter just to ensure there was no contact with the lead screw and the wall of the crosshead. Everything else was determined by my previous math. 

<img width="467" height="395" alt="image" src="https://github.com/user-attachments/assets/1335346f-3e3d-48a9-8f72-384006ca7445" />

## Cost table (Nolan)

<table style="border-collapse: collapse; width: 100%; text-align: center;">
  <thead>
    <tr style="background-color: #999; color: black;">
      <th style="border: 1px solid black; padding: 8px;">Item #</th>
      <th style="border: 1px solid black; padding: 8px;">Quantity</th>
      <th style="border: 1px solid black; padding: 8px;">Name</th>
      <th style="border: 1px solid black; padding: 8px;">Cost/Item</th>
      <th style="border: 1px solid black; padding: 8px;">Cost</th>
      <th style="border: 1px solid black; padding: 8px;">Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid black; padding: 8px;">1</td>
      <td style="border: 1px solid black; padding: 8px;">2</td>
      <td style="border: 1px solid black; padding: 8px;">Lead Screw</td>
      <td style="border: 1px solid black; padding: 8px;">$28.64</td>
      <td style="border: 1px solid black; padding: 8px;">$54.56</td>
      <td style="border: 1px solid black; padding: 8px;"><a href="https://www.mcmaster.com/98940A305/">Link</a></td>
    </tr>
    <tr>
      <td style="border: 1px solid black; padding: 8px;">2</td>
      <td style="border: 1px solid black; padding: 8px;">2</td>
      <td style="border: 1px solid black; padding: 8px;">Flange Nut</td>
      <td style="border: 1px solid black; padding: 8px;">$178.60</td>
      <td style="border: 1px solid black; padding: 8px;">$357.20</td>
      <td style="border: 1px solid black; padding: 8px;"><a href="https://www.mcmaster.com/97790A110/">Link</a></td>
    </tr>
    <tr>
      <td style="border: 1px solid black; padding: 8px;">3</td>
      <td style="border: 1px solid black; padding: 8px;">4</td>
      <td style="border: 1px solid black; padding: 8px;">Head Screw</td>
      <td style="border: 1px solid black; padding: 8px;">$10.02 <small>(50 ct.)</small></td>
      <td style="border: 1px solid black; padding: 8px;">$10.02</td>
      <td style="border: 1px solid black; padding: 8px;"><a href="https://www.mcmaster.com/92316A540/">Link</a></td>
    </tr>
    <tr>
      <td style="border: 1px solid black; padding: 8px;">4</td>
      <td style="border: 1px solid black; padding: 8px;">1</td>
      <td style="border: 1px solid black; padding: 8px;">Frame</td>
      <td style="border: 1px solid black; padding: 8px;">$125.63</td>
      <td style="border: 1px solid black; padding: 8px;">$125.63</td>
      <td style="border: 1px solid black; padding: 8px;"><a href="https://www.mcmaster.com/47065T882-47">Link</a></td>
    </tr>
    <tr style="background-color: #ccc;">
      <td colspan="5" style="border: 1px solid black; padding: 8px; text-align: right; font-size: 1.4em; font-weight: bold;">TOTAL</td>
      <td style="border: 1px solid black; padding: 8px; font-size: 1.4em; font-weight: bold;">$565.41</td>
    </tr>
  </tbody>
</table>

## Total time Nolan = 2.5 hr

## Parametric Modeling (Brandon)

I began by using the calculations that Nolan came up with to build my equation sheet. In the instructions we were given some unknowns, but the rest Nolan had to solve and I had to use them for the CAD model. By using his calculations, it made it very simple to make my equations on SolidWorks. 

<img width="724" height="221" alt="Screenshot 2026-11-15 224432" src="https://github.com/user-attachments/assets/69e45ef6-0985-457b-98db-a32f2d1a66bc" />

After completing the equations and knowing the values I was able to begin my sketch. Below is an image of how I began modeling the cross body. 

<img width="349" height="208" alt="Screenshot 2026-11-15 224733" src="https://github.com/user-attachments/assets/5b3dc2c2-0b7a-49eb-93a2-4311ecb69225" />

After sketching the part, I extruded it to the correct measurements given to me by Nolan. 

<img width="732" height="415" alt="Screenshot 2026-11-15 224822" src="https://github.com/user-attachments/assets/c7817610-811d-4ad4-ac82-ab1953e337d3" />

Once I finished the cross head I put the frame together and began to put the assembly together. 


<img width="321" height="290" alt="Screenshot 2026-11-17 002823" src="https://github.com/user-attachments/assets/a2e8e73d-1814-4a6c-a362-ae9fa9cbc65b" />

Below is the assembly completed. Everything worked very well and was completed as instructed. 

<img width="236" height="347" alt="Screenshot 2026-11-17 005119" src="https://github.com/user-attachments/assets/01a914df-99c4-4213-b6a3-cf93743e0d17" />

## Lessons Learned
Modeling the lead screw and crosshead helped me better understand how individual mechanical components work together in an assembly. I learned the importance of using accurate dimensions, aligning components properly, and making sure the threads and mating features fit together correctly. One challenge was creating the threaded lead screw and ensuring the crosshead could move along it as intended. This project improved my CAD modeling skills and taught me to pay closer attention to detail when designing parts that must interact with one another. Overall, I gained a better understanding of mechanical assemblies and how proper modeling can help ensure that a design functions as expected.


## Total time Brandon = 5 hours

## CAD FILES

# A10 CAD Files

[Google Drive – A10 CAD Files](https://drive.google.com/drive/u/0/folders/1nQlM7cM3rbcqljRFo6o5Ii-l7HKpFuqM)

















