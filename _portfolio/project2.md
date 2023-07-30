---

title: "Simulation of Gene Expression Tables and Probabilities Analysis"
layout: single
---


The primary goal of this project is to develop a versatile script capable of simulating gene expression tables from various types of CSV files and performing probabilistic analyses to assess the significance of observed gene counts. The script generates three crucial outputs: the simulation table, higher probabilities table, and lower probabilities table.


![APP UI Image](images/p2.png)


The above is the figure of the app UI. 

**Step 1: Simulation for Gene Expression Table** The initial step involves simulating the gene expression table to determine if the observed gene counts are statistically significant or simply due to chance. The key challenge is ensuring that the sum of genes in the simulated table matches the sum of genes in the input table. To tackle this, the script employs a custom randomization method using R's powerful `sample` function. This approach guarantees that each gene has an equal probability of being assigned to any cell position.

**Shiny App for User-Friendly Interaction** To democratize this research and make it accessible to all, we have developed a user-friendly Shiny app in R Studio. Users can effortlessly upload their CSV files by clicking the "Browse" button. Once the file is uploaded, the gene expression table will be displayed in the right panel labeled "Table."

**Customizable Simulation Times** Flexibility is paramount in this research, and as such, users can choose the number of simulation iterations they desire. The default number of simulations is set to 10,000, but users can modify this according to their requirements.

**Simulation and Probabilistic Analysis** Upon selecting the desired simulation times, users can initiate the simulation process by clicking the "Simulate" button. The script then runs the simulations and analyzes the results to identify higher and lower probabilities for each gene.

**Downloadable Output Tables** Upon completion of the simulation and analysis, the app displays the higher values and lower values. Users can then download the three essential output tables:

1. Simulation Table
2. Higher Probabilities Table
3. Lower Probabilities Table

**Unbiased Adaptability for All Data** The script has been meticulously designed to handle diverse types of gene expression data without any biases. It ensures that the simulation process remains robust and accurate across all datasets.

This research project provides a powerful and adaptable tool for researchers and biologists, enabling them to validate observed gene counts and assess the statistical significance of their findings. The Shiny app's user-friendly interface simplifies the simulation process, making it accessible to researchers with varying degrees of expertise. By offering customizable options and unbiased adaptability, this script ensures its applicability to a wide range of gene expression datasets.
