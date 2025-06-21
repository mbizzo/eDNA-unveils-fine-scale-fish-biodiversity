#### `2_Environmental_Data/`

Contains environmental variables used in biodiversity modeling and machine learning predictions.

##### Contents:

- **`GEE_SeagrassExtent2021.js`**  
  JavaScript script for classifying seagrass extent from 2021 Sentinel-2 imagery using Google Earth Engine (GEE).

- **`Environmental_Layers/`**  
  Folder containing all environmental raster layers (.tif format) projected to a common 500 m grid (UTM Zone 49S, ellps: GRS80).

##### Summary of Environmental Variables:

| Variable                | Source                                                       | Resolution | Time Frame       | Derived Values (500 m grid)                       |
|------------------------|--------------------------------------------------------------|------------|------------------|--------------------------------------------------|
| Marine Habitat Types    | Strydom et al. (2020)                                        | 10 m       | 2021             | % cover of each habitat type                     |
| Bathymetry (Depth)      | Geoscience Australia (Beaman, 2023)                          | 250 m      | 2023             | Depth [m], slope [°]                             |
| Structural Complexity   | Lebrec et al. (2021)                                         | 10 m       | 2017–2020        | SD of depth within 500 m                         |
| Sea Surface Temperature | ESA Sentinel-3A SLSTR                                        | 1000 m     | Aug–Sep 2021     | Median SST [°C], daily variation                 |
| Chlorophyll-a           | ESA Sentinel-3A OLCI                                         | 300 m      | Aug–Sep 2021     | Median and SD Chlo-a [mg/m³] (log10 scaled)      |
| Suspended Matter (TSM)  | ESA Sentinel-3A OLCI                                         | 300 m      | Aug–Sep 2021     | Median and SD TSM [g/m³] (log10 scaled)          |
| Salinity                | Copernicus Global Ocean Physics (L4)                         | ~9 km      | Sep 2021         | Monthly mean salinity (practical salinity units) |
| Distance to Shore       | Calculated using R `geosphere::dist2Line` + coastline shapefile | 500 m      | NA               | Distance to shoreline [m]                        |

All layers were harmonised to the study grid (500 m resolution, UTM Zone 49S) prior to modeling.
