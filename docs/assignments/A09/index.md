# A9 – Pulleys

## Objective

This week we are designing a pulley system. Below is the provided information, as well as some assumptions and early calculations.

<img width="334" height="386" alt="image" src="https://github.com/user-attachments/assets/38217a62-0438-495f-883c-78a1529d39a7" />

Pulley systems require special attention to the stresses applied to the belt. As discussed later, I faced some unique complications having to do with the additional stress applied via the rotation of the pulleys..

## Belt

To select a proper belt for the system, we need to be aware of friction ration between the pulley material (aluminum) and belt material (polyurethane). A quick search shows that the coefficient of friction between the two is 0.3. We will use this to solve for the friction ratio, which we can use to solve for our tensions.  

#### Knowns and Unknowns

<img width="660" height="283" alt="image" src="https://github.com/user-attachments/assets/ded44f1f-b892-429f-9135-d3b5482a710f" />

#### Solving for Belt Area, Diameter and Length 

Here we see the application of the friction ratio I spoke of earlier. Using this ratio and some basic algebra, we are able to solve for both tensions.

<img width="660" height="688" alt="image" src="https://github.com/user-attachments/assets/b25aa4ec-fc9d-46c2-b301-9825f9d59797" />

#### Belt Selection

The belt I selected for the pulley system is McMaster-Carr stock number: [3044K606](https://www.mcmaster.com/3044K606-1835T383/). This belt is available in the required circumference, and will easily withstand the stresses applied to it. 

<img width="1051" height="842" alt="image" src="https://github.com/user-attachments/assets/6a031313-1ffb-441b-8642-f37e7dd9e2b8" />

Once we solve for the cross sectional area, we can solve for the diameter of the belt. We are left with a diameter of 19.4".

## Shaft

Solving for the shaft is relatively straight forward know that we know the tensions being applied to the two pulleys. Note the change of material from the aluminum pulleys to 1060 Steel. The specific unknowns we are looking for is the maximum shear stress applied to the shaft by the belts, the moment created by the belts and finally the minimum diameter of the shaft.

#### Knowns and Unknowns

<img width="785" height="486" alt="image" src="https://github.com/user-attachments/assets/b1c92119-15d2-40eb-9604-a7c17e8be576" />

#### Solving for Minimum Shaft Diameter

<img width="787" height="323" alt="image" src="https://github.com/user-attachments/assets/25c6a95a-f2c6-45c4-a6ff-b1f2fc55572f" />

Solving for the shaft diameter minimum, we see that it is 0.145". While this diameter takes into account our safety factor a 3, it was difficult to find a bearing with this specific diameter. Our selected diameter is 0.25". This will make choosing a bearing much simpler, as well as add to the rigidity of the system.

## Bearings

The key to selecting a bearing is the PV limit. Multiplying the pressure (P) by the rotational velocity in ft/min (V) gives us that. 

#### Knowns and Unknowns

<img width="564" height="200" alt="image" src="https://github.com/user-attachments/assets/c9c5ba2c-e046-42f1-bc45-6a4c5cf53f61" />

#### Solving for PV limit

<img width="542" height="317" alt="image" src="https://github.com/user-attachments/assets/4bd9cc92-e3e1-40de-8f7a-bd46e8bafad4" />

#### Bearing Selection

With a PV limit of 15,712 we chose porous bronze. These bearings are impregnated with lubrications, and our selected diameter makes choosing one simple. 

The bearing selected is McMaster-Carr stock number: [6391K114](https://www.mcmaster.com/6391K126/).

<img width="1055" height="840" alt="image" src="https://github.com/user-attachments/assets/f88ad1d2-0962-47c1-b9d9-d863afab28e2" />

## Lessons Learned

This week I learned that using solely the static tension that is applied to the shaft does not take the torque applied during the operation. When I would double check my answers, I would find my values significantly off. However, despite this the selected diameter of 0.25" is more than adequate for the operation of the pulley system. 
