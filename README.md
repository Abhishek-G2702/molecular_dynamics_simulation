# molecular_dynamics_simulation:
This repository contains the data and analysis scripts for a Molecular Dynamics (MD) simulation of the 5EE2 protein. The primary goal of this project was to investigate the structural stability and dynamic behavior of the protein under specific simulated conditions.

🎯 Objective:
To study the conformation and energy of the 5EE2 protein using molecular dynamics and simulation methods.

 Tools Used:
GROMACS (Version 2020–2023)

VMD (Visual Molecular Dynamics)

Xmgrace (for plotting)

📁 File Descriptions
.gro: Structure file containing atomic coordinates and box dimensions

.top: Topology file defining molecular structure and force field parameters

.itp: Include topology file (e.g., position restraints)

.mdp: Molecular dynamics parameters file

.tpr: Binary input file for simulation

.xtc: Trajectory file

.xvg: Data file for plotting

 Procedure Steps
1. Protein Preparation
Downloaded PDB ID: 5EE2

Removed water molecules and ligands

Generated topology and structure files using pdb2gmx

2. System Setup
Defined a cubic box around the protein

Solvated the system with water molecules

Added ions to neutralize the system

3. Energy Minimization
Minimized the system energy to remove steric clashes

Verified convergence using potential energy plots

4. Equilibration
NVT Equilibration: Constant Number, Volume, and Temperature

NPT Equilibration: Constant Number, Pressure, and Temperature

Monitored temperature and pressure stability

5. Production MD
Ran a 100 ps production simulation

Saved trajectory for analysis

6. Analysis
Removed periodic boundary conditions from trajectory

Calculated RMSD (Root Mean Square Deviation)

Calculated Radius of Gyration

Visualized results using VMD and Xmgrace

📊 Results
The protein 5EE2 remained stable throughout the simulation

Low RMSD values indicate minimal structural deviation

Consistent radius of gyration suggests maintained compactness

Stable hydrogen bonding confirms structural integrity

 How to Run
Ensure GROMACS and VMD are installed

Clone this repository

Follow the command sequence as in the documentation

Use provided .mdp files for parameter settings

 Visualization
Use VMD to visualize the trajectory

Use Xmgrace to plot energy, temperature, RMSD, and gyration graphs

✅ Conclusion
The MD simulation confirms that the 5EE2 protein is structurally stable under the simulated conditions, supporting its potential biological functionality.

