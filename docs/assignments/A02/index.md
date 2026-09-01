# A2 – Truss Stress Analysis

## Objective 

# Project Overview

**All images below can be zoomed in on for better quality.**

For this assignment, I created and analyzed a truss with specific measurements. The work below documents steps taken to design my truss. The geometry, pin reactions, member force reactions, cross sectional area, and the truss weight are all documented below. The page has been organized to show every step taken to design and build the truss. Each section has a title above it telling what each image represents. Below is a image that was given to us with some parameters.


<img width="300" height="250" alt="download" src="https://github.com/user-attachments/assets/aa6a21d4-7568-41b0-8e27-0c66fd79250c" />


The distance a is 0.4m and b is 0.3m. The two forces labeled P have to be chosen at any number between 20-30 kN. Point A is a pin connection, and point B is a roller. The beam must be made of A500 steel and the cross sections had to be equal throughout the beam. 



## Decide 

The image below shows the truss I decided to create. I chose the truss below because I though by making a connection to the pin the truss would not move and would allow the support to be greater than if I used the roller. I chose 23kN for my force P. 


<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/aa8b62c0-1b61-461a-93e7-4182644b5415" />



## Analyze

# Truss Geometry

To set up the truss analysis, I first identified the locations of all the joints and labeled the individual members. The truss consists of five members: AB, BC, CD, DA, and AC. I used the dimensions provided in the problem, including the 0.3 m vertical measurement and the 0.4 m distances associated with BC, CD, and AD.

For the external load, I needed to select a value from 20 to 30 kN. I chose 23 kN as my load because 23 is the jersey number worn by my favorite NBA player, LeBron James. After selecting the load, I determined the types of reactions created by each support. Point A is a pin, meaning it can resist forces in both the horizontal and vertical directions, so I represented its reactions as Ax and Ay. Point B is a roller support, which only provides a vertical reaction, represented by By.

# Solving for External Reactions

Before determining the forces within the individual truss members, I needed to calculate the reaction forces at the supports. I started by taking moments about point A because this allowed me to eliminate the reactions at A and solve directly for the unknown reaction at B. Using the given distances and the 23 kN load, my moment equation was:

−By(1.2) − 23(0.8) + 23(0.4) = 0

Solving this equation resulted in By = −7.667. Once I found the reaction at B, I used the vertical force equilibrium equation to determine Ay. This gave me Ay = −By, resulting in Ay = 7.667 N. Finally, the horizontal reaction at A, Ax, is equal to zero because there is no horizontal force applied to the truss.


<img width="1074" height="1002" alt="0" src="https://github.com/user-attachments/assets/de06a496-3224-4d42-821b-831ea11fc1d2" />


# Method of Joints 

Once the support reactions were determined, I moved on to analyzing the forces acting within the truss members. I used the method of joints, examining each joint separately to determine the unknown member forces. For each joint, I applied the equilibrium conditions in both the horizontal and vertical directions. Setting the sum of the forces in the x-direction and y-direction equal to zero allowed me to calculate the axial force carried by each member.

**Joint B**

I chose joint B as the starting point for the method of joints because the reaction at this support had already been determined, leaving only two unknown member forces to solve. Based on the 0.30 m vertical dimension and the 0.40 m horizontal dimension, member BC has a total length of 0.50 m. From these dimensions, I determined the angle of the member to be approximately 53° 13′.

I then applied the equilibrium equations at joint B. Summing the forces in the vertical direction allowed me to determine the force in member BC as 13.89 kN. I followed this by summing the forces horizontally, which resulted in a force of −11.11 kN in member AB. The positive or negative sign of an internal member force indicates its type of loading. A positive value represents tension, while a negative value indicates compression.

<img width="1356" height="1002" alt="0" src="https://github.com/user-attachments/assets/b05f9555-17a0-4923-9e1b-26d1910a98e0" />

**Joint D**

