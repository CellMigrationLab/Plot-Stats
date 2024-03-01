# Plot_and_Stats
Jupiter notebooks created to help us plot and analyse our datasets


## Plot and Stats for Tidy Format

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CellMigrationLab/Plot_and_Stats/blob/main/Notebooks/Plot_and_Stats_for_Tidy_Format.ipynb)


This Jupyter Notebook is crafted for the purpose of analyzing datasets maintained in a [tidy format](https://thenode.biologists.com/converting-excellent-spreadsheets-tidy-data/education/). It integrates a comprehensive set of functionalities for in-depth data examination, statistical evaluation, and dataset balancing, enhancing both the analysis and interpretability of your data.

### **Key Features**

- **Boxplots with Labels**: Creates detailed boxplots that visually differentiate each data point and clearly label repeats, facilitating an immediate understanding of the data distributions.

- **Cohen's d Calculation**: Enables the computation of Cohen's d value, offering a quantitative measure of the effect size between groups and highlighting the significance of observed differences.

- **Randomization Test Based on Cohen's d**: Implements a non-parametric randomization test using Cohen's d, suitable for datasets that may not meet the strict assumptions required for traditional parametric tests. More info on randomization [tests here](https://thenode.biologists.com/user-friendly-p-values/research/).

- **Statistical Summaries Export**: Automatically generates and exports comprehensive statistical summaries, providing a snapshot of crucial metrics throughout the dataset.

- **Dataset Balance Check**: Examines the dataset for balance across various conditions and repeats, ensuring that each group is equally represented in subsequent analyses.

- **Dataset Resampling**: Facilitates the adjustment of the dataset to a balanced condition through downsampling, making comparisons across groups fairer and more meaningful.

- **Analysis of Resampled Dataset**: Offers tools to further analyze the balanced dataset, with plots and statistical tests designed to uncover robust insights from the equitably represented data.

This notebook acts as a powerful tool for researchers and data analysts, streamlining the workflow from data ingestion to comprehensive analysis, thus enabling a deeper and more accurate exploration of datasets.

