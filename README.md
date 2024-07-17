**Welcome to DFT-Turbomole, a WaNo designed for predicting hyperpolarizabilities in molecules. Our workflow leverages Density Functional Theory (DFT) calculations using the Turbomole software suite. This WaNo enables efficient computation and screening of hyperpolarizabilities across a diverse range of molecular structures.**
---
# DFT-Turbomole WaNo

The DFT-Turbomole WANO is a workflow automation tool designed for computational chemistry tasks, focusing primarily on hyperpolarizability calculations. This tool facilitates the calculation of various molecular properties, including:
- Geometry optimization
- Frequency calculation
- Excited state calculation
- Hyperpolarizability calculation

These calculations can be performed for molecules in both gas phase and solution environments. However, the primary purpose of this workflow automation tool is to streamline hyperpolarizability calculations, aiding in the screening and assessment of molecular candidates for applications in nonlinear optics and related fields. The only needed input file is xyz structure of the molecule.

![Alt Text](dft.png)

# Parameters
In this section, we will explain each of the following parameters in detail:
- **Title:** Provide the title of the calculation or project.
- Molecular Structure
    - **Structure file type:** Specify the type of structure file being used (XYZ, Turbomole coord, Gaussian input).
    - **Structure file:** The actual structure file containing the molecular coordinates.
    - **Internal coordinates:** Information on the internal coordinates used for defining the molecule.
- Basis set
    - **Basis set type:** Specify the type of basis set employed in the calculation.
- Initial guess
    - Charge
    - Multiplicity
- DFT options
    - Max SCF iterations
    - Use RI
    - Memory for RI
    - Functional
    - Integration grid
    - vdw correction
    - COSMO calculation
- Type of calculation
    - Structure optimization
    - Excited states calculation
    - Hyperpolarizability
    - Frequency calculation
    - Plot HOMO-LUMO orbt