At joint D, I used the equilibrium equations to determine the remaining unknown force in member DA. After applying the appropriate sum of forces, I calculated the force in DA to be 38.33 kN. With this final member force determined, I had all the necessary force values to move forward with sizing the truss members based on the stresses they experience.

<img width="1043" height="1002" alt="0" src="https://github.com/user-attachments/assets/2b6fbc6e-a576-4cfa-8815-13d9d6523cf3" />

**Joint C**

I then analyzed joint C by first determining the diagonal length of member AC. Using the truss geometry, I calculated AC to be 0.8544 m. From this value, I determined the directional components needed for the equilibrium equations, obtaining cosθ = 0.9363 and sinθ = 0.3511.

After resolving the forces into their horizontal and vertical components, I applied the sum of forces equations at joint C. The calculations resulted in an axial force of −41.774 kN for member AC and 28.003 kN for member CD. The negative value for AC indicates that the member is actually experiencing compression, which is opposite to the assumed force direction used in the free-body diagram. Of all the forces calculated in the truss, AC has the greatest magnitude, making it the critical member that will determine the required member size during the next stage of the design.

<img width="1317" height="1002" alt="0" src="https://github.com/user-attachments/assets/998d7934-cd89-43e4-a814-da4ad427799f" />

# Cross Sectional Area (Miniumum) 

To determine the required cross-sectional area of the members, I based my calculations on the normal stress equation, which relates stress, force, and area as σ = F/A. I also accounted for the specified factor of safety by calculating the allowable stress from the material’s yield stress using σallow = σy/N. After combining these relationships and rearranging the equations, I obtained the minimum required area as Amin ≥ NFmax/σy. This equation provides the minimum cross-sectional area needed for the member to safely withstand the maximum applied force while maintaining the required factor of safety. Below is my symbolic answers. 

<img width="1731" height="930" alt="0" src="https://github.com/user-attachments/assets/2b4b71a8-c168-4d20-b376-72155158b6a9" />

I then plugged the numbers in to get the numerical answers. (You can click the image to make it bigger and easier to read)

<img width="1908" height="869" alt="0" src="https://github.com/user-attachments/assets/ac47b3bb-2fcd-4402-a898-04c65d854d19" />

# Critical Member selection 

Based on the results from the previous analysis, member AC is the critical member because it experiences the highest force, with a magnitude of 41.774 kN while being subjected to compression. For the sizing calculations, I used the design parameters provided in the problem. These included a factor of safety of 3.5, a material yield strength of 345 MPa, and a density of 7850 kg/m³. These values, along with the calculated member force, were used to determine the required dimensions of the member. The following section summarizes the known quantities and the variables that still need to be determined:

<img width="1123" height="1002" alt="0" src="https://github.com/user-attachments/assets/145d5595-efbb-4144-a028-697c3fa27cf7" />

# Trust Member Weight

The next step was to determine the overall size and weight of the truss. I used the member dimensions from my worksheet, which were 1.20 m for AB, 0.50 m for BC, 0.40 m for CD, 0.50 m for DA, and 0.8544 m for AC. Together, these members resulted in a combined length of 3.2544 m.

I used this total length along with the cross-sectional area to determine the volume using V = AL. Once the volume was known, I calculated the truss mass from the material density using m = ρV. To convert the mass into a force due to gravity, I used W = mg. These calculations resulted in a volume of 0.001464 m³ and a mass of 11.49 kg. The corresponding weight of the truss members was calculated to be 112.7 N.

<img width="1075" height="1002" alt="0" src="https://github.com/user-attachments/assets/91fa8825-497d-40c8-902f-052dcb139c4d" />

# Pin Shear

Unlike the truss members, the pins are designed based on shear loading instead of normal stress. For this part of the analysis, I used the greatest reaction force at the supports as the critical load, rather than using the maximum force found in an individual truss member. The reaction force used was 8.33 kN, which is equivalent to 1.873 kip.

