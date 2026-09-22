# A5 – [Bracket Design]

For this assignment I had to design a bracket. The objective of this design is to develop a bracket that can move freely along a rigid T-beam while safely carrying a 600 lbf applied load. A safety factor of 4 is required to ensure the bracket withstands the expected loading conditions. Aluminum 6061-T6 was selected as the material, with a yield strength of 40,000 psi and a Young’s modulus of 10,000,000 psi. Throughout the analysis, several engineering assumptions and approximations will be introduced and explained as needed. Shear failure is excluded from consideration in this design.

<img width="1395" height="1108" alt="image" src="https://github.com/user-attachments/assets/ccbf5b53-69c9-4f95-98fb-0930f8efe3b9" />

To simplify the design and analysis process, I chose to maintain a symmetrical bracket geometry, incorporating this decision into the subsequent calculations.


## Part 1 ( Stress Calculations )

I now calculated the stress of the bracket by dividing it into 5 parts as shown in the image below. This image was given to me in the assignments directions. 


<img width="382" height="345" alt="image" src="https://github.com/user-attachments/assets/14a34e8f-e0f2-4db1-b2d3-95add9e97044" />

The following sections detail the analysis performed on each bracket component. The design incorporates a 0.75-inch-wide U-line strap with a 14-inch diameter, which influenced several of the assumptions used throughout the calculations. To evaluate the forces and reactions acting on the bracket, I created a free-body diagram (FBD) for each individual segment. The resulting equations are first developed symbolically and then solved using numerical values to determine the required dimensions and verify the design.


<img width="1116" height="1417" alt="image" src="https://github.com/user-attachments/assets/e4171f1b-b5c2-4a08-b387-8e63a3bfc0fb" />


<img width="946" height="803" alt="image" src="https://github.com/user-attachments/assets/80facb65-96b7-49c3-abf6-c9921561e7d1" />


<img width="1341" height="1313" alt="image" src="https://github.com/user-attachments/assets/374e6d9c-360d-4fb5-8cc0-24294a28fe30" />


<img width="1232" height="1078" alt="image" src="https://github.com/user-attachments/assets/1859a231-198f-4a9b-8ef4-8fc87af60c2b" />


<img width="1265" height="1019" alt="image" src="https://github.com/user-attachments/assets/9a261dba-0e55-4c0a-94bb-9e98518d03cf" />



## Part 2 ( Stiffness Calculation )

The stiffness evaluation focused on determining how the bracket’s dimensions would change under the specified loading conditions. I retained the material length from Part A and applied it to the deflection formulas to establish the revised dimensions. For each section, I outlined the available information, identified the quantities being solved for, and documented the assumptions used in the analysis. Free-body diagrams were created for the individual segments, with the calculations presented through both theoretical equations and numerical substitutions.


<img width="1863" height="1202" alt="image" src="https://github.com/user-attachments/assets/bc8eb2b9-cfa8-406f-a939-5cd81d8a0828" />


<img width="1704" height="1304" alt="image" src="https://github.com/user-attachments/assets/b8da3300-dc67-444b-a052-f0c627b00ce7" />


For C-E I used the internal dimensions. 


<img width="1447" height="1185" alt="image" src="https://github.com/user-attachments/assets/3921755b-516a-49f3-920f-72e8c6c4f26f" />


<img width="1592" height="1133" alt="image" src="https://github.com/user-attachments/assets/45000c75-9dc1-453f-8421-47e459b5d0ae" />


<img width="2036" height="1279" alt="image" src="https://github.com/user-attachments/assets/128b3b2b-96e4-4cd4-a050-b7e544e4ae98" />



## Multiview Drawings

I created orthogonal views after I found my dimensions to properly display the design. 


<img width="1152" height="1366" alt="image" src="https://github.com/user-attachments/assets/608d6e3d-4e72-429a-b5a3-b88a54d66164" />


<img width="920" height="998" alt="image" src="https://github.com/user-attachments/assets/a6a73e25-4462-498b-9b14-94fc3b924367" />


I completed the drawings by hand except for the full view. I used the image to make it neater and easier to read. I copied my first drawing of stress and pasted it for stiffness as well and just changed up the numbers.


## Lessons learned

This assignment helped me strengthen my understanding of how statics and strength of materials are used to analyze mechanical components. I learned how to apply normal stress, bending stress, and stiffness equations to determine the appropriate dimensions for a bracket. Developing free-body diagrams for each segment improved my ability to identify forces and establish the equations needed for analysis. I also gained experience making reasonable engineering assumptions and simplifying a design while maintaining accurate calculations. One of the most important lessons I learned was that a component must satisfy both strength and deflection requirements, rather than relying on stress analysis alone. Working through the algebraic and numerical solutions also improved my problem-solving skills and helped me better understand how theoretical equations apply to practical engineering designs.

This assignment took me 8 hours to complete. 


