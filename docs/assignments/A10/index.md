# A10 – Lead Screw Translating System

Lead screw Diameter (Bryson)
I began by assuming steel with a yield strength of 310 MPa for the lead screws. This gave me a starting point for estimating the minimum diameter before selecting an actual screw. Assuming the two screws share the 2 kN load equally, each screw supports 1,000 N. I used axial stress and a safety factor of 4 to calculate a minimum diameter of approximately 4.05 mm. This represents the minimum diameter needed for axial strength under my assumed material properties and helped guide my selection of a commercially available lead screw.



After estimating the minimum diameter, I selected a 1/2"-10 lead screw and used its dimensions to calculate the required rotational speed and torque. With 10 threads per inch and a single-start thread, the screw advances 2.54 mm per revolution. Dividing the required crosshead speeds of 1–50 mm/min by this lead gave me a rotational speed range of approximately 0.39–19.68 rpm. Using the 1,000 N load per screw, an assumed friction coefficient of 0.2, and the dimensions shown in my calculations, I obtained an estimated torque of 1,695.831 N·mm per screw. These calculations connected the selected screw’s geometry to the motion and driving torque required for the tensile tester.

image

Nut and Flange (Bryson)
Next, I researched McMaster-Carr’s recommended nuts and flanges for the lead screw I selected. I chose a 1/2"-10 flanged nut made from 932 bearing bronze to match the screw’s thread size. I calculated the number of engaged threads (N_t) by dividing the thread engagement length of 44.45 mm by the pitch of 2.54 mm, resulting in 17.5 engaged threads. I then used this value to calculate the thread bearing and bending stresses under the 1,000 N load per screw. Using a bronze yield strength of 124 MPa and a safety factor of 4, I calculated an allowable stress of 31 MPa. My calculated bearing stress of approximately 1.253 MPa and thread bending stress of approximately 4.229 MPa were below this value. Based on the dimensions and assumptions used in this analysis, the selected nut met the calculated thread-strength requirement.

image

Total Time (Bryson) = 2.5 hrs
Crosshead (Nolan)
The project parameters allowed us to design a crosshead with a lot of freedom. I did some research, and found that a 300mm crosshead (length) would work nicely. I then had to choose the material and thickness of the crosshead. I chose ASTM A36 steel for its high stiffness and a base width of 60mm. I then modeled the crosshead as a beam supported at both ends with a load in the center (as explained in lecture). I then found where the shear force = 0 (max moment location) and then found the max moment equation to equal PL/4.

image

To perform a stress analysis, I did some algebra with the equations for stress due to bending on a beam, moment of inertia, and neutral axis to POI (c). I ended up with a derived equation for the minimum allowed height of the crosshead due to normal stress (due to bending) and plugged in the numbers to obtain a value of 15.49mm.

image

To determine the minimum height of the crosshead in terms of deflection, I first took a cut of the left hand side of the beam, and determined the moment equation in terms of x. I then integrated twice to get the deflection and slope equation, and solved to finish my derivation of max deflection for the beam. Although this information is available online, I decided to derive it to get a better understanding for how these equations come to fruition. Using this equation, I derived an expression for the minimum height for the cross section of the crosshead, and got 22.41mm due to deflection. This would designate the true height since 22.41 is larger than the 15.49 due to stress. I rounded to 25 mm for ease during the CAD modeling and design process.

image

Hand Sketch (Nolan)
For the handsketch, I only had one small decision to make. I made the holes cut for the leadscrew to pass through an inch in diameter just to ensure there was no contact with the lead screw and the wall of the crosshead. Everything else was determined by my previous math.

image

Cost Table (Nolan)
Item #	Quantity	Name	Cost/Item	Cost	Link
1	2	Lead Screw	$28.64	$54.56	Link
2	2	Flange Nut	$178.60	$357.20	Link
3	4	Head Screw	$10.02 (50 ct.)	$10.02	Link
4	1	Frame	$125.63	$125.63	Link
TOTAL	$565.41
Total Time (Nolan) = 2.5 hrs
Parametric Modeling (Brandon)
I began by using the calculations that Nolan came up with to build my equation sheet. In the instructions we were given some unknowns, but the rest Nolan had to solve and I had to use them for the CAD model. By using his calculations, it made it very simple to make my equations on SolidWorks.

image

After completing the equations and knowing the values I was able to begin my sketch. Below is an image of how I began modeling the cross body.

image

After sketching the part, I extruded it to the correct measurements given to me by Nolan.

image
