# Cortical Protein Expression Analysis for Trisomic Mice
This repository contains code and data for the analysis of protein expression levels in a study investigating Down syndrome. The dataset consists of the expression levels of 77 proteins/protein modifications in the nuclear fraction of cortex samples from mice, with 38 control mice and 34 trisomic mice (Down syndrome), totaling 72 mice. Each protein was measured 15 times per sample/mouse, resulting in a total of 1080 measurements per protein.

![mice_spread](https://github.com/jacobserfaty/cortical_protein_expression/blob/main/cortical_plots/mice_spread.png)

### Dataset Description
**Purpose:** The purpose of this project is to identify subsets of proteins that are discriminant for different classes of mice based on genotype, behavior, and treatment conditions.

**Classes of Mice:**
- Genotype: Control (c) vs. Trisomic (t)
- Treatment Type: Memantine (m) vs. Saline (s)
- Behavior: Context-shock (CS) vs. Shock-context (SC)
- Experimental Conditions: There are eight classes of mice based on different combinations of genotype, behavior, and treatment conditions.

### Data Description
- **Mouse ID:** Identifier for each mouse.
- **Protein Expression Levels:** Values of expression levels of 77 proteins measured in the nuclear fraction. Protein names are followed by "N" indicating measurement in the nuclear fraction, for example, DYRK1A_n.
- **Genotype:** Control (c) or Trisomy (t).
- **Treatment Type:** Memantine (m) or Saline (s).
- **Behavior:** Context-shock (CS) or Shock-context (SC).
- **Class:** Combination of genotype, behavior, and treatment type. Examples: c-CS-s, c-CS-m, c-SC-s, c-SC-m, t-CS-s, t-CS-m, t-SC-s, t-SC-m.

### Project Objectives
**Data Preprocessing:**
- Handle missing values.
- Encode categorical variables.

**Data Exploration and Visualization:**
- Explore protein expression distributions.
- Visualize relationships between protein expression and other variables.

**Feature Selection/Dimensionality Reduction:**
- Use techniques like t-SNE or feature selection methods to reduce dimensionality.

![t-SNE c-CS-m](https://github.com/jacobserfaty/cortical_protein_expression/blob/main/cortical_plots/t-SNE_c-CS-m.png)

**Statistical Analysis:**
- Identify proteins with significant expression differences between classes using statistical tests.
- Explore variation in protein expression between treatment groups (e.g., context-shock vs. shock-context, memantine vs. control).

![SOD1_N violin](https://github.com/jacobserfaty/cortical_protein_expression/blob/main/cortical_plots/SOD1_N_violin.png)

![CaNA_N violin](https://github.com/jacobserfaty/cortical_protein_expression/blob/main/cortical_plots/CaNA_N_violin.png)

**Machine Learning Modeling:**
- Train models to classify mice into different classes based on protein expression.

**Interpretation:**
- Interpret results and discuss biological relevance, including behaviorally instigated genetic transcription changes and drug-induced genetic transcription changes.
- Explore relationships between different proteins using agglomerative hierarchical clustering.

**Visualization:**
- Create visualizations (e.g., heatmaps, dendrograms) to illustrate relationships between proteins and classes, and to demonstrate the effectiveness of t-SNE in identifying protein groups and hierarchical clustering in revealing deeper relationships between proteins.

![Heatmap c-SC-m](https://github.com/jacobserfaty/cortical_protein_expression/blob/main/cortical_plots/Heatmap_c-SC-m.png)

![heatmap c-CS-m](https://github.com/jacobserfaty/cortical_protein_expression/blob/main/cortical_plots/heatmap_c-CS-m.png)
