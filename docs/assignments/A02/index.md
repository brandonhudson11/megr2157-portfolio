# A2 – Truss Stress Analysis

## Objective 

# Project Overview

**All images below can be clicked on to view better and bigger.**

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


<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/5b9fba80-4d1b-4327-afd1-b7c2b3095cc9" />


# Method of Joints 

Once the support reactions were determined, I moved on to analyzing the forces acting within the truss members. I used the method of joints, examining each joint separately to determine the unknown member forces. For each joint, I applied the equilibrium conditions in both the horizontal and vertical directions. Setting the sum of the forces in the x-direction and y-direction equal to zero allowed me to calculate the axial force carried by each member.

**Joint B**

I chose joint B as the starting point for the method of joints because the reaction at this support had already been determined, leaving only two unknown member forces to solve. Based on the 0.30 m vertical dimension and the 0.40 m horizontal dimension, member BC has a total length of 0.50 m. From these dimensions, I determined the angle of the member to be approximately 53° 13′.

I then applied the equilibrium equations at joint B. Summing the forces in the vertical direction allowed me to determine the force in member BC as 13.89 kN. I followed this by summing the forces horizontally, which resulted in a force of −11.11 kN in member AB. The positive or negative sign of an internal member force indicates its type of loading. A positive value represents tension, while a negative value indicates compression.

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/055ecc33-62e7-4617-bf52-f83a4b8dc727" />

**Joint D**

At joint D, I used the equilibrium equations to determine the remaining unknown force in member DA. After applying the appropriate sum of forces, I calculated the force in DA to be 38.33 kN. With this final member force determined, I had all the necessary force values to move forward with sizing the truss members based on the stresses they experience.

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/f52e1df5-de4f-49d1-9e3a-dab52ca4a367" />

**Joint C**

I then analyzed joint C by first determining the diagonal length of member AC. Using the truss geometry, I calculated AC to be 0.8544 m. From this value, I determined the directional components needed for the equilibrium equations, obtaining cosθ = 0.9363 and sinθ = 0.3511.

After resolving the forces into their horizontal and vertical components, I applied the sum of forces equations at joint C. The calculations resulted in an axial force of −41.774 kN for member AC and 28.003 kN for member CD. The negative value for AC indicates that the member is actually experiencing compression, which is opposite to the assumed force direction used in the free-body diagram. Of all the forces calculated in the truss, AC has the greatest magnitude, making it the critical member that will determine the required member size during the next stage of the design.

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/4adbcee6-bf41-41e1-b5b7-9aaa9078de60" />

# Cross Sectional Area (Miniumum) 

To determine the required cross-sectional area of the members, I based my calculations on the normal stress equation, which relates stress, force, and area as σ = F/A. I also accounted for the specified factor of safety by calculating the allowable stress from the material’s yield stress using σallow = σy/N. After combining these relationships and rearranging the equations, I obtained the minimum required area as Amin ≥ NFmax/σy. This equation provides the minimum cross-sectional area needed for the member to safely withstand the maximum applied force while maintaining the required factor of safety. Below is my symbolic answers. 

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/c8f65895-6330-414a-9f60-1c71fc39b981" />

I then plugged the numbers in to get the numerical answers. (You can click the image to make it bigger and easier to read)

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/fa779805-6065-4a48-ac9a-5af77062f8f3" />

# Critical Member selection 

Based on the results from the previous analysis, member AC is the critical member because it experiences the highest force, with a magnitude of 41.774 kN while being subjected to compression. For the sizing calculations, I used the design parameters provided in the problem. These included a factor of safety of 3.5, a material yield strength of 345 MPa, and a density of 7850 kg/m³. These values, along with the calculated member force, were used to determine the required dimensions of the member. The following section summarizes the known quantities and the variables that still need to be determined:

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/5199ad6d-409a-47c4-af6c-4596ec46d82e" />

# Trust Member Weight

The next step was to determine the overall size and weight of the truss. I used the member dimensions from my worksheet, which were 1.20 m for AB, 0.50 m for BC, 0.40 m for CD, 0.50 m for DA, and 0.8544 m for AC. Together, these members resulted in a combined length of 3.2544 m.

I used this total length along with the cross-sectional area to determine the volume using V = AL. Once the volume was known, I calculated the truss mass from the material density using m = ρV. To convert the mass into a force due to gravity, I used W = mg. These calculations resulted in a volume of 0.001464 m³ and a mass of 11.49 kg. The corresponding weight of the truss members was calculated to be 112.7 N.

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/f5b99acf-d42e-4a5c-9ccf-a19c1646a28e" />

# Pin Shear

Unlike the truss members, the pins are designed based on shear loading instead of normal stress. For this part of the analysis, I used the greatest reaction force at the supports as the critical load, rather than using the maximum force found in an individual truss member. The reaction force used was 8.33 kN, which is equivalent to 1.873 kip.

The remaining design parameters were a shear strength of 170 ksi, a safety factor of 4, and a material density of 0.278 lb/in³. I also assumed that the pin experiences one shear plane. Using these values and the appropriate shear-stress relationship, I developed the symbolic calculation shown below to determine the required pin size.

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/dee7abce-7109-4e58-ba1d-ac7db1732649" />

Below is the shear solved with numbers. 

<img width="257" height="160" alt="0" src="https://github.com/user-attachments/assets/f25bf02a-9e5f-41a4-bb2b-0611acc9a531" />





