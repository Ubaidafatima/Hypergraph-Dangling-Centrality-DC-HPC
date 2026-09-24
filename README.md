# Hypergraph Dangling Centrality and DC-HPC

Reproducibility package for the manuscript:

**Dangling Centrality in Hypergraphs: Structural Vulnerability and Centrality-Guided Overlapping Community Discovery**

**Author:** Ubaida Fatima  
**Affiliation:** Department of Mathematics, NED University of Engineering and Technology, Karachi, Pakistan

## Contents

The `code/` directory contains six Google Colab/Jupyter notebooks:

1. `01_Illustrative_8_Node_Hypergraph_Centrality.ipynb`  
   Manual/validated 8-node, 5-hyperedge example. Computes hyperdegree, closeness,
   betweenness, eigenvector centrality, Hypergraph Dangling Centrality (HDC), and timings.

2. `02_Enron_Hypergraph_Centrality.ipynb`  
   Loads and validates the Enron higher-order e-mail dataset, constructs the static
   hypergraph representation, computes centrality measures, and generates analysis outputs.

3. `03_NDC_Hypergraph_Centrality_and_Communities.ipynb`  
   Computes NDC-classes centralities, exact HDC, hyperedge-percolation communities,
   sensitivity analyses, memberships, and descriptive associations.

4. `04_Walmart_Hypergraph_Scalable_Centrality.ipynb`  
   Scalable Walmart Trips analysis. Computes full-data sparse measures and exact
   betweenness/HDC on the reproducible 250-product structural core used in the manuscript.

5. `05_Enron_Community_Analysis_and_Visuals.ipynb`  
   Hyperedge-percolation community analysis, centrality-related outputs, and figures for Enron.

6. `06_Walmart_Community_Analysis_and_Visuals.ipynb`  
   Hyperedge-percolation community analysis, centrality-related outputs, and figures for Walmart.

## Data sources

The original real-world datasets are not redistributed in this archive. Download them
from the Cornell Higher-Order Network Dataset Repository and upload them to the
corresponding Colab notebook when prompted:

- Enron e-mail: https://www.cs.cornell.edu/~arb/data/email-Enron/
- NDC-classes: https://www.cs.cornell.edu/~arb/data/NDC-classes/
- Walmart Trips: https://www.cs.cornell.edu/~arb/data/walmart-trips/

The manuscript cites the appropriate original dataset references.

## Running the notebooks

The notebooks are designed for Google Colab. Upload a notebook to Colab, choose
**Runtime -> Run all**, and provide the requested raw dataset archive when prompted.

Common Python dependencies used across the notebooks include NumPy, pandas,
SciPy, NetworkX, Matplotlib, and, where required, HyperNetX.

## Reproducibility notes

- Unreachable hypergraph distances are represented as infinity, with reciprocal
  contribution equal to zero.
- The Walmart exact HDC analysis uses a reproducible 250-vertex structural core because
  exact repeated node-isolation shortest-path computation is expensive at full scale.
- Hyperedge-percolation calculations are performed on the original hypergraph structure.
  Pairwise/co-membership projections are used only where a notebook explicitly states
  that they are needed for a centrality calculation or visualization.
- Randomized procedures use fixed seeds where specified in the notebooks.

## Suggested Zenodo record type

Software

## Suggested version

v1.0.0
