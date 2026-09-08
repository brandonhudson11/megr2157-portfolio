# A3 – Paramteric and FEA

## Part 1

The purpose of this assignment was to design a solid circular bar that has a load between 300-500 lbf while limiting the max axial deflection to 0.009 inches. The bar had to be constructed of aluminum with a modulus of elasticity between 8.5-11.5 x10^6 psi. For my cross-sectional design, I chose a diameter of 0.5 inches. I chose my force to be 400 lbf and my elasticity to be 11x10^6. I then calculated the cross-sectional area by using the formula pi x diameter^2 all divided by 4. I then used the direct tension elongation equation, δ = AE/FL, and arranged the equation to solve for L (length). I then used my force of 400 lbf and the minimum modulus of elasticity to show the most demanding design condition. My calculations are shown below. 

<img width="1239" height="1189" alt="unnamed" src="https://github.com/user-attachments/assets/53607d4d-85a8-4133-8351-162a3f892348" />


## CAD

I started the CAD by sketching the circular end of my bar. The diameter was .500 as shown below. 

<img width="284" height="199" alt="Screenshot 2026-09-08 004428" src="https://github.com/user-attachments/assets/cf9e9188-6fef-4c28-b28d-6bb5488a0546" />

I then extruded the length to 48.60 inches. I got 48.60 for my L by the calculations I did. 

<img width="836" height="302" alt="Screenshot 2026-09-08 004712" src="https://github.com/user-attachments/assets/9d42dd3e-1e10-4031-9ce0-1abeb3880975" />

I then went to the equations tab and inserted the equations and all of my variables. My answers I got when I solved were the same as SolidWorks as shown below. 

<img width="599" height="263" alt="Screenshot 2026-09-08 005425" src="https://github.com/user-attachments/assets/814bfa46-eb10-4608-bfa8-c2ce2ad13eb3" />

Then I chose the material for my bar. It needed to be made of aluminum, so I chose the 1060 alloy because it met my calculations the most.

<img width="612" height="483" alt="Screenshot 2026-09-08 014317" src="https://github.com/user-attachments/assets/b871f022-e75d-4fed-ac1e-72a5aed8c8cc" />


## FEA Simulation

For the FEA simulation I began by putting one end as fixed geometry and applying a 400 lbf to the other end pulling away from the bar. 

<img width="771" height="446" alt="Screenshot 2026-09-08 011126" src="https://github.com/user-attachments/assets/d7c84de1-e545-4cbe-897e-301f84e816e2" />

<img width="719" height="433" alt="Screenshot 2026-09-08 011259" src="https://github.com/user-attachments/assets/0daa6b2c-3268-484e-b267-ff48ce772143" />


## Deflection Curve

Next, I ran a simulation to find a deflection curve. The result gave me .00905 which matches what was in the instructions given. 

<img width="782" height="410" alt="Screenshot 2026-09-08 012616" src="https://github.com/user-attachments/assets/c0a0e337-db7f-4f80-aa7b-ca20e7c4bb40" />


## von Mises Stress Curve

The stress curve shows the beam strength to be 3.999x10^3 which shows a safety factor of 1.47. Since the max stress is 2.193 psi and that number is lower than yield strength, the beam is in the allowed strength. 

<img width="792" height="410" alt="Screenshot 2026-09-08 012310" src="https://github.com/user-attachments/assets/c2c7fb13-976d-4ced-9a65-e7d2454195e3" />


## Design Reflection 

The assignment was very easy to understand and made a lot of sense. I did have a few moments that I did struggle though. It took me a little time to find the simulation and how to insert the force and fixed geometry. After figuring that out, everything else fell in place. The only other issue I had was changing units on my von Mises graph. Once I figured that out, I had no more issues. 

My axial deflection was similar to what was given to me. Therefore, I believe my numbers and bar are correct. The two values I calculated are relatively close because the bar has a uniform cross-section and is under simple axial loading. The original design did not have any significant changes in geometry or stress. The small difference between the two results could be due to the material properties used in SolidWorks. For this axial bar, I would rely slightly more on the hand calculations since the bar has a uniform cross-section. However, the FEA results are still useful because they show that the model behaves very similarly to the analytical prediction.  This is way higher than the 3999 psi yield strength of the 1060 aluminum. The resulting safety factor was 0.34, so the design implementing a large pin would no longer pass.

This assignment took 3.5 hours to complete. 

