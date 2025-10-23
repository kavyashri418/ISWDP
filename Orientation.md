### Semiconductors, their importance, complexities and how its developed?

### Reducing form factor, increasing functionality, increased design complexity, increased necessity of knowledge transfer and skill development

### What keeps the semiconductor development rolling?

Cutting edge research
- New device structure --> paradigm shift from planar to 3D structures, finFETs, HEMTs
- New materials integrations, like strained Si:Ge for enhanced mobility, shifting to wide band gap semiconductors like GaN, SiC, Diamond
- Moving to 2D and even single atom devices

Reliability improvements through innovation
Improved understanding of physical mechanisms
Bringing down cost of research, development and production

### Understanding Device Design

### A step ahead - designing of a diode

### Design seems complex?
Recombination current at lower forward biases

### Should we increase complexity? 

### Designing Planar MOSFET

What happens if we increases Na?
- Affects Qsd --> can tune Vt, body effect
- Increase electric field near drain --> early failure and reliability concerns

Reducing Na
- Reduced field near drain edge
- Increased voltage drop in substrate --> false triggering of the parasitic BJT --> failure
- Punch through --> more promient in short channel devices
- Trade off between realiability and performance

### Designing Planar MOSFET

### Should we try and increase complexity further?

- Non planar structure? FinFETs
 - The potential distribution, electric fields and carrier densities will have to be analyzed in 3-dimensions
 - Correlated design parameters --> simultaneous optimization --> exponentially increasing design time
- What happens when we integrate different materials?
 - Different band gap, different mobility formation of quantum well

### Is Understandiong Device Design Enough?

- Process challenges in fabricating modern-day devices
- The process limitation induced impact on device design
- The device design has to take into account the exact device structure
- Ion implementation the trade off between doping control, cost and crystal damage

### Typical Semiconductor Device Development Cycle

### TCAD Based Approach : Addressing these challenges

First hand generation of any novel structure 
Simulation time a few minutes quick conceptualized and testing
Fab process simulator effectively simulates different fabrication process steps including etching , ion implementation induced doped profile, damage, the impact of annealing temperature on dopant diffusion and stress profiles


### Device Simulator - DC, AC, Transient performance and reliability analysis, device circuit co-simulation

### TCAD - Technology Computer Aided Design

What is process simulation?

- Virtual representation or simulation of the manufacturing process of semiconductor chips
  - focused on the smallest building blocks the individual transistor and their immediate environment

- Sentaurus Process
  - focused on doping implant and diffusion and oxidation
  - more phenomenological on etching and deposition

 - DOPING - locally doping the electrical properties of the semiconductor
 - IMPLANTING - "shooting" ions the semiconductor
 - DIFFUSION / ANNEALING - heat treatment to drive the ions in deeper, activate them, and to heal damage
 - OXIDATION - turning a semiconductor into an insulator
 - ETCHING - removing material with either reactive ions or solvents
 - DEPOSITION - growing material typical from compounds in the gas environment
 - MASKING - using the layout like a masking tape to expose or protect certain area
Process flow description are input to process simulation

### Ion Implantation

- Ion implantation into on axis crystals leads to many ions experiencing small angle scattering and channel deep into the crystal
- Their stopping is then dominated by electronic drag only, which results in a channeling tail
- The resultant profile is described by a "dual - pearson distribution"

Tilting the wafer reduces channeling

Implantation through a thin oxide also reduces channeling

### Diffusion

- Diffusion is modelled either modelled atomistic or in a continum with a set of partial differential equation


In the kick out mechanisms, self interstitials kick out substitutional dopants

In the frank mechanisms, interstitial dopants or dopant interstiatial pairs occupy vacant sites and become substitutional dopants

### Sentaurus Process Simulator

- General purpose multidimensional (2D/3D) process simulator
- Integrated 3D geometric modelling engine
- API for user defined models
- Advanced physical models
  - Analytic and Monte Carlo implantation
  - Diffusion - laser/flash annealing, kinetic monte carlo
  - Mechanical stress
  - Oxidation
  - Geometric deposition and etching
 
### Sentaurus Structure Editor

- Geometric operations
- Easy to use GUI
- Scripting language
- Adavanced geometrical modeling with analytic doping definitions
- Direct interface to meshing engines

### Prcoess Explorer

- From layout files and process step description process explorer builds high-fidelity topographical 3D models allowing DOE creation based on a collaborative database
- Key capabilities
  - GUI and batch support
  - Support for large layouts
  - Fast turn around time
- Advantages
  - Collaborative environment
  - Different technologies
  - Value links with TCAD
 
### What is Device Simulation?

 - Virtual tests of the electrical and thermal behavior of the transistor
 - Focused on the smallest building blocks the individual transistor and their immediate environment
 - Solving drift - diffusion transport equations poisson + carrier continuity equation
 - Can solve the heat transport equation

### Sentaurus Device Simulator

- General purpose multidimensional (2D/3D) device simulator
- Silicon and compound semiconductors
- Mixed mode simulation TCAD devices in a SPICE circuit
- Drift diffusion, hydrodynamic and Monte Carlo transport
- Wide range of advanced physical models
  - Strained silicon mobility enhancement
  - Quantization and random doping effects
  - Non - volatile memory operation
  - Optics-raytracing and more

### Sentaurus Workbench

- TCAD framework environment
- Project management
- Design of experiments and optimizations
- Job framing

### Sentaurus Visual - TCAD Data Visualizer

- Enhanced GUI experiences
  - 2D/3D fields
  - X-Y data
  - S-parameter plots
  - Overlay and difference plots
- Powerful scripting capabilities
  - Python and TCL

 ### Synopsys TCAD Product Family


