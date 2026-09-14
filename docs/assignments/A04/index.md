# A4 – Motor Mount

## Assignment description/objective 

This assignment is designed to give students experience in designing a motor mount in two different ways. One part of the design will use stress and the other will use deflection. The difference in the approach will help students better understand design challenges and how to optimize for the two different types of constraints. 

Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) HERE which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

<img width="123" height="99" alt="download" src="https://github.com/user-attachments/assets/28956435-a517-4513-95e9-385a7102eacf" />

Figure 1(above): Shows motor, the rigid wall and the force received on the shaft of the motor, where P = 300 N

<img width="1625" height="505" alt="unnamed" src="https://github.com/user-attachments/assets/9856e722-ffa1-472e-af64-d70ffb1355f9" />

<img width="296" height="289" alt="download" src="https://github.com/user-attachments/assets/b9052cc9-6d35-4d69-89ec-f6f4605268f9" />


## Feature 1

In feature 1 I began by determining the minimum height of the motor mount needed to safely support the applied load without exceeding stress or maximum deflection allowed which was .30mm. I then created a FBD of feature one so I could determine the forces acting on it so I could calculate the moment. The applied load was 300N and my width was 40mm for feature 1. The mount was designed using ABS, which has an elastic modulus of approximately 2,000 N/mm². A safety factor of 3 was required for the stress analysis, with a maximum allowable deflection of 0.30 mm. The applied load produced a moment of 5,400 N·mm. The primary unknown in the design was the height of Feature 1. To organize the given information and simplify the calculations, I created separate columns for the known and unknown variables. This allowed me to clearly identify the required dimension and determine the height needed to meet the design requirements.

<img width="790" height="1002" alt="0" src="https://github.com/user-attachments/assets/87f344ab-2a25-411e-abb0-07593875410b" />

Using the known and unknown values, I applied the bending stress and deflection equations to determine the required height of the feature. I first rearranged both equations symbolically to isolate the height, which made it easier to substitute the known values. After calculating the required height from both the stress and deflection equations, I compared the two results and selected the larger value. This ensured that the final feature height satisfied both the allowable stress and maximum deflection requirements.

<img width="777" height="1002" alt="0" src="https://github.com/user-attachments/assets/c43e932c-f893-4e5d-a6b8-f2a12e16e285" />






## Feature 2 

<img width="746" height="1002" alt="0" src="https://github.com/user-attachments/assets/2e54cea1-56b4-40b0-a944-d6a6d3871f49" />

<img width="773" height="1002" alt="0" src="https://github.com/user-attachments/assets/942bfc7c-d71a-4ff2-a066-20238fb03a6a" />




## CAD Model (Parametric)

