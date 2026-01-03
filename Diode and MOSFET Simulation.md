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
<img width="1208" height="688" alt="Screenshot 2026-01-03 125725" src="https://github.com/user-attachments/assets/a52b7ee8-1de1-46c5-9f01-2bd2a03b233e" />
<img width="1096" height="846" alt="Screenshot 2026-01-03 125738" src="https://github.com/user-attachments/assets/30a8c07d-5222-4b09-be7a-cde7ae5c7529" />
<img width="2378" height="878" alt="Screenshot 2026-01-03 125809" src="https://github.com/user-attachments/assets/f6d980b0-9787-4f76-97c2-d8e20d90d25f" />
## Ideal MOS Capacitor:- energy band design
-  Since 1970s, for Si-based MOS --> ploy Si is sed as gate metal.
-  Since 2008, metal gate is being reintroduced with high -k dielectric.
<img width="2129" height="1233" alt="Screenshot 2026-01-03 130021" src="https://github.com/user-attachments/assets/be133c20-bf0d-4977-a6d5-4b93aed44866" />
## Flat Band Condition
- A negative voltage must be applied at the gate to achieve flat band at Si/SiO2
- Flat band voltage
<img width="1164" height="1315" alt="Screenshot 2026-01-03 130108" src="https://github.com/user-attachments/assets/ac74298d-16b8-43dd-b84a-f664a07970ce" />
<img width="2073" height="1346" alt="Screenshot 2026-01-03 130258" src="https://github.com/user-attachments/assets/3a6ca12b-e934-46b8-bf2c-6ba87327d058" />
## TCAD Based Analysis - Work Function
<img width="3344" height="1664" alt="Screenshot 2026-01-03 130427" src="https://github.com/user-attachments/assets/abbab32b-2387-4f67-835e-e2c2ab3a7dd7" />
## TCAD Based Analysis - Substrate Doping
<img width="3122" height="1675" alt="Screenshot 2026-01-03 130530" src="https://github.com/user-attachments/assets/1503d06f-6ce7-46eb-b6b1-0ea9da93ef51" />

## MOS Capacitor under Bias: Qualitative Analysis
<img width="3165" height="831" alt="Screenshot 2026-01-03 131042" src="https://github.com/user-attachments/assets/080941e1-0d4b-4024-acc0-3d644e894e57" />
- Application of negative potential on gate --> pulls the energy bands up.
- Ef-Ev reduces near the Si/So2 interface --> increase in hole density --> accumulation of majority cariers.
- Surface potential determines the hole density at the interface.
- Any increase in dQ charge on gate --> increase dQ charge at the interface.

<img width="3345" height="892" alt="Screenshot 2026-01-03 131231" src="https://github.com/user-attachments/assets/ce8986d3-d778-4ac6-b2f1-3db7bbd73e1f" />
- Application of small positive bias on gate --> pushes energy bands down.
- Ef-Ev increases Ef approaches Ei --> interface gets depleted of any free charge carriers.
- Applied charge balanced by ionized immobile acceptors.
- Increase in dQ charge on the gate --> increase depletion width.

<img width="3344" height="858" alt="Screenshot 2026-01-03 131947" src="https://github.com/user-attachments/assets/3dc60057-6718-4831-b0f9-4ecb48131145" />
- Higher positive bias on gate --> Ef moves closer to Ec --> increase in electron density (nsurf) at S/O interface + saturation of depletion width.
- At threshold voltage(Vth) nsurf = pbulk
- Electrons in p-si --> thermal generation --> slower process --> Q on gate --> increase in Qinv or Wdep (determined by speed of Operation)

## What does a MOS System do?
<img width="3256" height="872" alt="Screenshot 2026-01-03 132139" src="https://github.com/user-attachments/assets/8a2c779d-95e9-4ed9-b92d-55df40686362" />
- Gate voltage dependent modulation of the interface conductivity.
- Also changes the majority carrier type at the interface.

## MOS to MOSFETs
<img width="2821" height="1769" alt="Screenshot 2026-01-03 132610" src="https://github.com/user-attachments/assets/ca4b8731-7dec-4e18-9f9f-1e263f1d8994" />
## nMOSFET Band Diagram
<img width="2772" height="1194" alt="Screenshot 2026-01-03 132753" src="https://github.com/user-attachments/assets/b79290ec-42b8-450d-b1a3-ce011b098fac" />
## nMOSFET Operation
<img width="1471" height="1002" alt="Screenshot 2026-01-03 132826" src="https://github.com/user-attachments/assets/191d0bd2-bfc0-4f4a-b457-d2dac05d502f" />
- Accumulation region - hole channel connecting n+ regions!
<img width="1505" height="1015" alt="Screenshot 2026-01-03 132834" src="https://github.com/user-attachments/assets/26806224-38cc-4540-9054-213f656fe014" />
- Channel inversion - electron channel connecting n+ regions ! --> registors --> linear operation!!

## nMOSFET Operation: higher Vds
- MOS capacitor --> channel charge
  - a potential difference of Vt between the gate and channel!
- Near drain end, channel acquires potential equal to V<sub>DS</sub>
  - as V<sub>DS</sub> increases --> V<sub>g</sub>, drain end reduces
