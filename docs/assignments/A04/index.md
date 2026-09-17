# A4 – Motor Mount

## Objective
This week we will be designing a motor mount for a Brushed 24V DC Gear Motor. We were provided with the following parameters:
1. A maximum deflection of 0.3 mm.
2. A force of 300 N.
3. A Safety Factor (SF) of 3.
4. A rough sketch of what our design should look like (shown below).
<img width="194" height="151" alt="image" src="https://github.com/user-attachments/assets/03f61b34-8ec0-4ac5-978f-18ea689a504f" />

We will be designing Feature 1 and Feature 2 separately. Both features will be made of PETG, a plastic commonly used in 3D printers. I chose this material thanks to its excellent structural strength, making it resistant to deflection and vibrations. It is also the most heat resistant of the options, with PLA softening around 50 degrees Celsius while PETG only starts to soften at 75 degrees Celsius. This gives us a Yield Strength ($\sigma$) of 48 MPa and a Elastic Modulus (E) of 2100 MPa. Knowing this, we can now solve for our allowed bending stress, taking into account the safety factor of 3.

<img width="958" height="271" alt="image" src="https://github.com/user-attachments/assets/dce8324b-fd6e-4b96-aded-67911bd95249" />

Solving for our bending stress, with the safety factor taken into account, we are left with an allowed bending stress of 16 MPa. Now its time to start work on the features.

## Feature 1

### Stress

Feature 1 is the base where the motor will rest. For the design we are tasked with finding the cross sectional area of the feature. To start we will assign the feature a length and base of 50 mm, and solve for the height or thickness of the feature.

<img width="958" height="729" alt="image" src="https://github.com/user-attachments/assets/ab9967e7-f1a0-452e-a75d-f8186699b8a4" />

To find the height required for the feature to support the motor wile remaining within our stress limits, we will use our stress equation for a cantilever beam. To solve, I started by taking the equations for the Second Moment of Area (I) and plugging in into the stress equation. Once we have our equation set up, we can plug in the numbers and solve for the height.

<img width="870" height="672" alt="image" src="https://github.com/user-attachments/assets/4654fe11-63bd-42b3-b610-86450352a50b" />

In order to properly account for the 16 MPa stress limit, Feature 1 will require a height of 10.61 mm.

### Deflection

Solving for the height required to stay within our deflection constrains the feature will also require plugging in the equation for I. Once we have that, we can solve for the height of the object.

<img width="832" height="404" alt="image" src="https://github.com/user-attachments/assets/d593de9a-f21c-44f7-b5a0-27e4b5f867ac" />

In order to properly support the motor and limit the deflection Feature one requires a height of 16.82 mm. To allow Feature 2 room for deflection, I have rounded the thickness for this part up to 20 mm, and this will be the height we use moving forward. 

<img width="783" height="84" alt="image" src="https://github.com/user-attachments/assets/ee848e4d-0bd4-41f1-bb5d-652e006c25c3" />

As you can see in the image above, with a height of 20 mm, there is 0.179 mm of deflection. This leave 0.121 mm of deflection for Feature 2.

## Feature 2


## Isometric Drawing


## CAD Model (Parametric)


## Drawings

