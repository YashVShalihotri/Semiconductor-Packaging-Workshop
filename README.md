# Semiconductor Packaging workshop
Notes summarized for the Semiconductor workshop attended between 9th and 18th May 2025

## 1.	Packaging Evolution: From Basics to 3D Integration
        1. Introduction to Semiconductor Packaging and Industry Overview
        2. Understanding Package Requirements and Foundational Package Types
        3. Evolving Package Architectures from Single-chip to Multi-chip modules
        4. Interposers, Redistribution layer, and 3D Packaging Approaches
        5. Comparative Analysis and Selecting the Right Packaging Solution
## 2.	From Wafer to Package: Assembly and Manufacturing Essentials
    	1. Setting the Stage: Supply Chain and Facilities
    	2. Wafer pre-preparation: Grinding and Dicing
    	3. Wire Bond Packaging: Die attach to Molding
    	4. Flip Chip Assembly: Bump Formation and Underfill
    	5. Wafer Level Packaging And Conclusion
## 3.	Labs: Thermal Simulation of Semiconductor Packages with ANSYS
    	1. Introduction And Getting Started With ANSYS Electronics Desktop
    	2. Setting Up A Flip-Chip BGA Package
    	3. Material Definitions And Thermal Power Sources
    	4. Meshing And Running The Thermal Analysis
    	5. Summary
## 4.	Ensuring Package Reliability: Testing and Performance Validation
    	1. Introduction to Package Testing and Electrical Functionality Checks
    	2. Reliability and Performance Testing of Semiconductor Packages
## 5.	Package Design and Modeling: Building a Semiconductor Package from Scratch
    	1. Introduction to Package Cross-Section Modeling in ANSYS Electronics Desktop
    	2. Creating the Die and Substrate in AEDT
    	3. Adding Die Attach Material and Bond Pads
    	4. Wire Bond Creation and Material Assignment
    	5. Applying Mold Compound and Finalizing the Package Model
## 6.	Conclusion: Semiconductor Packaging


# 1. Packaging Evolution: From Basics to 3D Integration
## 1.1 Introduction to Semiconductor Packaging and Industry Overview
Semiconductor Packaging is needed to package the dies that come out of the wafer in a controlled environment of a clean room to be used in the real world.
Packaging is necessary to protect them from the environment and connect them to the real world.
Packaging helps in the following ways-
1. Protect the die from the environment and give it mechanical support (moisture, physical damage)
2. Electrical connections to the outer world.
3. Heat dissipation
           
![1](./Packaging/1.png)

### Package and Testing Industry
Companies are working in various sectors of the semiconductor industry.
1. **Fabless**: That only designs the chip.
2. **Foundry**: That takes the design and fabricates dies on the wafer, but does not design the chip
3. **IDM(Integrated Device Manufacturer)**: That does both designing and fabrication of the chip
4. **OSAT(Outsource Semiconductor Assembly and Test)**: That takes the dies from the wafer and packages them; they do not design or fabricate chips. 
![2](./Packaging/2.png)

## 1.2 Understanding Package Requirements and Foundational Package Types
### How to choose a package
Based on the listed requirements, packages are chosen for the packaging of the die.
<br>
![3](./Packaging/3.png)
### Typical Thermal Package Structure
This consists of die, mold compound, carrier, and System board(PCB).
Broadly speaking, there are two types of mounting technology on the System board
1. Through-hole mount technology: Pins are inserted in the system board.
2. Surface mount technology: Component leads are soldered to the surface-mounted pads instead of insertion.
![4](./Packaging/4.png)

## 1.3 Evolving Package Architectures from Single-chip to Multi-chip modules
## Anatomy of Package
### Lead Frame-based packages
A leadframe is a thin sheet of metal, typically copper or a copper alloy, that creates a die pad and leads for the outer world connection.
1. **Die Pad**: Area where the silicon die is mounted.
2. **Leads**: Serve as electrical connections between the die and the external PCB.
### Leadframe-type packages have
1. **Silicon die**
2. **Die attach** material that sticks the die onto the substrate.
3. **Wire bonds** that connect the die pads to leads for outerworld connection.
4. **Encapsulation** that surrounds all these components for safety, made using epoxy resin.
5. **Leads** the metal that extends out of this geometry.
### Common Lead-frame Package
1. **DIP (Dual In-line Package)** has pins that go into the PCB on both sides of its packaging, which is rectangular.
2. **QFP (Quad Flat Package)** Four-sided surface-mount package with fine-pitch leads on all sides.
3. **QFN (Quad Flat No-lead)** Exposed pad package without leads; pads are on the bottom for better thermal and electrical performance.
4. **DFN (Dual Flat No-lead)** Like QFN but with pads only on two sides. Very compact.

### Laminate-based Package
A laminate-based package has a multi-layer organic substrate rather than a metal leadframe.
### Common Laminate-Based Package Types
1. **Wire Bond PBGA (Plastic Ball Grid Array)** Die is connected via wirebonds to a laminated substrate with solder balls for board attachment.
2. **Flip Chip PBGA** Die is flipped and directly bonded to the substrate using solder bumps.
3. **LGA (Land Grid Array)** flat contacts for direct connection; no solder balls are used.

### Advanced package substrates
These packages are made for a larger number of dies on the same substrate, which gives high I/O pins and has lots of interconnection layers.
1. **2D**: Multiple dies placed side by side on a single substrate (FCBGA). Since there is no redistribution layer in this, the dies have a  longer path between them.
2. **2.1D**: Similar to 2D but includes RDL (Redistribution Layer) to improve routing and integration.
3. **2.3D**: Uses organic interposer to connect dies.
4. **2.5D**: Instead of Organic, a silicon interposer for high-speed interconnects between dies.
![5](./Packaging/5.png)

## 1.4 Interposers, Redistribution layer, and 3D Packaging Approaches
1. Redistribution Layers (RDL) is a metal layer added on top of a die or wafer to reroute the I/O pads to new locations. Connects different dies on the substrate, as without RDL, it takes longer for the dies to communicate with each other.
2. Interposer: Acts as an intermediate routing interface between the die and the substrate.
Silicon as an interposer reduces mechanical stress between the die and substrate as it has the same CTE as of die.
![6](./Packaging/6.png)
Nomenclature for the packages.
## 1.5 Comparative Analysis and Selecting the Right Packaging Solution
Different packages have different advantages and disadvantages, and uses, as can be seen from the image.
![7](./Packaging/7.png)

# 2 From Wafer to Package: Assembly and Manufacturing Essentials
## 2.1 Setting the Stage: Supply Chain and Facilities
![8](./Packaging/8.png)
