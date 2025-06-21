#### `3_Sample_MetaData/`
This folder contains two files summarising the sample metadata used in this paper:

- **`PRJEB84923_Sample_Metadata`** – an overview of all samples and their metadata used in the study:
  
    **Study-specific columns:**
  - `sample_title`: Unique sample ID
  - `Location ID`: Shared ID for samples collected from the same geographic site
  - `collection date`: Date the eDNA sample was collected
  - `geographic location (latitude / longitude)`: GPS coordinates of the sampling site
  - `sampling depth`: Depth of water where the sample was taken (in meters)
  - `sample_type`: Type of sample — `S` (sample), `FNC` (field negative control), `ENC` (extraction negative control), `PC` (positive control), `PCindex` (positive index control)
  - `depth`: Bathymetry at the site (in meters)
  - `Channel_Perc.`: Percentage cover of channel habitat in 500 m grid cell
  - `Complexity`: Seafloor structural complexity (standard deviation of depth)
  - `Distance_to_Shore`: Distance to nearest shoreline (in meters)
  - `Sand_Perc.`: Percentage cover of sand habitat
  - `Sand_Silt_Perc.`: Percentage cover of sand/silt habitat
  - `Seagrass_Perc.`: Percentage cover of seagrass habitat
  - `Slope`: Slope of the seafloor (in degrees)
  - `Salinity`: Practical salinity units (psu)
  - `SST_Daily_Diff`: Median daily sea surface temperature difference (°C)
  - `SST`: Median sea surface temperature (°C)
  - `Turf_Algae_Perc.`: Percentage cover of turf algae
  - `in_rich`: Indicates if the sample was used for richness analysis (`yes` / `no`)
  - `in_comp`: Indicates if the sample was used for composition analysis (`yes` / `no`)

	**ENA-specific columns:**
  - `tax_id`: NCBI taxonomy ID for the sample (e.g., 496924 for fish metagenome)
  - `scientific_name`: Scientific or metagenomic community name (e.g., "fish metagenome")
  - `sample_description`: Short sample description
  - `project name`: ENA project accession (e.g., `PRJEB84923`)
  - `broad-scale environmental context`: General environment category (e.g., "marine")
  - `local environmental context`: More specific description of habitat (e.g., "Shark Bay")
  - `environmental medium`: Medium from which DNA was extracted (e.g., "water")
  - `geographic location (country and/or sea)`: Country or marine region (e.g., "Australia")
  
- **`PRJEB84923_SampleAccessionKey.csv`** – The ENA sample accession key for each sample ID
