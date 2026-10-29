# A8 – Gears

## Objective

This week I am designing a gear box for 2 different gears as well as selecting proper bearings for the design.

## Design of Shafts

### Input Shaft

The only torque provided for the design was at the output, so I needed to use the gear ratio as well as the RPM (solved for in the next image) to calculate the torque being applied to the input.

<img width="713" height="122" alt="image" src="https://github.com/user-attachments/assets/e166b165-33db-4d4d-a5d8-a88439143ca3" />

Solving for the power allows me to solve for the minimum diameter necessary for the input shaft.

<img width="895" height="457" alt="image" src="https://github.com/user-attachments/assets/3306c678-1dec-4961-be50-1c5d5deb7633" />


### Output Shaft

As mentioned before, the torque and RPM of the output shaft was provided for, so all that was left was to solve for the power and diameter. As you can see the 0.1167 inch minimum diameter is well below the quarter inch provided.

<img width="895" height="351" alt="image" src="https://github.com/user-attachments/assets/dd33a6be-7dbf-48d7-974e-4bd6d4289fc4" />


## Design of Journal Bearings

To properly select a bearing material, I must solve for the Load Capacity, Survace Speed and PV limit (Pressure-Velocity limit).

<img width="569" height="324" alt="image" src="https://github.com/user-attachments/assets/c4b3a9c1-9d6b-4815-bc6c-abbc9d070caf" />

### Input Shaft

First we will solve for the Area of the cross section of the shaft. I chose the Length of 0.125 inches because this meets the standards set out in Machineries Handbook where the ratio between the length of the bearing and the diameter of the shaft should be 1.

<img width="845" height="535" alt="image" src="https://github.com/user-attachments/assets/19c850bf-fe2d-46b7-ad9b-0ec8b87f421d" />


### Output Shaft

Solving for the output shaft, we take the same approach as the input shaft. The Length to diameter ratio is 1.

<img width="819" height="444" alt="image" src="https://github.com/user-attachments/assets/ad934ad9-3c63-43b5-9e9f-99671bea6b30" />


### Journal Bearing Thickness

Solving for the Journal thickness the approach is for it to be 1/4 to 1/2 of the diameter of the shaft. Adding the diameter of the shaft and 2 * the thickness of the shaft gives us the outside diameter of the bearing. Now we can take the PV limit, dimensions and material selection and pick out our bearing from McMaster-Carr's website.

<img width="728" height="501" alt="image" src="https://github.com/user-attachments/assets/a64e6635-250f-4ada-ac80-6c96439bd5bc" />


### Journal Bearing Selections

For the 0.125" diameter shaft we went with a bronze graphite lubricated bearing. 

[Link to McMaster-Carr](https://www.mcmaster.com/9368T95/)

<img width="617" height="448" alt="image" src="https://github.com/user-attachments/assets/44024ad8-4b96-4e6b-92de-13afbef9cbe0" />

For the 0.25" shaft, we stuck with bronze for a material.

[Lint to McMaster-Carr](https://www.mcmaster.com/2867T43/)

<img width="621" height="447" alt="image" src="https://github.com/user-attachments/assets/6748fba5-1a60-47f9-8034-1697fec588c7" />


## Sketch

Below is the rough sketch of the gear box.

<img width="532" height="317" alt="image" src="https://github.com/user-attachments/assets/3fcd96fc-138f-4925-99e3-6d81c74d3a9e" />

## CAD Model


### Parametric Design

The following dimensions will allow us to parametrically design all components of the gear box. 

<img width="822" height="395" alt="parametric" src="https://github.com/user-attachments/assets/7fd9bb96-3a3f-473b-86e8-906029eaa690" />


### Design

<img width="1919" height="1007" alt="assem_pic" src="https://github.com/user-attachments/assets/295177e2-5f31-4124-8dc5-6105284a6e18" />


<img width="1194" height="749" alt="full_assem_pic" src="https://github.com/user-attachments/assets/eaddea90-d211-40f5-bded-37c3367cccea" />


## Drawings

<img width="848" height="656" alt="image" src="https://github.com/user-attachments/assets/52adcac7-6c7f-4bf9-88e4-25b20ec3c9e8" />

<img width="754" height="585" alt="image" src="https://github.com/user-attachments/assets/f5f41be1-84d9-4416-8b94-20e03e7fbf6e" />

<img width="778" height="605" alt="image" src="https://github.com/user-attachments/assets/0ebbd393-0b1c-4273-b4d1-231e0a06973c" />

<img width="822" height="630" alt="image" src="https://github.com/user-attachments/assets/de690419-0b64-4019-a2b3-aefa585fa3cc" />

<img width="874" height="675" alt="image" src="https://github.com/user-attachments/assets/6bd474e9-5297-41ec-8a17-9df796839658" />

<img width="766" height="593" alt="image" src="https://github.com/user-attachments/assets/ff2de231-2378-4050-98bf-18cbeeb7ed69" />

<img width="656" height="509" alt="image" src="https://github.com/user-attachments/assets/c6c51415-b7e3-4a79-8c64-5f271ff6197c" />

### [Link to Download CAD File and Drawings](https://drive.google.com/drive/folders/14A8U5oYg87rSfvFFgkx6eMHjwfaJhaWu?usp=sharing)

## Lessons Learned

This week was all about learning how to operate Solidworks. The biggest lesson that I learned from this was that different types of CAD software are all doing the same thing, with slightly different variations. I was stuck trying to thread the screw holes for the design and discovered the abundance of resources available for Solidworks. This has been a much more pleasant design experience compared to using Fusion and Creo in previous weeks. 

I also learned about gearing and designing parts to fit them. I initially failed to use the pitch diameter of the gears when designing the layout, and instead used the outside diameter. This did not allow for the gears to properly mesh, and it was fixed. 
