# A3 – Parametric and FEA

## Objective

For this assignment we were given a simple task: to parametrically design a bar with a circular cross section, place it under a load and analyze the results. The image below gives you a rough idea of the design.  

<img width="476" height="114" alt="image" src="https://github.com/user-attachments/assets/ee28b87f-04dd-4d2e-a9a4-f646e49af3b8" />

## Parametric Design

To begin we opened up Fusion 360 and set the parameters for the bar. We were provided with a force (400 lbf), a change in length (0.009 in) and the Youngs Modulus for the aluminum material (1*10^7). I chose the base diameter of 1 inch.

<img width="1919" height="978" alt="Screenshot 2026-09-09 203646" src="https://github.com/user-attachments/assets/c664f2c8-9e0b-47a8-8572-980c4cba66f8" />

To solve for the length we are using 2 separate equations for stress: the first is the equation where you are multiplying the Youngs modulus by the strain, and the second is force divided by area. Since both are equations for stress, we set them equal to each other and solve for the length. 

<img width="1919" height="978" alt="Screenshot 2026-09-09 203646" src="https://github.com/user-attachments/assets/6237756d-44ec-471b-a4d3-21190b8b7658" />

The final equation is the same equation we solved for under the parameter "length" in Fusion.

The value this parametric design generated was 176.715 inches, a number my hand calculations confirmed.

## Modeling the Part

To begin modeling the part, a circle was sketched and the diameter was set equal to the base diameter of 1 inch.

<img width="858" height="434" alt="Screenshot 2026-09-09 204009" src="https://github.com/user-attachments/assets/269c9037-5c6b-4250-9460-62856f4ce212" />

Then we extruded the circle to make the rod, setting the height equal to the length we calculated in the parametric design.

<img width="1916" height="982" alt="Screenshot 2026-09-09 204031" src="https://github.com/user-attachments/assets/fbeafbde-7b80-4718-8c8f-7dd19ad5d814" />

To complete the model, we made sure to change the material from the default of steel to aluminum. Notice the slight change in material properties from our given properties to the ones saved in Fusions programing.  

<img width="1918" height="1035" alt="Screenshot 2026-09-09 204532" src="https://github.com/user-attachments/assets/c301a345-e1be-443e-b7e5-8a33823ed43a" />

## Conducting the Finite Element Analysis (FEA)

The first step to conducting our FEA is to set constraints on the model. We will begin by locking the bottom face of the bar to the plane it originates from.

<img width="1919" height="1005" alt="Screenshot 2026-09-09 204639" src="https://github.com/user-attachments/assets/3376333d-2c17-4aa3-a6b0-eb13a5427365" />

Then we will apply our 400 lbf force to the face pointing away from the origin plane. Anchoring the bottom and pulling on the top will generate the tensile stress necessary to complete our analysis. 

<img width="1918" height="1030" alt="Screenshot 2026-09-09 205003" src="https://github.com/user-attachments/assets/0a2e0051-1cf9-4eed-90b7-e0765037012f" />

Once we run the simulation it provides detailed information. 

<img width="1919" height="1030" alt="Screenshot 2026-09-09 210750" src="https://github.com/user-attachments/assets/a5d0bc29-80a5-4d73-a3e4-eb0ffc2e02d0" />

# Deflection Map

<img width="1920" height="892" alt="a3 displacement" src="https://github.com/user-attachments/assets/f33a7cd2-5d03-4a4f-ad1b-44cbff3914e8" />

The image above highlights the deflection caused by the force.

# Mises Stress Map

<img width="1920" height="892" alt="A3 von mises" src="https://github.com/user-attachments/assets/21d6cb40-0cb7-4367-b9c3-ce1b3e2c73dc" />

# The Numbers

Maximum Stress: 1,002.944 psi
The maximum stress is significantly lower than the strength of aluminum (~1 ksi vs 40 ksi).
Axial Deflection: 0.004 in
Safety Factor: 8

## Reflection 
There was a meaningful discrepancy. The hand calculations showed a deflection of 0.009 in, while the simulation showed a deflection of 0.004 in. While the difference is miniscule, the simulated value is less than half of the hand calculated value. I believe this discrepancy comes from an error on my part when setting up the simulation. I would trust my hand calculation over the simulated, as I have more experience with hand calculations and minimal experience in Fusion360. 

## Modifying Design Parameters

I modified the parametric design parameters by changing the load to 1000 lbf and base diameter to 0.25 in. I believe that the length will increase. Below are the changed parametric design parameters.

<img width="1918" height="981" alt="Screenshot 2026-09-09 215213" src="https://github.com/user-attachments/assets/d821fb13-7763-4782-b676-e84b714cc21f" />

The results are not shocking, there was an increase in length. However, this design was flagged by Fusion 360 as not being safe, due to the forces applied. 

<img width="1920" height="892" alt="image" src="https://github.com/user-attachments/assets/65953335-4219-43ce-844c-ddea5328f83b" />

## Files

[Link to CAD file.](https://a360.co/4r19dJH) 

