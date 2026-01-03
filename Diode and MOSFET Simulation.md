## Why study Metal Oxide Semiconductors?
Their study enables designing capacitors on wafers for ICs.
<img width="3305" height="586" alt="Screenshot 2026-01-03 125113" src="https://github.com/user-attachments/assets/e7e1dd05-c0eb-461f-8d2d-0b4d805a9e8d" />
Forms a integral part of modern semiconductors devices
<img width="1795" height="533" alt="Screenshot 2026-01-03 125246" src="https://github.com/user-attachments/assets/d996d2fb-0fe2-4558-893f-448075fdd2ec" />
- Enables us to understand how transistor work.
- How gate modulates the channel conductivity.

## Ideal MOS Capacitor
- MOS capacitor is the heart of the MOSFET
- Analogous to parallel plate capacitor (Metal and Semiconductor separated by oxide/dielectric)
C' = E/d
Q' = C'/V
E = V/d

## Ideal MOS Capacitor:- energy band design
-  Since 1970s, for Si-based MOS --> ploy Si is sed as gate metal.
-  Since 2008, metal gate is being reintroduced with high -k dielectric.

## Flat Band Condition
- A negative voltage must be applied at the gate to achieve flat band at Si/SiO2
- Flat band voltage

## TCAD Based Analysis - Work Function

## TCAD Based Analysis - Substrate Doping

## MOS Capacitor under Bias: Qualitative Analysis

- Application of negative potential on gate --> pulls the energy bands up.
- Ef-Ev reduces near the Si/So2 interface --> increase in hole density --> accumulation of majority cariers.
- Surface potential determines the hole density at the interface.
- Any increase in dQ charge on gate --> increase dQ charge at the interface.

- Application of small positive bias on gate --> pushes energy bands down.
- Ef-Ev increases Ef approaches Ei --> interface gets depleted of any free charge carriers.
- Applied charge balanced by ionized immobile acceptors.
- Increase in dQ charge on the gate --> increase depletion width.

- Higher positive bias on gate --> Ef moves closer to Ec --> increase in electron density (nsurf) at S/O interface + saturation of depletion width.
- At threshold voltage(Vth) nsurf = pbulk
- Electrons in p-si --> thermal generation --> slower process --> Q on gate --> increase in Qinv or Wdep (determined by speed of Operation)

## What does a MOS System do?
- Gate voltage dependent modulation of the interface conductivity.
- Also changes the majority carrier type at the interface.

## MOS to MOSFETs
## nMOSFET Band Diagram
## nMOSFET Operation
- Accumulation region - hole channel connecting n+ regions!
- Channel inversion - electron channel connecting n+ regions ! --> registors --> linear operation!!

## nMOSFET Operation: higher Vds
- MOS capacitor --> channel charge
  - a potential difference of Vt between the gate and channel!
- Near drain end, channel acquires potential equal to V<sub>DS</sub>
  - as V<sub>DS</sub> increases --> V<sub>g</sub>, drain end reduces
-  Channel turns off near drain end!

Current can no longer increase with Vds! Loss of linear behaviour!
Low V<sub>DS</sub>, uniform channel --> acts like a resistor

```
Resistance ∝ 1/μ x channel charge
```
Moderately high Vds, voltage drop across the oxide near drain current ↓, \Q'n| ↓, conductivity ↓, slope ↓

V<sub>DS</sub> channel pinch-off near drain, slope ≈ 0
V<sub>GS</sub> - V<sub>DS</sub>(sat) = V<sub>T</sub> -->V<sub>DS</sub>(sat)=V<sub>GS</sub> - V<sub>T</sub>

V<sub>DS</sub> > V<sub>DS</sub>(sat), if change in channel length is small compared to original length I<sub>D</sub> will remain constant

## TCAD Based Characteristics
How pinch-off looks like

## MOSFET Operation - Quanlitative Analysis
Linear region drain current is given as 

I<sub>D</sub> = WμnCox/2L [2(V<sub>G</sub> - V<sub>T</sub>)V<sub>DS</sub> - V²<sub>DS</sub>] = k'n/2.W/L [2(V<sub>GS</sub> - V<sub>T</sub>)V<sub>DS</sub> - V²<sub>DS</sub>
k'n = μnCox is the process conductance parameter with unit of A/V²
kn = k'nW/2L is the conductance parameter

## TCAD Based Visualization
Formation of channel for V<sub>GS</sub> > V<sub>T</sub>(sat)
The current flow

What happens when we make the channel short?

Drain Induced Barrier Lowering --> even drain voltage can turn on the channel

## Device Performance Metrices Summary
1) On-current
2) Off-current
3) Channel Resistance
4) Output Reistance
5) Threshold Voltage
6) Drain Saturation Voltage
7) Subthreshold Swing s (mv/dec)
8) Drain Induced barrier lowering DIBL (mv/v)

How to simulate it 

## Steps to generate the Structure
- Step 1 - create the substrate
- Step 2 - define the doping in the substrate
- Step 3 - create n-type doping windows for S/D use of ref/eval window
- Step 4 - defining gate
           overlapping boxes
           different boxes
- Step 5 - defining contacts drain, gate and source
- Step 6 & 7 - placing contacts and meshing

- Creating the boundary
  - Creating rectangle for substrate
  - Creating rectangle for gate oxide and side wall oxide
- Defining doping
  - Constant Na doping in the complete substrate
  - Refinement definition
  - Refinement placement
- Constant Nd doping in the source and drain regions
  - Defining refinement/evaluation window
  - Refinement definition
  - Refinement placement
- Contact Definition
  - Placing source/drain/gate metal rectangles
  - Defining contact set: source, drain, gate, substrate
  - Setting source/drain/gate contacts at the region boundary edge
  - Setting buld constant at the bottom edge
- Meshing ]
  - Global mesh
  - Doping gradient dependent refinement (to capture doping variation as we move from source/drain to bulk)
  - Si/SiO2 interface refinement
  - Lateral refinement the channel region
  - Si/SiO2 to contact interface refinement

## Todays Device: Bipolar Junction Transistors

## Energy Band Diagram 
- Any estimate on what will be the best way to extract current out of these devices?
- Large number of carriers in emitter? they should participate in conduction
- E-B junction barrier should be lowered!
- What about C-B junction? If we forward bias this as well flooding of carriers in the base junction
- Reverse bias

## Modes of Operation
Two different junctions --> four possible modes of operations
1) Both E-B and C-B junctions are reverse biased
2) E-B forward biased and C-B is forward biased

Huge electron injection from emitter and collector to base!! Base is designed to support minimum recombination --> saturation of base with electrons --> no gain out of the transistor
  


