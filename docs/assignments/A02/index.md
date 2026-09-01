# A2 – Truss Stress Analysis
Assignment 2 asked to design a lightweight planar truss with the following parameters: the truss will be made of A500 Steel or an alternative material, the cross sectional area of each element is identical, the pins must also be identical, and it must fit the parameters in Figure 1 below. For the external forces acting upon points C and D, I was given the choice of a force in the range of 20-30kN, I chose 30 kN. 
<img width="881" height="441" alt="image" src="https://github.com/user-attachments/assets/295a7e68-d74e-42e2-8b0e-3851c2d0bc1a" />
## My Design

I chose to base the design of the truss off a standard truss bridge. This design uses triangles to handle the applied forces while using as little material as possible in an attempt to save weight. To start the process I began buy solving for the additional geometry the design called for. These calculations were made simple by the fact that my design only produces 3/4/5 triangles, giving truss' BC, CF and AD a length of 0.5 m.

<img width="681" height="308" alt="image" src="https://github.com/user-attachments/assets/7e1ae43e-a696-4c33-85d2-24d6fbd8bc51" />

To begin solving for the internal forces, I started with the external forces. There are a total of 4 external forces, with 2 unknown. Thanks to forces P1 and P2 only acting on the y-axis, there are forces acting on the x-axis as I have shown in the image below. To solve for the forces of Ay and By I start by taking the sum of moments about point B. This leaves me with one unknown (Ay), which I solved for by taking the sum of forces on the y-axis. 

<img width="789" height="475" alt="image" src="https://github.com/user-attachments/assets/c33874d7-1b9f-4100-a44f-8685777f3571" />

Now that I have the external forces solved, I can solve for the internal forces. For this I used the Method of Joints. I started by drawing each joint where two or more beams connect in a Free Body Diagram (FBD), allowing me to visualize the forces acting upon the joint. For each joint the sum of forces in any axial direction is equal to zero, allowing me to solve for the internal loads with a simple sum of forces equation. I started this process at Pin B. With one external force acting on this point, and 2 internal, I was able to solve for BE and BC. I repeated this 4 more times, not having to solve for Pin C because I had solved for everything already. 

<img width="599" height="718" alt="image" src="https://github.com/user-attachments/assets/22986a03-f63a-4d2c-aabc-7c2d96519b13" />



## Objective


## Analyze


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

