**Welcome to DFT-Turbomole, a WaNo designed for predicting hyperpolarizability in molecules. Our workflow leverages Density Functional Theory (DFT) calculations using the Turbomole software suite. This WaNo enables efficient computation and screening of hyperpolarizability across a diverse range of molecular structures.**
---
# DFT-Turbomole WaNo

The DFT-Turbomole WANO is a workflow automation tool designed for computational chemistry tasks, focusing primarily on hyperpolarizability calculations. This tool facilitates the calculation of various molecular properties, including:
- Geometry optimization
- Frequency calculation
- Excited state calculation
- Hyperpolarizability calculation

These calculations can be performed for molecules in both gas phase and solution environments. However, the primary purpose of this workflow automation tool is to streamline hyperpolarizability calculations, aiding in the screening and assessment of molecular candidates for applications in nonlinear optics and related fields. Figure 1 depicts the workflow layout.
![Alt Text](images/wano1.png)

<figure align="center">
    <img src="images/wano1.png" alt="Example Image" width="300">
    <figcaption>Figure 1: This is an example image caption</figcaption>
</figure>

# Parameters
In this section, we will explain each of the following parameters in detail:
- **Title:** Provide the title of the calculation or project.
- **Molecular Structure**
    - _**Structure file type:**_ Specify the type of structure file being used (XYZ, Turbomole coord, Gaussian input).
    - _**Structure file:**_ The actual structure file containing the molecular coordinates.
    - _**Internal coordinates:**_ Information on the internal coordinates used for defining the molecule.
- **Basis set**
    - _**Basis set type:**_ Specify the type of basis set employed in the calculation.
- **Initial guess**
    - _**Charge:**_ Indicate the total charge of the molecule.
    - _**Multiplicity:**_ Specify the multiplicity of the molecule.
- **DFT options**
    - _**Max SCF iterations:**_ Set the maximum number of SCF (Self-Consistent Field) iterations.
    - _**Use RI:**_ Specify whether the RI (Resolution of Identity) approximation is used.
    - _**Memory for RI:**_ Allocate memory for RI calculations.
    - _**Functional:**_ Specify the DFT functional used.
    - _**Integration grid:**_ Define the integration grid used for the DFT calculations.
    - _**vdw correction:**_ Indicate if van der Waals correction is needed.
    - _**COSMO calculation:**_ Specify if COSMO calculations are needed.
- **Type of calculation**
    - _**Structure optimization:**_ Performing geometry optimization if you select this option. The final structure will be stored in the output directory.
    - _**Excited states calculation:**_ Computing the electronic states of a molecule that are higher in energy than the ground state using the Time-Dependent Density Functional Theory (TD-DFT) method.
    - _**Hyperpolarizability:**_ DFT-Turbomole is able to calculate the first hyperpolarizability for both static and dynamic frequencies. By default, Turbomole calculates the first hyperpolarizability for the second harmonic generation case. However, this WaNo is designed to calculate hyperpolarizability for the Pockels effect as well.
    - _**Frequency calculation:**_ Calculate second derivatives of the energy with respect to nuclear positions. This can be chosen either with the structure optimization parameter or alone.
    - _**Plot HOMO-LUMO orbt:**_  If you need to see the frontier orbitals, selecting this parameter will calculate the related cube files.

# Input
The only needed input file is xyz structure of the molecule.
