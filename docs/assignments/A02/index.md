# A2 – Truss Stress Analysis

## Objective 

# Project Overview

For this assignment, I created and analyzed a truss with specific measurements. The work below documents steps taken to design my truss. The geometry, pin reactions, member force reactions, cross sectional area, and the truss weight are all documented below. The page has been organized to show every step taken to design and build the truss. Each section has a title above it telling what each image represents. Below is a image that was given to us with some parameters.


<img width="257" height="160" alt="download" src="https://github.com/user-attachments/assets/aa6a21d4-7568-41b0-8e27-0c66fd79250c" />


The distance a is 0.4m and b is 0.3m. The two forces labeled P have to be chosen at any number between 20-30 kN. Point A is a pin connection, and point B is a roller. The beam must be made of A500 steel and the cross sections had to be equal throughout the beam. 



## Decide 

The image below shows the truss I decided to create. I chose the truss below because I though by making a connection to the pin the truss would not move and would allow the support to be greater than if I used the roller. I chose 23kN for my force P. 


<img width="300" height="202" alt="0" src="https://github.com/user-attachments/assets/aa8b62c0-1b61-461a-93e7-4182644b5415" />



## Analyze

**Truss Geometry**

To set up the truss analysis, I first identified the locations of all the joints and labeled the individual members. The truss consists of five members: AB, BC, CD, DA, and AC. I used the dimensions provided in the problem, including the 0.3 m vertical measurement and the 0.4 m distances associated with BC, CD, and AD.

For the external load, I needed to select a value from 20 to 30 kN. I chose 23 kN as my load because 23 is the jersey number worn by my favorite NBA player, LeBron James. After selecting the load, I determined the types of reactions created by each support. Point A is a pin, meaning it can resist forces in both the horizontal and vertical directions, so I represented its reactions as Ax and Ay. Point B is a roller support, which only provides a vertical reaction, represented by By.

**Solving for External Reactions**

Before determining the forces within the individual truss members, I needed to calculate the reaction forces at the supports. I started by taking moments about point A because this allowed me to eliminate the reactions at A and solve directly for the unknown reaction at B. Using the given distances and the 23 kN load, my moment equation was:

−By(1.2) − 23(0.8) + 23(0.4) = 0

Solving this equation resulted in By = −7.667. Once I found the reaction at B, I used the vertical force equilibrium equation to determine Ay. This gave me Ay = −By, resulting in Ay = 7.667 N. Finally, the horizontal reaction at A, Ax, is equal to zero because there is no horizontal force applied to the truss.


<img width="300" height="202" alt="0" src="https://github.com/user-attachments/assets/5b9fba80-4d1b-4327-afd1-b7c2b3095cc9" />


## Method of Joints 

