# A7 – FEA on Bracket

### [LINK TO DOWNLOAD CAD FILE](https://a360.co/4i0vKU6)

## Objectives and Problem Formulation 
This week we will be conducting FEA on the bracket that I parametrically designed over the last 2 assignments. Below are the conditions and restrictions.

#### Load: 600 lbforce acting on the support pin.

<img width="811" height="472" alt="image" src="https://github.com/user-attachments/assets/fd338336-7d6b-4c71-8bb1-5c38632efd7a" />

#### Fixed Constraints: The bottom side of the bracket, which interacts with the top of the T-beam.

<img width="514" height="483" alt="image" src="https://github.com/user-attachments/assets/20c931aa-815a-439f-98ec-685c1bbb3ace" />

#### Material Properties: When parametrically designing the object I failed to change the material type. This was not an issue, because the equations we used to solve for the dimensions parametrically used the correct figures, but for this analysis I needed to change the material to aluminum for the FEA.

<img width="652" height="313" alt="image" src="https://github.com/user-attachments/assets/46ff8a89-02bc-41f6-8131-e7252b88f0df" />

## Inner Loop: Mesh Convergence Analysis

### Table of Mesh Convergence Analysis Figures

<img width="726" height="115" alt="image" src="https://github.com/user-attachments/assets/c88944a0-5f23-40d4-88c9-d581c29dfb03" />

### Stress Analysis of Bracket. Iterations are from right to left.

<img width="710" height="314" alt="image" src="https://github.com/user-attachments/assets/b1c905aa-c0fa-41e8-b6b5-a63080d25764" />

## Outer Loop: Iterative Design Optimization

### Design II prior to testing.

<img width="555" height="748" alt="image" src="https://github.com/user-attachments/assets/6bb0e9b4-6c92-47a0-bd43-afa6106cc189" />

### Stress Analysis of Bracket. Iterations are from right to left.

<img width="723" height="115" alt="image" src="https://github.com/user-attachments/assets/86427c79-620e-4689-b21a-df74dbb5433a" />

<img width="889" height="421" alt="image" src="https://github.com/user-attachments/assets/a297ab76-589c-4f8b-bb4c-4b260d1f1c15" />

### Design III prior to testing.


## Reflections

An engineering lesson that I learned is how Fusion deals with assemblies vs a solid part. Attempting to modify an assembly in Fusion took me down a 3 hour rabbit hole that ended with me having to recreate the part, export it as a step file and then I was able to join them into something modifiable. Finding resources for Fusion proved difficult, as most of the class provided ones were for CREO or Solidworks. Moving forward I am going to attempt to do future assignments in Solidworks, as that appears to be the most popular amongst my peers and is the software used by the instructor in class.
