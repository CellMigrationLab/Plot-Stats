# Plot&Stats
Jupiter notebooks created to help us plot and analyse our datasets

## Quick Start

Access the notebooks directly in Google Colab for an easy-to-use environment:

- **Plot&Stats - Wide to Tidy Format**: Transform wide-format data into tidy format for analysis.
  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot%26Stats%20-%20wide%20to%20tidy.ipynb)
  
- **Plot&Stats - BoxPlots**: Enhanced data visualization, quantifies effect size, adapts to non-standard distributions, streamlines analysis, ensures equitable group representation, achieves dataset balance for fairer comparisons, and delivers in-depth insights from balanced data.
  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot&Stats_BoxPlots.ipynb)

- **Plot&Stats - dimensionality reduction**: Notebook for generating PCA, UMAP or t-SNE dimensional reduction of multidimensional datasets.
    
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot%26Stats-%20dimensionality%20reduction.ipynb)

## About the Notebooks


### Plot and Stats - wide to tidy 
This notebook is designed to transform wide-format data into a tidy format for further analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot%26Stats%20-%20wide%20to%20tidy.ipynb)


Wide and tidy formats represent two principal ways of structuring tabular data:

- **Wide Format**:
  - Each row represents a subject or item.
  - Observations spread across multiple columns.
  - Suitable for data entry or presentation.
  - Example with biological repeats:
    ```
    | Subject | Cond1_Repeat1 | Cond1_Repeat2 | Cond2_Repeat1 | Cond2_Repeat2 |
    |---------|---------------|---------------|---------------|---------------|
    | 1       | ValueA        | ValueB        | ValueC        | ValueD        |
    ```

- **Tidy Format**:
  - Each column is a variable, each row an observation.
  - Suited for statistical analysis and plotting.
  - Each row represents a unique combination of variables.
  - Example with biological repeats:
    ```
    | Subject | Condition | Repeat | Value  |
    |---------|-----------|--------|--------|
    | 1       | Cond1     | 1      | ValueA |
    | 1       | Cond1     | 2      | ValueB |
    | 1       | Cond2     | 1      | ValueC |
    | 1       | Cond2     | 2      | ValueD |
    ```

Wide format is more readable for direct comparisons across a subject's measurements, while tidy format is optimized for analysis, making data transformations, summarizations, and visualizations more straightforward.

### Plot&Stats - BoxPlots

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot&Stats_BoxPlots.ipynb)


This Jupyter Notebook is crafted for the purpose of analyzing datasets maintained in a [tidy format](https://thenode.biologists.com/converting-excellent-spreadsheets-tidy-data/education/). It integrates a comprehensive set of functionalities for in-depth data examination, statistical evaluation, and dataset balancing, enhancing both the analysis and interpretability of your data.

#### **Key Features**

- **Boxplots with Labels**: Creates detailed boxplots that visually differentiate each data point and clearly label repeats, facilitating an immediate understanding of the data distributions.

- **Cohen's d Calculation**: Enables the computation of Cohen's d value, offering a quantitative measure of the effect size between groups and highlighting the significance of observed differences.

- **Randomization Test Based on Cohen's d**: Implements a non-parametric randomization test using Cohen's d, suitable for datasets that may not meet the strict assumptions required for traditional parametric tests. More info on randomization [tests here](https://thenode.biologists.com/user-friendly-p-values/research/).

- **Statistical Summaries Export**: Automatically generates and exports comprehensive statistical summaries, providing a snapshot of crucial metrics throughout the dataset.

- **Dataset Balance Check**: Examines the dataset for balance across various conditions and repeats, ensuring that each group is equally represented in subsequent analyses.

- **Dataset Resampling**: Facilitates the adjustment of the dataset to a balanced condition through downsampling, making comparisons across groups fairer and more meaningful.

- **Analysis of Resampled Dataset**: Offers tools to further analyze the balanced dataset, with plots and statistical tests designed to uncover robust insights from the equitably represented data.

This notebook acts as a powerful tool for researchers and data analysts, streamlining the workflow from data ingestion to comprehensive analysis, thus enabling a deeper and more accurate exploration of datasets.

### Plot&Stats - dimensionality reduction

#### **Key Features**

 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot%26Stats-%20dimensionality%20reduction.ipynb)

- **PCA Analysis & Plots**: Generates PCA plots that visually represent the data's variance along principal components, along with the PCA loadings to identify contributing features.
- **UMAP or t-SNE  Visualization**: Utilizes UMAP or t-SNE for dimensionality reduction to project high-dimensional data into a lower-dimensional space, enhancing cluster identification.
- **HDBSCAN Clustering**: Applies the HDBSCAN algorithm to identify naturally occurring clusters in the data without specifying the number of clusters a priori.
- **Fingerprinting Plots**: Creates fingerprinting plots that detail the distribution of the identified clusters accross the conditions.
- **Boxplots of Clusters**: Generates boxplots for each identified cluster to compare distributions across different conditions.


