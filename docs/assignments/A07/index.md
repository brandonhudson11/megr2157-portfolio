# A7 – [FEA On Bracket]

This project focuses on evaluating three versions of a bracket using computer-based engineering analysis. The work builds on the models created in Assignments #5 and #6, with design changes introduced to improve the bracket's ability to support loads and maintain its shape under stress. Each version is assessed using Finite Element Analysis (FEA) to determine how well it performs in terms of strength, rigidity, and material usage. Mesh refinement is also performed to check the reliability of the calculated results. The goal is to achieve a difference of 7% or less between successive mesh results, or to use the finest mesh after three attempts if this requirement is not met.

To keep the comparison consistent, the same material, loading conditions, and supports were maintained throughout the study. All three models were assigned 6061-T6 aluminum in SOLIDWORKS. A 600 lbf force was directed downward onto the lower cylindrical portion of the bracket, while the bottom surfaces of the retaining lips were restrained. For each design, the simulation was repeated with three mesh settings to examine how mesh refinement affected the results. The report includes plots from the finest mesh for each version, along with tables comparing the results from each attempt to determine whether the solutions were sufficiently consistent.

## Design 1

The first bracket configuration was analyzed using the original model, with no adjustments made to its shape or dimensions. The simulation indicated that stress was concentrated around the junction between the vertical stem and the upper horizontal section, where the sharp corner creates a potential weak point. For this analysis, I selected a mesh element size of 0.12 in. to evaluate the bracket's stress distribution. The results, simulation image, and supporting calculations for the finest mesh of each design are presented below.

<img width="2172" height="724" alt="919b2854-afa6-47f2-8906-9cdcab119a4e" src="https://github.com/user-attachments/assets/7c41897d-7c94-46b9-9a3b-8b2d38e34e15" />


<img width="1604" height="540" alt="fdc000d2-2223-4159-b145-189be1db911b" src="https://github.com/user-attachments/assets/dcef96ae-3179-4989-8852-5eea4cff3389" />


## Design 2

In the second design, I revised the bracket by adding a 0.15 in. radius at the joint between the stem and the crossbar. The rounded edge was introduced to help distribute stress more evenly and reduce the localized stress buildup observed in the original model. I then performed three simulations using progressively smaller mesh sizes. The final plots were taken from the finest mesh, which had an element size of 0.075 in. When comparing the last two mesh results, the stress variation was 7.08%, slightly above the allowable limit. Because the results did not fully satisfy the convergence requirement, the finest-mesh solution was retained for evaluating the second design.

<img width="2458" height="750" alt="b7c0e306-002c-4b7f-9af6-b969a1c548db" src="https://github.com/user-attachments/assets/2b1d75eb-1b68-4d87-8170-ccd2de6a7dde" />


<img width="1604" height="534" alt="97ec606e-5540-48a3-bb01-0fd51386858a" src="https://github.com/user-attachments/assets/8b6bf20f-32d5-415e-abfd-525289ad4436" />


## Design 3 

For the third design, I kept the fillet from Design 2 and increased the stem depth from 0.659 in. to 1.00 in. This adjustment was made to improve the bracket's stiffness and limit the bending observed in the previous designs. After running the simulations with different mesh sizes, the stress difference between the final two meshes was 2.89%, meeting the required convergence limit of 7%. This indicates that the stress results were consistent between the two finest meshes, making Design 3 the most reliable of the three designs in terms of mesh convergence.

<img width="2470" height="754" alt="eebc72c6-202b-49fb-b5a8-a9c82d699159" src="https://github.com/user-attachments/assets/a1537801-fa62-4e42-8ad7-d18f6ad2d1ac" />

<img width="1608" height="544" alt="ac945b84-e157-4270-8df1-06e0e921c03d" src="https://github.com/user-attachments/assets/b1fcc41e-5deb-470f-8543-40c141e103f9" />

## Final Mesh

<img width="1900" height="520" alt="download" src="https://github.com/user-attachments/assets/d0dc72c3-abad-4b13-971b-b9c1cf22cb47" />

<img width="1180" height="266" alt="ccd912d3-f521-4641-8891-090596ff348a" src="https://github.com/user-attachments/assets/cd032c19-6717-46bb-946a-f158bea71b66" />

When comparing the three bracket designs, Design 3 showed the greatest improvement in reducing deflection and achieving consistent stress results. The maximum displacement decreased from 1.251 mm in Design 1 to 0.3884 mm in Design 3, indicating that the final geometry was considerably stiffer under the applied load. This improvement was achieved by retaining the fillet added in Design 2 and increasing the depth of the stem to help limit bending. The mesh convergence study for Design 3 also produced a stress difference of 2.89% between the two finest meshes, satisfying the required 7% convergence criterion. Its factor of safety was 3.67, which was below the target value of 4, meaning that additional improvements would be needed to meet the desired safety margin. However, the final design's mass increased by 24.1% compared with the original bracket, showing that the improvements in stiffness and stress performance came with a weight penalty. Of the three designs, only Design 3 met the stress convergence requirement within the three mesh attempts. Overall, these results demonstrate the importance of balancing stiffness, strength, weight, and numerical accuracy when making engineering design decisions. Although Design 3 showed a substantial reduction in displacement and achieved acceptable stress convergence, further optimization could focus on reducing unnecessary material while maintaining its improved structural performance and bringing the factor of safety closer to the target of 4.


## Lessons Learned 

Throughout this project, I learned how changes in geometry can affect a bracket's stress distribution, stiffness, and overall performance. The first design showed that sharp corners can create areas of concentrated stress, while adding a fillet in the second design helped create a smoother transition between the stem and crossbar. Increasing the stem depth in the third design provided another way to address bending and improve stiffness. I also learned that mesh refinement is important when evaluating FEA results because different element sizes can produce different stress values. Comparing the results between mesh sizes helped determine whether the simulations were consistent enough to be considered converged. Overall, this project showed me how FEA can be used to identify weaknesses, test design improvements, and make engineering decisions based on simulation data rather than appearance alone.


## Time Spent

This assignment took me 9 hours to complete.

