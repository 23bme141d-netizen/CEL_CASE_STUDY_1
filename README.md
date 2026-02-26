Node Voltage Analysis of a Multi-Node DC Circuit using MATLAB

->Project Overview
This project focuses on determining the unknown node voltages of a multi-node DC resistor network using Kirchhoff’s Current Law (KCL) and computational analysis in MATLAB.

The node voltage solution is obtained when: • Kirchhoff’s Current Law is satisfied at each node • Ohm’s Law relations between connected nodes are maintained

This project demonstrates how numerical computation and matrix formulation can be used to analyse linear electrical networks efficiently using MATLAB.
⸻
->Objective
The main objectives of this project are: • To understand the concept of node voltage analysis • To apply Kirchhoff’s Current Law (KCL) • To formulate linear equations for a multi-node DC circuit • To convert circuit equations into matrix form • To determine node voltages using MATLAB • To verify circuit behaviour using computational tools
⸻
->Problem Description
A DC circuit consisting of: • A DC voltage source• Six resistors• Four essential nodes is analysed to determine the steady-state voltages at each node.
The resistor values used are typical practical values: • R₁ = 1 kΩ • R₂ = 2.2 kΩ • R₃ = 820 Ω • R₄ = 220 Ω • R₅ = 470 Ω • R₆ = 330 Ω
The source voltage is assumed to be 8 V under steady-state DC conditions.
⸻
->Mathematical Formulation
Node Voltage Definition
Let:
• Ground voltage = 0 V
• V₁ = Vₛ (connected directly to the voltage source)
• Unknown node voltages = V₂, V₃, V₄
Kirchhoff’s Current Law
At any node:
Σ I = 0
Using Ohm’s Law:
I = (Vᵢ − Vⱼ) / R
Node 2 Equation
(V₂ − V₁)/R₂ + (V₂ − V₃)/R₃ + (V₂ − V₄)/R₄ = 0
Node 3 Equation
(V₃ − V₁)/R₁ + (V₃ − V₂)/R₃ + (V₃ − V₄)/R₆ = 0
Node 4 Equation
(V₄ − 0)/R₅ + (V₄ − V₂)/R₄ + (V₄ − V₃)/R₆ = 0
Matrix Form
The system of equations can be written in compact form:
A V = B
Where V = [ V₂ V₃ V₄ ]ᵀ
Matrix A is formed using conductance values (1/R), and vector B contains source contributions from Vₛ.
⸻
->Methodology
The node voltages are determined using a computational approach: 1.Define source voltage and resistor values 2. Convert resistances to conductance's 3. Form the coefficient matrix 4. Construct the source vector 5. Solve the linear system in MATLAB 6. Display the computed node voltages
⸻
->MATLAB Implementation
The MATLAB script performs: • Definition of circuit parameters • Formation of conductance matrix • Construction of source vector • Solving linear equations using the backslash operator • Displaying node voltages
⸻
->Results
The computational analysis yields: • V₁ = 8.000 V• V₂ = 3.456 V• V₃ = 3.978 V• V₄ = 2.861 V
These results satisfy Kirchhoff’s Current Law at each node and represent the steady-state behavior of the circuit.
⸻
->Key Concepts Demonstrated
This project illustrates the application of: • Kirchhoff’s Current Law • Node voltage method • Linear equation modeling • Matrix formulation • MATLAB computational solving • Electrical network analysis
⸻
->Engineering Significance
Node voltage analysis is essential in: • Electronic circuit design• Power distribution systems• Embedded system development • Control systems • Electrical network modelling

This project highlights the importance of computational methods in solving linear multi-node engineering problems.
⸻
->How to Run the Project 1. Open MATLAB 2. Copy the provided .m script 3.Run the file 4. Observe • Computed node voltages
⸻
Author
Dhruv Patel 3rd Year Mechanical Engineering Student Computational Engineering Laboratory Project
⸻
Project Summary
This project successfully demonstrates how the node voltage method can be used to determine unknown voltages in a multi-node DC circuit using computational matrix techniques.
It reinforces the role of numerical methods and MATLAB in modern engineering circuit analysis.