-  Channel turns off near drain end!
<img width="1554" height="1537" alt="Screenshot 2026-01-03 133445" src="https://github.com/user-attachments/assets/4253bab4-1658-49b3-bcaa-10671c2da6f4" />
Current can no longer increase with Vds! Loss of linear behaviour!
<img width="3287" height="1048" alt="Screenshot 2026-01-03 134125" src="https://github.com/user-attachments/assets/8015fb6f-8f57-4215-b1ac-c052962aadd3" />
Low V<sub>DS</sub>, uniform channel --> acts like a resistor
```
Resistance ∝ 1/μ x channel charge
```
Moderately high Vds, voltage drop across the oxide near drain current ↓, \Q'n| ↓, conductivity ↓, slope ↓
<img width="3342" height="937" alt="Screenshot 2026-01-03 134140" src="https://github.com/user-attachments/assets/507e381a-f46e-421f-9989-cf1465e2f044" />
V<sub>DS</sub> channel pinch-off near drain, slope ≈ 0
V<sub>GS</sub> - V<sub>DS</sub>(sat) = V<sub>T</sub> -->V<sub>DS</sub>(sat)=V<sub>GS</sub> - V<sub>T</sub>

V<sub>DS</sub> > V<sub>DS</sub>(sat), if change in channel length is small compared to original length I<sub>D</sub> will remain constant

## TCAD Based Characteristics
How pinch-off looks like
<img width="3280" height="1202" alt="Screenshot 2026-01-03 135200" src="https://github.com/user-attachments/assets/92326e36-93e0-46b0-8612-3973065d3c50" />

## MOSFET Operation - Quanlitative Analysis
Linear region drain current is given as 
I<sub>D</sub> = WμnCox/2L [2(V<sub>G</sub> - V<sub>T</sub>)V<sub>DS</sub> - V²<sub>DS</sub>] = k'n/2.W/L [2(V<sub>GS</sub> - V<sub>T</sub>)V<sub>DS</sub> - V²<sub>DS</sub>
k'n = μnCox is the process conductance parameter with unit of A/V²
kn = k'nW/2L is the conductance parameter

## TCAD Based Visualization
Formation of channel for V<sub>GS</sub> > V<sub>T</sub>(sat)
The current flow
<img width="3156" height="1069" alt="Screenshot 2026-01-03 135316" src="https://github.com/user-attachments/assets/9030cc0f-300f-46c9-a76c-9482a6fb71a3" />
What happens when we make the channel short?
<img width="3262" height="1231" alt="Screenshot 2026-01-03 142001" src="https://github.com/user-attachments/assets/686f2189-0709-472f-a8b6-f23535ee4b11" />
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

## How to simulate it 
<img width="1724" height="1155" alt="Screenshot 2026-01-03 142652" src="https://github.com/user-attachments/assets/46e8bc74-c8f1-43ab-972b-bb53702424a7" />
## Steps to generate the Structure
- Step 1 - create the substrate
- Step 2 - define the doping in the substrate
- Step 3 - create n-type doping windows for S/D use of ref/eval window
- Step 4 - defining gate
           overlapping boxes
           different boxes
<img width="1324" height="289" alt="Screenshot 2026-01-03 142820" src="https://github.com/user-attachments/assets/6faa3225-a242-4af3-8aee-fd77e8ea15fd" />
- Step 5 - defining contacts drain, gate and source
- Step 6 & 7 - placing contacts and meshing
<img width="1279" height="954" alt="Screenshot 2026-01-03 142801" src="https://github.com/user-attachments/assets/30acdda9-a8cd-45c4-b7f4-779a61c0179f" />
<img width="2356" height="430" alt="Screenshot 2026-01-03 142812" src="https://github.com/user-attachments/assets/d1038a1f-982c-47b6-a2ae-fcf74dead153" />

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
<img width="3328" height="1890" alt="Screenshot 2026-01-03 144122" src="https://github.com/user-attachments/assets/c60d144f-d2a1-4200-bec0-9cc76e848c71" />
## Todays Device: Bipolar Junction Transistors
<img width="2878" height="1605" alt="Screenshot 2026-01-03 144957" src="https://github.com/user-attachments/assets/b6d93dc3-c5f5-47f8-bdfa-6b6adf4ef269" />
## Energy Band Diagram 
- Any estimate on what will be the best way to extract current out of these devices?
- Large number of carriers in emitter? they should participate in conduction
- E-B junction barrier should be lowered!
- What about C-B junction? If we forward bias this as well flooding of carriers in the base junction
- Reverse bias
<img width="1529" height="1561" alt="Screenshot 2026-01-03 145130" src="https://github.com/user-attachments/assets/eab24152-d9fc-4e86-a6b9-b797ec444d0e" />
## Modes of Operation
Two different junctions --> four possible modes of operations
1) Both E-B and C-B junctions are reverse biased
<img width="1181" height="616" alt="Screenshot 2026-01-03 145710" src="https://github.com/user-attachments/assets/8fd7a9c2-48d0-4caf-95e8-967f588b173c" />
<img width="1307" height="1412" alt="Screenshot 2026-01-03 145703" src="https://github.com/user-attachments/assets/7e424d1a-48fa-4658-8c40-1aee3b8cc1e5" />
2) E-B forward biased and C-B is forward biased
<img width="1162" height="641" alt="Screenshot 2026-01-03 145828" src="https://github.com/user-attachments/assets/5d749653-ff1f-44a8-bd3e-8cfb21437e53" />
<img width="1278" height="1276" alt="Screenshot 2026-01-03 145936" src="https://github.com/user-attachments/assets/f51bce48-42e6-4a4f-9f5c-d319a676b44c" />
Huge electron injection from emitter and collector to base!! Base is designed to support minimum recombination --> saturation of base with electrons --> no gain out of the transistor
  


