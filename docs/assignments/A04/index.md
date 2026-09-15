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

For Feature 2, I first created a free-body diagram (FBD) and identified all of the known and unknown values. Before determining the required height, I needed to calculate the feature’s overall length and maximum bending moment. Using the 80 mm plate length and the 13 mm height from Feature 1, I determined the overall length to be (L_2 = 93) mm. I then used the applied force of 300 N and the distance from the fixed end to calculate the maximum bending moment, which was (M = 33,300) N·mm.

<img width="746" height="1002" alt="0" src="https://github.com/user-attachments/assets/2e54cea1-56b4-40b0-a944-d6a6d3871f49" />

After determining these values, I used the bending stress and deflection equations to calculate the required height, (h_2). I then compared the heights obtained from each equation and selected the larger value. Using the larger height ensures that Feature 2 satisfies both the allowable stress and maximum deflection requirements.

<img width="773" height="1002" alt="0" src="https://github.com/user-attachments/assets/942bfc7c-d71a-4ff2-a066-20238fb03a6a" />

## Motor Mount Sketch 


<img width="2005" height="1211" alt="unnamed" src="https://github.com/user-attachments/assets/880e3c76-7a5b-4b1e-aaa0-48eb3fb3c13c" />




## CAD Model (Parametric)

Here are my global variables that helped me build my part. 

<img width="599" height="263" alt="Screenshot 2026-09-15 000835" src="https://github.com/user-attachments/assets/1ade8eae-3fd8-40b6-b219-c216b1f3670e" />


Once I had my dimensions, I traced out the shape of the motor to then base extrude the part. 

<img width="619" height="342" alt="Screenshot 2026-09-15 001418" src="https://github.com/user-attachments/assets/f793c02d-0533-44e8-b22f-c84ccea0a640" />

I then cut the holes on feature 2 for the screws. 

<img width="497" height="340" alt="Screenshot 2026-09-15 003921" src="https://github.com/user-attachments/assets/e50ae4be-8c28-428f-a8ac-300aba6a7e9c" />

I then cut the holes for the motor to sit in.

<img width="334" height="211" alt="Screenshot 2026-09-15 004554" src="https://github.com/user-attachments/assets/ce2aaf03-4e21-4b00-8cfb-e13f2cd6a9da" />

I then had the completed part as seen below: 

<img width="456" height="356" alt="Screenshot 2026-09-15 004717" src="https://github.com/user-attachments/assets/e0248b35-5eb0-442b-a07b-2cb7d4c8a772" />


## Lessons learned 

While completing the motor mount assignment, I learned very important factors including how to implement a safety factor for both deflection and stress. I learned how to sketch on different planes to connect the drawing in the end. It was very challenging at first, but once I cut out my part it made much more sense. 

This assignment took me around 6 hours to complete. 



## Appendix 

These are the websites I got additional information/inspiration: 

[Appendix 1](https://thmotorsports.com/8496834-innovative-mounts-10751-75a-innovative-steel-motor-mounts)

[Appendix 2](https://www.advanceadapters.com/engine-motor-mounts-2)

