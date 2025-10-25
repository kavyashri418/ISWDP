# Introduction to Semiconductor Devices

## How to analyze any Semiconductor Device?
- Primary steps required to translate a device from textbook or idea to a TCAD simulation
- Start with intrinsic and extrinsic silicon bar, p-n junction diode and then proceed towards transistors
- First step in learning devices and their simulation

## Energy bands of materials

<img width="2137" height="1176" alt="Screenshot 2025-10-24 093714" src="https://github.com/user-attachments/assets/c67e8f55-e595-44ae-9074-771c97c831a3" />

Large Eg prohibits thermally excited electrons from moving to the conduction band

## What are Semiconductors
- Conductivity lies between that to insulators and conductors.
- Distinguish through band gap.
- Silicon (Group IV elemen) is widely used.
- Doping is used to modulate the conductivity
  - N-type dopant (V) electrons are the majority carriers
  - P-type dopant (III) holes are the majority carriers

## Analysing a Si Semiconductor bloack

<img width="3183" height="1450" alt="Screenshot 2025-10-24 095333" src="https://github.com/user-attachments/assets/f28f6783-78f2-4c6f-834b-6e2fbea9de45" />

## How does the carrier concentration vary with Temperature

Case I: T = 0K

<img width="1765" height="837" alt="Screenshot 2025-10-24 095733" src="https://github.com/user-attachments/assets/adf81937-87cf-40ec-95e3-accb405b563b" />

No extrinsic carriers due to doping, and no intrinsic carriers due to thermal excitation across the band gap.

Case II: T > 0K (Low Temperature)

<img width="1736" height="808" alt="Screenshot 2025-10-24 100832" src="https://github.com/user-attachments/assets/e6ab43e3-9b7b-442e-aa06-eb14b042d8ea" />

A few extrinsic carriers due to doping, but no intrinsic carriers due to thermal excitation across the band gap.

Case III: T = 300K

<img width="1758" height="827" alt="Screenshot 2025-10-24 100913" src="https://github.com/user-attachments/assets/8c522292-2cdc-4da8-ae15-46f1a44d4fbe" />

Many extrinsic carriers due to doping, but very few intrinsic carriers due to thermal excitation across the band gap.

Case IV: T >> 300K (High Temperature)

<img width="1885" height="939" alt="Screenshot 2025-10-24 101329" src="https://github.com/user-attachments/assets/5269e190-65fe-446c-b143-65255f917ca3" />

Extrinsic carriers due to doping, but also many intrinsic carriers due to thermal excitation across the band gap also many holes in the valence band now.

## Fermi-Level for Extrinsic Semiconductor

<img width="3330" height="940" alt="Screenshot 2025-10-24 102041" src="https://github.com/user-attachments/assets/1b124ccd-7eca-4e09-a5d8-efceb26beb05" />

Fermi-Level (Ef) = average energy of electrons in a material, the fermi-dirac distribution, f(E) gives the probability that a state having energy E is occupied by an electron

## Impact of Doping on Energy Band Diagram

<img width="3239" height="1397" alt="Screenshot 2025-10-24 103639" src="https://github.com/user-attachments/assets/bfa60b80-955d-4a3a-9abb-82ca85b791ae" />

## How current flows through the semiconductor?
Current density J = σE
- E = applied electric field
- σ = conductivity
- q = electronic charge
- n = electron / hole density
- 𝜇 = mobility

## Mobility vs Doping

<img width="2027" height="1341" alt="Screenshot 2025-10-24 105050" src="https://github.com/user-attachments/assets/21473e51-3377-4921-9e34-3d73bd71441c" />

## Ionized Impurity Scattering

<img width="1274" height="699" alt="Screenshot 2025-10-24 105104" src="https://github.com/user-attachments/assets/385b8b51-f0fe-46d4-a91c-04377b461d24" />

Donors provide electrons to the conduction band but ionized donors can "scatter" those electrons
Analyzing a Si semiconductor bar σ = qn𝜇
- n = free carrier mobility

How can we increase the current for a given voltages?
Increase conductivity, increase 𝜇 or n
Increase n will reduce mobility less promient increase in current

Note - These relations and a linear increase in current holds only for low electric field

## What is Mobility?
- In the world of semiconductor devices, electron mobility plays a crucial role.
- It refers to the speed at which an electron moves through a material when subjected to an electric field.
- The lighter the mobility of electrons in a material the faster they can move, and the faster the device can operate.
- This makes it an important factor in the design of electronic devices as it affects their speed, power consumption.

## Mobility vs Temperature

<img width="3249" height="1326" alt="Screenshot 2025-10-24 111001" src="https://github.com/user-attachments/assets/723efef0-f3cf-43fb-91ed-3be63b4b8e31" />
<img width="1420" height="413" alt="Screenshot 2025-10-24 112506" src="https://github.com/user-attachments/assets/5f7c3232-b5dc-4454-a928-d856d93e3068" />

## Velocity and Electric field

<img width="3341" height="1597" alt="Screenshot 2025-10-24 111359" src="https://github.com/user-attachments/assets/1cbb5c41-4fe8-4eec-a8b3-4872edcf5af1" />

## Understanding the complexities of physical models

Case I: A lower node current as compared to electron current.

<img width="1864" height="724" alt="Screenshot 2025-10-24 112357" src="https://github.com/user-attachments/assets/646d1bc7-0803-4f87-99d0-347f4aeb8d61" />

Case II: Everything looks prefect we can visualize the impact of n on mobility and current.

<img width="1875" height="694" alt="Screenshot 2025-10-24 112444" src="https://github.com/user-attachments/assets/9e18bae5-f1f1-4ac8-9ca3-9ffaa20a7a1b" />

What happens at high electric fields to velocity saturation effect
Current should have saturated doesnot happen 
Physics section and the operator's understanding of device physics is critical.

<img width="3023" height="1015" alt="Screenshot 2025-10-24 112624" src="https://github.com/user-attachments/assets/25f68a90-2dbf-4487-995d-d2db10d19ee8" />
