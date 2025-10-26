## Introduction to Structure Editor (SDE)

- Uses a drag drop approach as in paint.
- Materials specification of objects, basic 2D/3D shapes boolean operations for complex shapes.
- Doping definitions like, constant, gaussian or even a user defined function.
- Advanced structure editing like rounding of edges, or proces emulation of etching.
- It supports script.

<img width="3306" height="1823" alt="Screenshot 2025-10-26 124451" src="https://github.com/user-attachments/assets/51834357-a243-40ab-b273-dc628b2c7db6" />

## How do we start?

- Compute device structure and doping
   example a block of doped silicon
- Exact co-ordinates of diagonally opposite ends for creating rectangle.
- Region names - only one region here, situation can be complex in modern day devices.

## Steps to create a structure

Step 1 - create the boundary of the structure, clearly defining the shapes size and the materials used.
Step 2 - define the doping in different regions of the structure, species, profile and concentration are parameters.

<img width="1346" height="1510" alt="Screenshot 2025-10-26 125212" src="https://github.com/user-attachments/assets/45b14321-614b-42a8-bf6c-a3f140a7de5b" />

## Defining Doping

- Need to define substrate doping
- Three options for placement material wise, region wise, refinement window wise.
  - select material --> silicon or region --> substrate
- Constant profile definition --> doping details
  - Name --> name of the definition
  - Species --> doping species --> boron active concentration
- Click on add placement.

## Defining Contacts

- First define contact sets.
- Defined contacts will then appear in the contact list.

<img width="1975" height="1181" alt="Screenshot 2025-10-26 131004" src="https://github.com/user-attachments/assets/b9a60a86-6204-4cdd-b186-54563fc9ef2c" />

## Setting Contacts

- Select "A" from contact list.
  - In the selection list section "select edge".
  - Select the selection tool from bar.
  - Now select the top edge.
  - Now go to contacts --> set contact.
- Select "B" from contact list
  - In the selection list select "select edge".
  - Select the selection tool from tool bar.
  - Now select the top edge.
  - Now go to contacts --> set contact.
 
<img width="1588" height="1098" alt="Screenshot 2025-10-26 131142" src="https://github.com/user-attachments/assets/262c70ff-122e-4a8c-b4dc-161f3551d799" />

## What is meant by where to solve the equations ?

- Apply Vab and the find out current, potential distribution, electric field.
- Three basics equations
  - Gauss's law --> poisson equation
  - Electron transport equation
  - Hole transport equation
- Boundary conditions --> determined by the boundaries where we expect maximum change the happen
- How will simulator know --> meshing

<img width="1314" height="1582" alt="Screenshot 2025-10-26 131554" src="https://github.com/user-attachments/assets/b53fef8a-3d11-478e-ab1c-5ca34dcd7f4b" />

## Meshing

- A single semiconductor block --> easier meshing

Steps for meshing
1 Define a refinement window.
2 Mention x,y and z refinements any other.
3 Create placement
4 Build mesh.

## Measuring Device Behavior

- Different physics comes into picture in different devices!
- There cannt be a common set of equations to solve all the semiconductor behavior.
- User has to specify which physics models to use.

<img width="1074" height="927" alt="Screenshot 2025-10-26 133149" src="https://github.com/user-attachments/assets/6579f7e2-3ab9-4811-8c8b-e4a0566f154e" />

<img width="2140" height="1018" alt="Screenshot 2025-10-26 133221" src="https://github.com/user-attachments/assets/0c40da2e-5e8e-4bf5-ac33-8f89bf72d2c3" />

## Basic Command File Generation

To define the sdevice input command file (command_des.cmd) the following steps need to be followed
- Define input/output node file.
- Define physical contacts (electrode).
- Define physical models in various design regions.
- Define scalar and vector entities to be visualized.
- Define flags and solves for smoother computation.
- Define system (if mixed mode transient/CV simulations)
- Define bias conditions, solve coupled poisson and continuity equations and save solutions.

<img width="1580" height="1123" alt="Screenshot 2025-10-26 133800" src="https://github.com/user-attachments/assets/ac159833-8e80-4496-beae-5cbecbe3a8ab" />

## Command File - File Section

File - contains specifications of all the input and output files.
Grid file (.tdr format) - contains address of the input file containing devices structure with meshing doping and stress information.

- Parameter file (.par file) - material parameters.
- Current file (.plt format) - output file containing electrode names and resulting voltages, currents, charges, times and temperature.
- Plot file (_des tdr format) - contacts the 2D/3D output structure of the device in the form of a tdr file.
- Output file (_des log format) - log file that stores the simulator runtime data generated during the simulation.

<img width="1542" height="774" alt="Screenshot 2025-10-26 134908" src="https://github.com/user-attachments/assets/e0f0cc5a-86d1-40fa-af89-551eaecd7c32" />

Name - specified the name of the contact in the input structure (*_msh.tdr) file. The specified name should match a contact in the tdr file.
Note - even if there is a contact in the input tdr file and it is not declared in the electrode section here, it doesnot exist for the device simulator.

Voltage - specifies the initial voltages to be applied to the contact. It can be current boundary condition as well.
- Models are pre-defined in TCAD.
- Customizations can be done using PMI interfaces.
- Can also be declared region wise or material wise.

Math section - deals with solvers used for solving the suggested physical equations.
Plot section - specifies which scalar or vector values should be stored in the output tdr file.

<img width="1203" height="1051" alt="Screenshot 2025-10-26 140840" src="https://github.com/user-attachments/assets/a0ccde5c-7a43-4378-9b6f-8430ec5c6140" />

## Command File - Solve Section
This section actually applies the specified excitation and measures the response of the device.

Task - sweep Vab from -20 to 20V and measure the output current.

<img width="2025" height="1415" alt="Screenshot 2025-10-26 141113" src="https://github.com/user-attachments/assets/c897c05f-19e6-45ca-b500-a4be11093af8" />

