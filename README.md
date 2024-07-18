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
- **Molecular Structure**
    - _**Structure file type:**_ Specify the type of structure file being used (XYZ, Turbomole coord, Gaussian input).
    - _**Structure file:**_ The actual structure file containing the molecular coordinates.
    - **Internal coordinates:** Information on the internal coordinates used for defining the molecule.
- Basis set
    - **Basis set type:** Specify the type of basis set employed in the calculation.
- Initial guess
    - Charge: Indicate the total charge of the molecule.
    - Multiplicity: Specify the multiplicity of the molecule.
- DFT options
    - Max SCF iterations: Set the maximum number of SCF (Self-Consistent Field) iterations.
    - Use RI: Specify whether the RI (Resolution of Identity) approximation is used.
    - Memory for RI: Allocate memory for RI calculations.
    - Functional: Specify the DFT functional used.
    - Integration grid: Define the integration grid used for the DFT calculations.
    - vdw correction: Indicate if van der Waals correction is needed.
    - COSMO calculation: Specify if COSMO calculations are needed.
- Type of calculation
    - Structure optimization: Performing geometry optimization if you select this option. The final structure will be stored in the output directory.
    - Excited states calculation: Computing the electronic states of a molecule that are higher in energy than the ground state using the Time-Dependent Density Functional Theory (TD-DFT) method.
    - Hyperpolarizability: DFT-Turbomole is able to calculate the first hyperpolarizability for both static and dynamic frequencies. By default, Turbomole calculates the first hyperpolarizability for the second harmonic generation case. However, this WaNo is designed to calculate hyperpolarizability for the Pockels effect as well.
    - Frequency calculation: Calculate second derivatives of the energy with respect to nuclear positions. This can be chosen either with the structure optimization parameter or alone.
    - Plot HOMO-LUMO orbt:  If you need to see the frontier orbitals, selecting this parameter will calculate the related cube files.
