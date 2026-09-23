# A5 – Bracket Design

This week's design involves designing a bracket to hold a strap, which applies a load to that bracket. We will be using 2 different approaches to the design: Stress and Stiffness analysis. 

### Constraints and Givens:

<img width="567" height="266" alt="image" src="https://github.com/user-attachments/assets/be46312e-136e-49a1-8350-1000b7cd4db4" />

### Aluminum 6061 Characteristics:

For my material, I have chosen Aluminum 6061. I have chosen this over the steel and titanium options because it meets all of the strength requirements, as well as being vastly easier to machine.

<img width="412" height="130" alt="image" src="https://github.com/user-attachments/assets/1d6f9a5e-e920-4057-96b0-b02f2f8be0fe" />

T Beam Dimensions:

<img width="550" height="249" alt="image" src="https://github.com/user-attachments/assets/d4913862-b319-4609-b622-093ce8a2b7d3" />

Rough Geometry Example: 

<img width="366" height="306" alt="image" src="https://github.com/user-attachments/assets/a9ccba73-5d8e-4c58-a48f-eab69ce78a56" />


## Stress Analysis

### Feature 1

Feature 1 is the pin on which the strap will rest. If you are looking at the Rough Geometry Example provided in class, it is section A. This piece will be modeled after a cantilever beam with a load in the center.

#### Assumptions, Knowns and Unknowns:

<img width="768" height="390" alt="image" src="https://github.com/user-attachments/assets/751848b9-7489-4783-9af2-de3a18541c4c" />

#### Solving:

<img width="785" height="364" alt="image" src="https://github.com/user-attachments/assets/ce5a879e-3166-445c-a3b8-edf6893a23c0" />

The final Pin diameter is 0.386 in.

### Feature 2

Feature 2 is the bar which connects the pin to the body of the bracket. On the rough geometry example above, it is section B. This piece will be modeled after a bar under axial load. Notice how I have halved the force. For Feature 2 I will be using the symetry of the design to my benefit, halving the force and dimensions. While not 100% necessary for Feature 2, my reasoning will be better displayed on Features 4 and 5.

#### Assumptions, Knowns and Unknowns:

<img width="774" height="507" alt="image" src="https://github.com/user-attachments/assets/db16b356-94be-47d5-854b-4da94ff627e7" />

#### Solving:

<img width="540" height="297" alt="image" src="https://github.com/user-attachments/assets/1ca16332-d625-48b6-bd53-0e08b90ab92e" />

The final thickness for the bar is 0.155 in.

### Feature 3 

Feature 3 is the base of the bracket which connects to the T beam. On the Rough Geometry Example it is section C. This will be modeled after a simply supported beam with a load in the center of it. Notice how for this feature, I have not halved the force. I have done this because solving for a simply supported beam is easier than solving for 2 cantilever beams. 

#### Assumptions, Knowns and Unknowns:

<img width="723" height="383" alt="image" src="https://github.com/user-attachments/assets/6251c1ab-f5a1-4c0d-bbbd-0a7e8b013e80" />

#### Solving:

<img width="720" height="366" alt="image" src="https://github.com/user-attachments/assets/80d60bbe-f0c7-49a4-8f7d-c418e4772247" />

The final thickness for the bracket base is 0.474 in.

### Feature 4

Feature 4 is the "wall" or arms of the bracket, connecting the base to the overhanging Feature 5. This will also be modeled as a bar under axial load. Note how I have halved the force. This is because of the symmetry of the design. This allows me to solve for one side of the bracket, since the load will be evenly distributed between both arms. 

#### Assumptions, Knowns and Unknowns:

<img width="747" height="348" alt="image" src="https://github.com/user-attachments/assets/d051b11c-6b06-4d35-92fe-32ffe52dc93f" />

#### Solving:

<img width="524" height="314" alt="image" src="https://github.com/user-attachments/assets/4541b6ec-b120-4b49-88d3-2a2f946c0217" />

The final thickness for Feature 4 is 0.02 in.

## Stiffness Analysis

Stiffness Analysis will follow the same plan as the Stress Analysis, just using different equations, as well as a new constant. The Modulus of Elasticity is a constant characteristic of the Aluminum, similar to the Yield Strength we used to solve for the Stress Analysis. It measures the materials resistance to elastic deformation when a stress is applied. Many of the Assumptions and Unknowns will not change while solving for the thickness using Stiffness Analysis.

### Feature 1

#### Assumptions, Knowns and Unknowns:

<img width="764" height="387" alt="image" src="https://github.com/user-attachments/assets/f1acf9c1-3689-48f5-a4cc-2590a12695f3" />

#### Solving:

<img width="752" height="433" alt="image" src="https://github.com/user-attachments/assets/77dbd49b-c7b1-4d4d-b669-e9cb0daedf5f" />

The thickness for Feature 1 using Stiffness Analysis is 0.192 in. Note how similar that is is Feature 1's radius (0.193 in).

### Feature 2

#### Assumptions, Knowns and Unknowns:

<img width="713" height="437" alt="image" src="https://github.com/user-attachments/assets/71ef397e-5abd-42ae-9bc3-e87b3e547648" />

#### Solving:

<img width="686" height="203" alt="image" src="https://github.com/user-attachments/assets/4848b0d9-e0ff-4df6-969a-ea0464a6a2f3" />

The thickness for feature 2 is 0.031 in.

### Feature 3 

#### Assumptions, Knowns and Unknowns:

<img width="741" height="387" alt="image" src="https://github.com/user-attachments/assets/e61991f3-d02d-4f00-b047-516e2d04e9a4" />

#### Solving:

<img width="697" height="416" alt="image" src="https://github.com/user-attachments/assets/b4a24c5d-7cef-4c9a-b59c-4f3c2ab6837b" />

The thickness for feature 3 is 0.361 in.

### Feature 4

#### Assumptions, Knowns and Unknowns:

<img width="747" height="348" alt="image" src="https://github.com/user-attachments/assets/7580b659-9aec-4bd0-91a7-c56cfa4ab43a" />

#### Solving:

<img width="524" height="314" alt="image" src="https://github.com/user-attachments/assets/efa674dc-f776-4fb4-a877-305a7d021016" />

The thickness for feature 4 is 0.004 in.

## Lessons Learned

### Governing failure mode:

The closest final dimension we've seen between 2 features is with feature 3, being just slightly more than 1/10 an inch apart. 

### Error propagation:

Remember when I mentioned how similar the radius of the Feature 1's Stress Analysis is to the diameter of Feature 1's Stiffness analysis? I went ahead with the Stress Diameter until I started on this webpage, where I noticed it while screenshotting the work to put in here. The damage was minimal, I just had to rework a few problems. Still a valuable mistake to be made here, rather than outside of an educational environment. 

### Assumption sensitivity: 

One assumption I made was the length of the pin in Feature 1. I chose a length of 0.75 in so that the strap would rest nicely on it when in use, and it also made the math easier. If it were incorrect, or needed to be adjusted, it would mostly be isolate to changing the final pin diameter of the Feature.

