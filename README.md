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
   
![Picture1](./Packaging/image1.png)

**Package and Testing Industry**
Companies are working in various sectors of the semiconductor industry.
1. **Fabless**: That only designs the chip.
2. **Foundry**: That takes the design and fabricates dies on the wafer, but does not design the chip
3. **IDM(Integrated Device Manufacturer)**: That does both designing and fabrication of the chip
4. **OSAT(Outsource Semiconductor Assembly and Test)**: That takes the dies from the wafer and packages them; they do not design or fabricate chips. 
![Picture2](./Package/image2.png)

