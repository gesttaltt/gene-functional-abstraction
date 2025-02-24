# Gene Functional Abstraction (v0.1.0 branch)

![image](https://github.com/user-attachments/assets/2f6c3913-c166-4e67-8257-49bfd5a73f64)

Early-phase project exploring gene ontology data biases. The v0.1.0 branch establishes a foundation for a classification model to address gene ontology issues. Not production-ready— this is a proposal.

This project ingests Gene Ontology data (downloading `go-basic.json` if not present), processes it to extract key gene features (pathways, interactions, and a computed impact index), and visualizes the results through an interactive Dash dashboard with multiple tabs for bar charts, histograms, scatter plots, filtering, and summary statistics.

## References and Important Citations

Gene ontology data from the 2025-02-06 release (DOI:10.5281/zenodo.14861039) is made available under the terms of the CC BY 4.0 license.
Creative Commons 4.0 License legal code: https://creativecommons.org/licenses/by/4.0/legalcode

Gene Ontology Website: https://geneontology.org/
Papers:

    Ashburner et al. Gene ontology: tool for the unification of biology. Nat Genet. 2000 May;25(1):25-9. DOI: 10.1038/75556 [full text: https://pmc.ncbi.nlm.nih.gov/articles/PMC3037419/]
    The Gene Ontology Consortium. The Gene Ontology knowledgebase in 2023. Genetics. 2023 May 4;224(1):iyad031. DOI: 10.1093/genetics/iyad031 [full text: https://pmc.ncbi.nlm.nih.gov/articles/PMC10158837/pdf/iyad031.pdf]

"The database used in the v0.1.0 (go-basic.json) of this project is the DOI:10.5281/zenodo.14861039"

According to the terms of GO’s CC BY 4.0 license, those using our data publicly or redistributing it must provide:

    “identification of the creator(s) of the Licensed Material and any others designated to receive attribution, in any reasonable manner requested by the Licensor (including by pseudonym if designated);”
    “a copyright notice;”
    “a notice that refers to this Public License;”
    “a notice that refers to the disclaimer of warranties;”
    “a URI or hyperlink to the Licensed Material to the extent reasonably practicable;”

## How to Use

1. **Activate your virtual environment** (e.g., using `python -m venv venv` and activating it).
2. **Run the workflow** by executing:
   ```bash
   python src/main.py

Enhancing Genetic Analysis Through Functional Abstraction
-----------------------------------------------------------

Overview:
This project focuses on advancing genetic analysis by targeting "functionality"—
differentiating genes based on "levels of abstraction." It computes an adjustable
functional impact index for each gene and organizes them into a database that
reflects their participation in pathways and interactions. This approach distinguishes
high-level integrators from specialized, function-specific genes, offering a collaborative,
open-source tool for exploring complex genetic interactions.

Currently, the program primarily focuses on the genomics layer by leveraging gene ontology data. It visualizes and classifies genes based on their involvement in biological pathways and interactions—essentially providing insights into gene functionality and regulatory networks. In a multi-omics context, this represents the genomic aspect, with potential future integration of transcriptomic, proteomic, or metabolomic data to offer a more comprehensive systems biology view.

Project Stages:
---------------
Stage 1: Gene Classification & Data Integration
    - Compute the functional impact index for each gene.
    - Integrate additional annotation datasets.
    - Group genes by their abstraction degree (high vs. low).

Stage 2: Analysis & Visualization
    - Develop interactive dashboards and network graphs.
    - Enable users to explore gene interactions and filter data.
    - Provide insights into functional connectivity.

Stage 3: Validation, Community Collaboration & Expansion
    - Validate the model using experimental data and literature.
    - Engage the community for feedback and contributions.
    - Expand the tool’s capabilities for broader systems biology applications.

Glossary & Conventions:
-----------------------
Abstraction Definitions:
    - Genetic Functionality:
      The ability of genes to influence one another, facilitating expression,
      transcriptome formation, and other biological "layers."
    - Functional Impact:
      A measure of the "relevance" of a gene or group of genes based on specific parameters.
    - Layers:
      Structural blocks that compose the genome, representing groups of functionality.
    - Degrees:
      Indices that quantify the level of functional impact of genes.
    - Levels:
      Complexity indicators corresponding to the biological homeostatic functions
      of high-degree genes.

Statistical Indexes:

    - Qualitative Index:
      Derived by defining the desired quality and measuring the functional impact
      of genes using parameters such as connectivity, patterning, and hidden distributions.
      
    - Quantitative Index:
      Measures the intensity of qualitative indexes in different contexts, such as
      structural organization and interaction paradigms.

Note:
-----
This project and its accompanying glossary are works in progress. They provide an initial
structure for continued development and community collaboration.
