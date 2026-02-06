Empowering Rare Disease Biomedical Repositories via Semantic Knowledge Graph-based Structures
This repository contains the full implementation of a semantic knowledge graph framework for rare disease biomedical data. It includes  Jupyter notebooks, and example queries to construct, populate, and explore a knowledge graph integrating literature-mined and ontology-enriched biomedical entities.

Repository Contents: 
- notebooks/: Jupyter notebooks for each step of the framework 
- Knowledge_Graph_Queries.docx: Example queries and screenshots of subgraphs
- README.md: This file

Proposed Framework Steps:
1. Rare Disease Literature Retrieval: Uses BioEntrez to query PubMed for rare disease literature, filtered for Homo sapiens.
2. Named Entity Recognition using Pubtator3: Uses PubTator3 to extract diseases, genes, variants, chemicals, and chromosomes.
3. Entity Matching and Normalization: Cross-checks entities against curated rare disease databases: NORD, Orphanet, ORDO, eRAM.
4. Relation Extraction: Uses BioBERT for extracting relationships between entities.
5. Knowledge Graph Construction: Converts relationships into triples and imports into Neo4j.
6. Ontology Integration: Enriches the knowledge graph with GO, HPO, MONDO.

Installation & Requirements:
- Clone the repo
- Create a virtual environment
- Install dependencies
- Ensure Neo4j is installed

Usage:
- Run scripts in order
- Explore queries in Neo4j using Knowledge_Graph_Queries.docx



