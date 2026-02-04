# CandyMap: Dimensionality Reduction of Candy Popularity

This project explores hidden relationships between candies using dimensionality reduction techniques on the FiveThirtyEight candy dataset.  
We reduce high-dimensional candy features (ingredients, sugar %, price %, etc.) into 2D spaces using **PCA**, **t-SNE**, and **UMAP** to visualize how candies group by similarity and how **winpercent** (popularity) distributes across these maps.

## Goals
- Identify hidden patterns among candies based on their attributes
- Compare the structures revealed by PCA vs t-SNE vs UMAP
- Analyze how candy popularity (winpercent) relates to positions in reduced spaces

## Methods
- Data preprocessing: feature selection + standardization (StandardScaler)
- Dimensionality reduction:
  - **PCA** (linear, variance-based)
  - **t-SNE** (nonlinear, local neighborhood preservation)
  - **UMAP** (nonlinear, local + global structure)
- Popularity analysis: correlation between winpercent and distance in 2D embeddings (notably strong in UMAP)