The remaining design parameters were a shear strength of 170 ksi, a safety factor of 4, and a material density of 0.278 lb/in³. I also assumed that the pin experiences one shear plane. Using these values and the appropriate shear-stress relationship, I developed the symbolic calculation shown below to determine the required pin size.

<img width="1604" height="815" alt="0" src="https://github.com/user-attachments/assets/5a9a79bc-7945-4697-bb88-adfc3f5be9fe" />

Below is the shear solved with numbers. 

<img width="1507" height="1002" alt="0" src="https://github.com/user-attachments/assets/69e3be02-88d2-4090-a25a-e6a3c0d793f1" />

# CAD Model on Solidworks

Once I completed all the work above, I began to 3D model my truss. I started by using the sketch tool on solid works and drawing a trapezoid/triangle. Below is an image as soon as I finished drawing my lines before I extruded. 

<img width="761" height="362" alt="Screenshot 2026-09-01 001453" src="https://github.com/user-attachments/assets/a270bc90-4388-42c0-a459-b74393ae970f" />


Next, I begin to plan my extrude. The image below is my extruded part before I added the extra line to form my truss. 

<img width="705" height="290" alt="Screenshot 2026-09-01 002226" src="https://github.com/user-attachments/assets/ca6e22e1-c8ee-4ef2-877f-da9adcf3ad3e" />


Then, I decided to create a new parts folder and create my pins. The pin had a diameter of .005 and it worked perfectly. I extruded the pin the same depth as my truss structure.  

<img width="1336" height="1002" alt="0" src="https://github.com/user-attachments/assets/e4af304a-8dc5-4cf7-883a-07cead7897f1" />


Then, it was time to install the pins into the truss structure. I had to add the pins to an assembly with the truss. I then had to line up my pin with the truss and use a tool called mate in SolidWorks. 

<img width="741" height="377" alt="Screenshot 2026-09-01 012837" src="https://github.com/user-attachments/assets/43a5c205-a7c1-47fb-a995-19f7aa00992b" />

The image below is my pin going into the truss!

<img width="621" height="377" alt="Screenshot 2026-09-01 013120" src="https://github.com/user-attachments/assets/52ddf83d-8a28-400e-834f-ca925b72ba93" />

Below is my materials page with ASTM A36 steel because SolidWorks did not have A500. 

<img width="356" height="599" alt="Screenshot 2026-09-01 014638" src="https://github.com/user-attachments/assets/5760d373-db53-49fe-aecd-b7d3f6be20b0" />


After SolidWorks showed me the weight of my truss, it said it weighed 9.87kg. The measurement I got when doing calculations was 11.49. My calculations were very close to what SolidWorks gave me. 


<img width="1720" height="958" alt="unnamed" src="https://github.com/user-attachments/assets/54602c57-0dbf-4bf6-90d6-09bca1732286" />

Here is my final CAD model of the truss:

<img width="621" height="272" alt="Screenshot 2026-09-01 014808" src="https://github.com/user-attachments/assets/f75e2525-2d9a-4f70-908c-2ff41c83d88c" />

The CAD Pdf was turned in on canvas. Below is a link to my files as well. Just access them through the drive photo.

[CAD A2 Files](https://drive.google.com/drive/u/0/folders/1-Yj8_bN6x-p6JOk36pKA5HuB3BvxTGS-)

# Engineering Lessons Learned

Through this truss project, I learned how important it is to understand the forces acting on each member of a structure. I gained experience using the method of joints to determine whether members were in tension or compression. I also learned how support reactions affect the forces throughout the entire truss. Another important lesson was understanding how safety factors and material properties are used to determine appropriate member sizes. Overall, this project helped me see how engineering calculations can be used to design a structure that is both safe and efficient. I believe in the future with assignments such as these preparing myself days in advance would be beneficiary. 

# Time Spent

This assignment took me around 17 hours to complete over the course of 5 days. 














