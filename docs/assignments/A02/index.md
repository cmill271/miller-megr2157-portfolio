# A2 – Truss Stress Analysis
Assignment 2 asked to design a lightweight planar truss with the following parameters: the truss will be made of A500 Steel or an alternative material, the cross sectional area of each element is identical, the pins must also be identical, and it must fit the parameters in Figure 1 below. For the external forces acting upon points C and D, I was given the choice of a force in the range of 20-30kN, I chose 30 kN. 
<img width="881" height="441" alt="image" src="https://github.com/user-attachments/assets/295a7e68-d74e-42e2-8b0e-3851c2d0bc1a" />
## My Design

I chose to base the design of the truss off a standard truss bridge. This design uses triangles to handle the applied forces while using as little material as possible in an attempt to save weight. To start the process I began buy solving for the additional geometry the design called for. These calculations were made simple by the fact that my design only produces 3/4/5 triangles, giving truss' BC, CF and AD a length of 0.5 m.

<img width="681" height="308" alt="image" src="https://github.com/user-attachments/assets/7e1ae43e-a696-4c33-85d2-24d6fbd8bc51" />

## Internal and External Forces

To begin solving for the internal forces, I started with the external forces. There are a total of 4 external forces, with 2 unknown. Thanks to forces P1 and P2 only acting on the y-axis, there are forces acting on the x-axis as I have shown in the image below. To solve for the forces of Ay and By I start by taking the sum of moments about point B. This leaves me with one unknown (Ay), which I solved for by taking the sum of forces on the y-axis. 

<img width="789" height="475" alt="image" src="https://github.com/user-attachments/assets/c33874d7-1b9f-4100-a44f-8685777f3571" />

Now that I have the external forces solved, I can solve for the internal forces. For this I used the Method of Joints. I started by drawing each joint where two or more beams connect in a Free Body Diagram (FBD), allowing me to visualize the forces acting upon the joint. For each joint the sum of forces in any axial direction is equal to zero, allowing me to solve for the internal loads with a simple sum of forces equation. I started this process at Pin B. With one external force acting on this point, and 2 internal, I was able to solve for BE and BC. I repeated this 4 more times, not having to solve for Pin C because I had solved for everything already. 

<img width="599" height="718" alt="image" src="https://github.com/user-attachments/assets/22986a03-f63a-4d2c-aabc-7c2d96519b13" />

## Cross Sectional Area of Elements

