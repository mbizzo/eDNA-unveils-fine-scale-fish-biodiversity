# Integrating Environmental DNA Metabarcoding and Remote Sensing Reveals Known and Novel Fish Diversity Hotspots in a World Heritage Area

**Running Title:** *eDNA unveils fine-scale fish biodiversity*  
**Study Location:** Shark Bay, Western Australia  
**Accession Number:** ENA Project [PRJEB84923](https://www.ebi.ac.uk/ena/browser/view/PRJEB84923)  
**Manuscript Reference:** *DDI-2025-0112*

---

## 📌 Overview

This repository supports the manuscript **"Integrating Environmental DNA Metabarcoding and Remote Sensing Reveals Known and Novel Fish Diversity Hotspots in a World Heritage Area"**. It provides data, scripts, and metadata used to assess fish biodiversity in Shark Bay, a UNESCO World Heritage site, through the integration of eDNA metabarcoding, remote sensing, and machine learning.

---

## 🔬 Study Summary

Shark Bay is highly vulnerable to climate change, yet its fish biodiversity has been poorly documented at fine spatial scales. This study used:

- **eDNA metabarcoding** (16S and 12S rRNA markers) to detect fish species from 270 water samples.
- **Remote sensing** to derive high-resolution environmental variables (e.g., salinity, depth, seagrass cover).
- **Machine learning** to model and extrapolate fish biodiversity patterns across 560 km².

**Key Findings:**

- 1067 fish species detected from 132 genera and 71 families.
- Biodiversity hotspots correspond to salinity gradients, seagrass density, and bathymetry.
- Detection of tropical species suggests climate-driven poleward shifts.
- Five distinct fish communities (A–E) were identified.

This framework offers a scalable, non-invasive approach for biodiversity monitoring in dynamic marine environments.

---

## 📁 Repository Structure

.
├── 1_eDNA_Bioinformatics/
│   └── README.md
├── 2_Environmental_Data/
│   └── README.md
├── 3_Sample_MetaData/
│   └── README.md
└── README.md (this file)


### Folder Details

#### `1_eDNA_Bioinformatics/`
Contains the complete bioinformatics workflow used to process raw sequencing reads into ZOTU (zero-radius OTUs) count tables and assign taxonomic identities.

- Includes filtering steps, and summary statistics, taxonomic assignmnets.
- Two sequencing runs:
  - `p751_run_250522` – MiFish12S metabarcode
  - `p751_run_220617` – Fish16S metabarcode
- Resulting ZOTU count tables including taxonomic assignmnents

#### `2_Environmental_Data/`
Environmental variables used in biodiversity modeling.

- Includes a JavaScript script for seagrass classification from 2021 satellite imagery.
- Environmental layers used in the study

#### `3_Sample_MetaData/`
Compiled sample-level metadata, including:

- Sample information (e.g. collection date)
- Sample locations
- Environmental data per site
- ENA accession keys for raw sequence data

---

## 🧪 Data Availability

- **Raw sequencing data** are deposited under ENA Project: [PRJEB84923](https://www.ebi.ac.uk/ena/browser/view/PRJEB84923)
- Total samples:
  - 273 eDNA samples
  - 17 negative controls
  - 2 positive controls

---

## 📖 Citation


---

## 🔧 Contact

For questions or contributions, please open an issue on this GitHub repository or contact the corresponding author listed in the manuscript.
