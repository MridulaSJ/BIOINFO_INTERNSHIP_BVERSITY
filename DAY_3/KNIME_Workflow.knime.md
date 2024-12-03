# **Day 3: Heatmap Analysis on KNIME**

## <ins>Objective:</ins>

  Use KNIME Analytics Platform to create a heatmap comparing penicillamine with other drug molecules.

## <ins>Process:</ins>

### 1. Introduction to KNIME:

   - Learned about the KNIME interface and how to use its workflow-based approach for data analysis.
   - Imported datasets containing molecular properties of penicillamine and a library of decoppering agents, antioxidants, and antirheumatic drugs.

> Dataset Preparation:

Imported a dataset containing chemical properties of:
     - Penicillamine (the query molecule).
     - Decoppering agents (e.g., trientine).
     - Antioxidants (e.g., vitamin C, flavonoids).
     - Antirheumatic agents (e.g., methotrexate, hydroxychloroquine).

Cleaned the dataset using KNIME nodes, ensuring no missing or redundant entries.

> Feature Selection:

  Selected molecular descriptors, such as molecular weight, polarity, and charge distribution, to quantify similarities.
  Standardized the features to ensure uniform scaling and avoid bias in the analysis.

>Similarity Calculation:

   Used a Tanimoto similarity matrix to calculate structural similarities between penicillamine and other compounds based on their molecular fingerprints.
   This matrix provided a quantitative score (ranging from 0 to 1) to represent the degree of similarity.

### 2. Heatmap Generation:

  - Processed data to calculate molecular similarities between penicillamine and other compounds.
  - Used KNIME nodes to clean the data, calculate similarity coefficients, and visualize the results in a heatmap format.

## <ins>Insights:</ins>

   - Analyzed the heatmap to identify potential drug alternatives for Wilson’s Disease.
   - Found that certain antioxidant compounds showed structural or functional similarities that could make them candidates for further exploration.
