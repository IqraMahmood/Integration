# Lung Cell Data Integration
## Predicting Cellular Activity using Deep Learning from Spatial Transcriptomics Data

**Overview**

This project aims to predict cellular activity using deep learning techniques from spatial transcriptomics data. We integrate single-cell RNA-seq data and spatially-resolved transcriptomics data obtained from HUMAN CELL ATLAS and 10x Genomics Visium, respectively. The deep learning model is trained to learn spatial patterns and gene expression relationships, enhancing our understanding of tissue organization and cellular functions.


## Data Sources
### Single-cell RNA-seq:

- Single-cell RNA-seq is downloaded from the Human Cell Atlas, which provides standardized, cell-type-resolved transcriptomic profiles of 62+ million human cells across 18 biological systems.


Download Link:
https://explore.data.humancellatlas.org/projects/b208466a-6fb0-4385-8cfb-8e03ff6b939e/get-curl-command

### Visium Spatial Data:

- Spatial Data is downloded from from 10x Genomics


10x Genomics obtained FFPE Human Lung Cancer tissue blocks from Avaden Biosciences. The tissue was sectioned as described in Visium CytAssist Spatial Gene Expression for FFPE – Tissue Preparation Guide Demonstrated Protocol (CG000518). Tissue sections of 5 µm was placed on a standard glass slide, then H&E-stained following deparaffinization. Sections were coverslipped with 85% glycerol, imaged, decoverslipped, followed by dehydration & decrosslinking Demonstrated Protocol (CG000520). The glass slide with tissue section was processed via Visium CytAssist instrument to transfer analytes to a Visium CytAssist Spatial Gene Expression slide. The probe extension and library construction steps follow the standard Visium for FFPE workflow outside of the instrument.

Link:
 https://www.10xgenomics.com/datasets/human-lung-cancer-ffpe-2-standard 


- Combining Human Cell Atlas single-cell RNA-seq with 10x Visium spatial data
## Workflow

- Files 
1. 01_rename.ipynb - Renaming and organizing single-cell RNA-seq data files and folders for compatibility.

2. 02_preprocess.ipynb - Preprocessing of single-cell and spatial data, including filtering, normalization, and data integration preparation.

3. 03_pca.ipynb - Dimensionality reduction using PCA for easier integration and computational efficiency.

4. 04_integration_using_tangram.ipynb - Integration of single-cell and spatial data using the Tangram tool.

5. 05_deep_learning_model.ipynb - Implementation of the deep learning model to predict cellular activity based on integrated data.
