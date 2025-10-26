## Introduction to Structure Editor (SDE)

- Uses a drag drop approach as in paint.
- Materials specification of objects, basic 2D/3D shapes boolean operations for complex shapes.
- Doping definitions like, constant, gaussian or even a user defined function.
- Advanced structure editing like rounding of edges, or proces emulation of etching.
- It supports script.

## How do we start?

- Compute device structure and doping
   example a block of doped silicon
- Exact co-ordinates of diagonally opposite ends for creating rectangle.
- Region names - only one region here, situation can be complex in modern day devices.

## Steps to create a structure

Step 1 - create the boundary of the structure, clearly defining the shapes size and the materials used.
Step 2 - define the doping in different regions of the structure, species, profile and concentration are parameters.

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