The next step was to solve for the required cross sectional area of each element. The Factor of Safety (FOS) was provided for us in the prompt, however I was left stumped for the yield strength of A500 steel. Some quick searching found it for me, as the [Steel Tube Institute](https://steeltubeinstitute.org/resources/astm-a500/) provides thorough information about it. A500 Steel is a common type of stainless steel used for construction and structural purposes. For the purposes we are using it for, A500 Grade C square cut steel tubing has a yield strength of 345 MPa. Going with hollow tube steel allows for all the strength of steel, while saving on weight. Using our equations for the FOS and stress, we are able to solve for the cross sectional area of each element. The required cross sectional area is 338.13 millimeters squared. 

<img width="637" height="412" alt="image" src="https://github.com/user-attachments/assets/e47dab0a-a078-4b8f-8ba3-306dc306b4a3" />

Additionally we calculated the approximate weight of each element by calculating the total length of A500 steel that will be required for the truss, and multiplying it by an approximate mass per unit length for A500 Steel with our cross sectional area. This gives us an approximate weight of 8.48 kg. 

<img width="639" height="406" alt="image" src="https://github.com/user-attachments/assets/37ea32f6-ac9a-469c-9a62-9c32d6ebee97" />

## Cross Sectional Area of Pins

We are now asked to determine the cross sectional area of the pins that will connect the elements of the truss together. We are provided with the, FOS, yield shear strength and density of the hardened tool steel that the pins will be made of. For simplicity, we will be using the joint with the largest reaction load to base our pin design off of. Similar to finding the areas of the truss elements above, we will be using the sheer FOS formula and single sheer formula to solve for the area. Note my exclusion of the variable "n". In the shear formula an additional variable "n" will be included in the denominator to denote the number of sheer connections the load is spread over. In this instance we are using a single sheer design, but if we were to use more than that, we would multiply the denominator by that number to account for the extra connections.  

<img width="632" height="197" alt="image" src="https://github.com/user-attachments/assets/c323b307-19f5-42e7-9627-c24f97edcb58" />

Now that we know what we know, and don't know, we can begin to solve for our required area. First, the sheer force acting on the pins plane. To solve for this we sum the forces acting on Pin C (the pin with the largest reaction load), and use Pythagoreans' theorem to solve for the total sheer acting on that plane. Note how the FBD for Pin C is different here compared to earlier when we were solving for internal forces. This is because when we solved for those internal forces, we discovered if they were in compression (pushing against the pin) or tension (pulling against the pin). This new FBD helps visualize this information better for solving the problem. This leaves us with a total sheer force of 13.34 kN.  

<img width="575" height="413" alt="image" src="https://github.com/user-attachments/assets/dc5aa313-b166-43e5-88c3-609fa5e0cc84" />

Finally, we can solve for area. Using the FOS and sheer formulas, we combine the two using the sheer force they share to give us the equation below. The final cross section area of the pins is 45.5 millimeters squared. 

<img width="591" height="107" alt="image" src="https://github.com/user-attachments/assets/61635adc-9fa4-40f0-b28f-ef64f391879b" />

We were also asked to solve for the estimated weight of the pins. The product of the pin area we found as our base, and the depth of the square A500 steel for our height, we find the volume of a pin. This is then multiplied by the density of the hardened tool steel (after some simple conversion to metric units), and we are left with an estimated total weight for the 6 pins of 38.67 grams. 

<img width="636" height="171" alt="image" src="https://github.com/user-attachments/assets/472d95dc-ff7f-4b61-9d4b-a1c3c1cba815" />

## CAD Model of Truss

The longest and most tedious part of this assignment was modeling the Truss and testing it in CAD. My chosen software is Creo Parametric. To start we first made a sketch of the truss. Ignore the listed dimensions, as tidying up the sketch so Creo would properly extrude the material threw off the perfect points and measurements. 

<img width="1387" height="568" alt="image" src="https://github.com/user-attachments/assets/6af46a2e-91c4-4606-8b9e-9c36524fd14b" />


## Lessons Learned

This exercise was an excellent refresher on my Statics and Mechanics skills. I learned a better method for finding the sheer stress in a pin than I had used previously, saving me time and effort. Drawing the FBD for the pin helped me to visualize the forces better and kept the numbers from getting mixed together.


## Failure Modes in Truss Components

In a truss there are 3 main forces that account for the majority of failures: 

### 1) A member buckling due to a compressive force.

Looking at our design the following members fall under compression: BC, CF, and AF. 

<img width="506" height="320" alt="image" src="https://github.com/user-attachments/assets/aa2c1158-c307-41b2-aa83-3e880f28dfab" />

When a member is placed under compression, the slenderness of the object becomes an issue. If the material is too thin or has the incorrect material properties for the job it will buckle under the force of the load. A single uncooked spaghetti noodle when placed under under a compressive force will buckle almost immediately, and fracture soon after. We can solve this by using more spaghetti noodles, combining them until we have a member that is rather compressible before and buckling or failure occurs. Buckling can be catastrophic for the truss, so important measures like adding more material can be taken to prevent it. However, adding too much material can add unnecessary or inhibitive amounts of weight. Choosing the right material for the task is key. In our case we designed the truss using A500 steel, a common structural steel that is perfect for the task.

### 2) A member fracturing due to tensile force.

Looking at our design the following members fall under a tensile force: BE, EF, CD, DF and AD. 

<img width="530" height="340" alt="image" src="https://github.com/user-attachments/assets/0ecbef7e-7e2d-49dc-ac26-fd66f21b6f5e" />

Under a tensile force, the material is pulled rather than compressed. The thickness of the material becomes important. Often times the body of the member is not most susceptible to a tensile force, its areas where the material must be thinned for the design. When I go flyfishing in a tiny trout stream in the mountains, the fish are small and cannot exert a tensile force great enough to break any line I carry, however when I went deep sea fishing the larger fish are able to exert a larger tensile force on the line, so I have to compensate with a thicker fishing line. More often than not, when I lose a fish or a fly, it is because the failure point was where I tied the fly to the line. In our design that would be where material is removed to allow pins to connect two or more members. This thinner material has less surface area connecting the material to itself, making it weaker.

### Solutions for 1 & 2. 

Dealing with the members of the truss our main enemies are compressive and tensile forces acting upon them. Luckily engineers have spend all of history solving these problems. The first solution we have is design. You'll notice that the shape made by each member of the truss is a triangle. The triangle shape is very strong, allowing for the distribution of a load across all 3 members that make it. The next solution we have is material choice. A500 steel is perfect for our design. It is a ductile material, meaning it can undergo significant plastic deformation before any permanent deformations occur. It's tubular shape is also perfect for adding rigidity to less material, saving on cost and weight.


## 3) Connection point failure.

The failure point of a pin comes down to the sheer forces applied to it. If the shear force becomes too great, the pin itself will sheer and the connection point will be compromised at best, or completely lost as worse. 

<img width="332" height="270" alt="image" src="https://github.com/user-attachments/assets/edafd031-1dbb-43cc-880d-33a9e8da0236" />

The image above represents the single sheer pin system we used in this design. The "single" in single sheer represents the single plane where the sheer force is applied. Adding additional material and alternating the material creates more planes, think of a door hinge. If you applied the same load to a double sheer pin, the amount of sheer force acting on each plane would halve. Since we were limited to a single sheer pin design for this assignment, we compensated with the thickness of the material. by ensuring the material was thick enough to with stand a force 4 times greater (the Factor of Safety being 4), we can ensure that the pin is thick enough to withstand the forces applied. To even further reduce this likelihood of failure we can make it a double or triple sheer.   

## Decide

I believe that my design choices were correct for this assignment. 

## Sources


