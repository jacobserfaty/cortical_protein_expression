# Cortical Protein Expression Analysis for Ttrisomic Mice
This repository contains code and data for the analysis of protein expression levels in a study investigating Down syndrome. The dataset consists of the expression levels of 77 proteins/protein modifications in the nuclear fraction of cortex samples from mice, with 38 control mice and 34 trisomic mice (Down syndrome), totaling 72 mice. Each protein was measured 15 times per sample/mouse, resulting in a total of 1080 measurements per protein.

### Dataset Description
Purpose: The purpose of this project is to identify subsets of proteins that are discriminant for different classes of mice based on genotype, behavior, and treatment conditions.

Classes of Mice:
- Genotype: Control (c) vs. Trisomic (t)
- Treatment Type: Memantine (m) vs. Saline (s)
- Behavior: Context-shock (CS) vs. Shock-context (SC)
- Experimental Conditions: There are eight classes of mice based on different combinations of genotype, behavior, and treatment conditions.

### Data Description
- Mouse ID: Identifier for each mouse.
- Protein Expression Levels: Values of expression levels of 77 proteins measured in the nuclear fraction. Protein names are followed by "N" indicating measurement in the nuclear fraction, for example, DYRK1A_n.
- Genotype: Control (c) or Trisomy (t).
- Treatment Type: Memantine (m) or Saline (s).
- Behavior: Context-shock (CS) or Shock-context (SC).
- Class: Combination of genotype, behavior, and treatment type. Examples: c-CS-s, c-CS-m, c-SC-s, c-SC-m, t-CS-s, t-CS-m, t-SC-s, t-SC-m.

### Project Objectives
Data Preprocessing:
- Handle missing values.
- Encode categorical variables.

Data Exploration and Visualization:
- Explore protein expression distributions.
- Visualize relationships between protein expression and other variables.

Feature Selection/Dimensionality Reduction:
- Use techniques like t-SNE or feature selection methods to reduce dimensionality.

Statistical Analysis:
- Identify proteins with significant expression differences between classes using statistical tests.

Machine Learning Modeling:
- Train models to classify mice into different classes based on protein expression.

Interpretation:
- Interpret results and discuss biological relevance.

Visualization:
- Create visualizations (e.g., heatmaps, dendrograms) to illustrate relationships between proteins and classes.
