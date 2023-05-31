# EXP 03 - THIRD PERSON CHARACTER MESH:

###### NAME: K.M.Swetha
###### REG NO: 212221240055 

## AIM:

1. Import the animation assets: Obtain the animation files for jump, walk, and idle in a compatible format such as FBX or BVH. To import the animations, go to the Content Browser panel in Unreal Engine, right-click in the desired folder, and select Import 

2. Create a Separate folder and Import the Animations to avoid any chaos 

3. Create an animation blueprint: In Unreal Engine, animation blueprints are used to control character animations. To create a new animation blueprint, follow these steps: 
    a. Right-click in the folder where you imported the mesh and select Create > Animation > Animation Blueprint. 
    
    b. In the Animation Blueprint Editor, click on the Event Graph tab. 
    
    c. Drag the new character mesh from the Content Browser and drop it onto the graph. 
    
    d. Connect the Output Pose pin of the mesh node to the Final Animation Pose pin of the Final Animation Pose node. 
    
    e. Save the animation blueprint. 
    
4. Open the animation blueprint: Open the animation blueprint you created for your character in the Animation Blueprint Editor. 

5. Create animation slots: Animation slots help organize different animations and control their blending. To create animation slots, follow these steps: 
    a. In the AnimGraph tab of the Animation Blueprint Editor, right-click in the graph and select Add State Machine > Animation Layer. 
    
    b. Double-click the newly created animation layer to open it. 
    
    c. Right-click in the graph of the animation layer and select Add State Machine. d. Double-click the newly created state machine to open it. 
    
    e. Right-click in the graph of the state machine and select Add State. 
    
    f. Rename the state to "Jump" and repeat steps e and f to create states for "Walk" and "Idle".
    
6. Add animation assets to states: In each state, you will assign the corresponding animation assets. To add animation assets to the states, follow these steps: 
    a. Double-click the "Jump" state to open it. 

    b. Right-click in the graph and select Add State Result. 

    c. Drag and drop the jump animation asset onto the graph. 

    d. Connect the Result node to the jump animation asset.

    e. Repeat steps a to d for the "Walk" and "Idle" states, assigning the appropriate animation assets. 

7. Create required Variables for the state’s like “ISJUMP”, “SPEED”. 

8. Set up transition rules: Transition rules determine when the character transitions between different animations. To set up transition rules, follow these steps: 
    a. Double-click the "Jump" state to open it. 
    
    b. Right-click in the graph and select Add Transition Rule. 
    
    c. Drag the transition rule from the "Jump" state to the "Idle" state. 
    
    d. Repeat steps a to c for the "Walk" state, creating transitions from "Idle" to "Walk" and from "Walk" to "Idle". 
    
    e. Configure the transition rules based on your desired conditions. For example, you might want to trigger the transition from "Idle" to "Jump" when the character jumps, and from "Jump" to "Idle" when the jump animation is finished. 

9. Create a Anim Montage in Animation Folder To Manage the montages of the animations.

10. Connect the animation blueprint to the character blueprint: To connect the animation blueprint to the character blueprint and enable the animations in the game, follow these steps:
    a. Open the character blueprint associated with the third person character. 
    
    b. In the Viewport tab of the Blueprint Editor, select the mesh component of the character.
    
    c. In the Details panel, under the Animation category, find the Animation Blueprint property. 
    
    d. Click on the dropdown menu and select the animation blueprint you created. 

11. Test the character: Compile and save all the changes in the blueprints and animations. Now, you can test the character's jump, walk, and idle animations by clicking the Play button in the Unreal Editor.

## OUTPUT:

### ANIMATIONS:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/b158a3fe-3240-4924-b60d-dad143bcba8e)

### STATE MACHINES:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/c0aef584-f0d0-412e-8146-39f81157601d)


### STATE DIAGRAM:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/64df2671-740a-4ef5-b402-3b827876310b)


### VARIABLES:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/46ce9822-7e6f-40b4-921d-3fb2707f703f)


### IDLE TO WALK:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/7a8bbd64-ab15-445f-9280-e6155633f830)

### WALK TO IDLE:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/a46cbe0c-6ff6-4180-a4fe-b6f7387fc4c6)


### WALK TO JUMP:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/7096c02a-a7ed-4953-b2ba-2bfe2247cc9d)

### JUMP TO WALK:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/e27b4477-8010-40ce-8dac-764bc8663fa5)

### JUMP TO IDLE:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/ea71effd-b0f8-4106-8aab-8e294733e869)

### IDLE TO JUMP:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/47c81fbe-4bbd-45dd-88eb-7f7f07cda437)

### ANIMATION BLUEPRINT:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/743d99c0-7034-450b-bced-75fc9bc60211)

### ANIM MONTAGE:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/a6f7ef63-ec7c-4204-8ab6-ba9d33d9e705)

### THIRD PERSON BLUEPRINT:
![image](https://github.com/Aashima02/Third-Person-Character-Mesh-/assets/93427086/3c670727-d315-422f-82db-0158cbc04960)

## RESULT:

The third person character mesh has been successfully changed using animations.
