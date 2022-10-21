# BDB_Magnoliopsida

In this repository you will find data related to the annotation of a Chromosome fragment, belonging to Kingdom: plantae, Division: Magnoliophyta, Class: Magnoliopsida.

With these files, the process of integration of information in a single database is carried out. Python tools are used for this purpose, with the objective of reading each file and adding new features. In the case of transposable elements, the initial and final position was identified and the sequence of the repetitive element was extracted from the chromosome (ptg000002l_format.json). In the case of genes, the file obtained for protein annotation was used as a basis and the reference identifier obtained in the BLAST file and a column with the gene sequence were added to it (genes_format.json).

With these databases, queries were performed, importing them into MongoDB.

Finally, we were able to expand the information of the predicted genes using the command: esearch. This accesses the NCBI page and extracts more information about the location and function of the identified protein (genes_format_genbank.json).
