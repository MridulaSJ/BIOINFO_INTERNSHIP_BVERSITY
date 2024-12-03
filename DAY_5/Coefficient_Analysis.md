# **Day 5: Coefficient Analysis and GitHub Setup**
## <ins>Objective:</ins>
  - Perform coefficient analysis to evaluate 2D and 3D conformers quantitatively.
  - Learn GitHub for managing and sharing the bioinformatics project.
## <ins>Process:</ins>
1. Coefficient Analysis in KNIME
- Understanding Coefficients:

Coefficients provide numerical metrics to evaluate structural properties and relationships between molecules.

Calculated for both 2D and 3D conformers to capture structural and spatial attributes.

- 2D Coefficients:

Derived from 2D descriptors such as molecular fingerprints, Tanimoto similarity, and other chemical properties.

Identified relationships between penicillamine and related compounds based on structural similarity.

- 3D Coefficients:

Calculated using RMSD values between conformers.

Analyzed spatial differences to determine which conformers are most likely to bind copper effectively.

## 1. Workflow 1: Tanimoto Coefficient Calculation
### Description
This workflow computes the **Tanimoto coefficient** for comparing 2D molecular fingerprints.

### Steps
1. **Input Files**:
   - SDF files containing molecular structures were imported using the `SDF Reader` node.
2. **Fingerprint Generation**:
   - Molecular fingerprints were generated using the `RDKit Fingerprint` node.
   - The fingerprint type was set to **Morgan** with radius 2.
3. **Similarity Calculation**:
   - The finferprint similarity node calculated the Tanimoto coefficient between pairs of molecules.
4. **Output**:
   - The coefficient values were obtained.

### Result
- **Tanimoto Coefficient**: 0.344 (Low similarity between the two 2D conformers).

## 2. Workflow 2: 3D Conformer Analysis
### Description
This workflow analyzes 3D conformers by calculating **RMSD**, scoring, and generating heatmaps.

### Steps
1. **Input Files**:
   - Molecule and reference structures were imported using the `SDF Reader` node.
2. **Conformer Generation**:
   - The `RDKit` node was used to generate multiple 3D conformers for each molecule.
3. **RMSD Calculation**:
   - The `RDKit` node compared each generated conformer against the reference structure.
   - The maximum RMSD value of 0.723 was noted.
4. **Scoring**:
   - The stability score was calculated, yielding a highest score of **71.777**.
5. **Heatmap Generation**:
   - A distance or interaction matrix was created using the `Jfreechart` node.
   - The matrix was visualized using the `Heatmap` node and exported as `heatmap.png`.
### Results
- **RMSD**: 0.723 (Maximum value).
- **Score**: 71.777 (Stability score).
- Heatmap visualized molecular interactions.

## Introduction to GitHub

Creating a Repository:
       
   Learned to set up a GitHub repository for the project, with a structured file hierarchy.
