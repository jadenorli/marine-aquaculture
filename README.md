Sustainable Growth: Exploring Integrative Multi-Trophic Aquaculture on
the West Coast
================

# Contents

This repository contains an analysis of potential locations within the
Economic Exclusion Zones (EEZ) along the West Coast of the US that are
potentially suitable locations for integrative multi-trophic aquaculture
(IMTA).

# Data

- The first dataset is Sea Surface Temperature (SST) from the [NOAA
  Coral Reef Watch Daily 5km Satellite Sea Surface Temperature (SST)
  (v3.1)](https://coralreefwatch.noaa.gov/product/5km/index_5km_sst.php)
  to characterize the average annual sea surface temperature inside the
  region of interest for the years 2008 to 2012 (NOAA Coral Reef Watch
  (2024)).

- The second dataset is bathymetry data from the [General Bathymetric
  Chart of the Oceans
  (GEBCO)](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area)
  which we used to generate a depth profile for the areas with the
  Economic Exclusion Zones (EEZ) (GEBCO Compilation Group (2024)).

- The third dataset is a shapefile from the [Flanders Marine
  Institute](https://www.marineregions.org/eez.php) that was used to
  define the area of U.S. waters within the EEZ (Flanders Marine
  Institute (VLIZ) (2024)).

- The fourth dataset was created in two steps:

  1.  First, potential finfish species were identified through an
      evaluation of the harvested species managed by the [West Coast
      NOAA Fisheries](https://www.fisheries.noaa.gov/species-directory)
      to compile a list of potentially compatible species (NOAA
      Fisheries: West Coast (2024)).
  2.  Then, life history parameters (thermal range of tolerance and
      vertical distribution) were obtained from
      [FishBase](https://www.fishbase.org.au/v4) (FishBase Consortium
      (2024)).

# Repository Structure

``` bash
      .
      ├── README.md
      ├── bibs
      │   ├── packages.bib
      │   └── references.bib
      ├── code
      │   ├── custom.css
      │   ├── marine_aquaculture.html
      │   └── marine_aquaculture.qmd
      ├── data
      │   ├── average_annual_sst_2008.tif
      │   ├── average_annual_sst_2009.tif
      │   ├── average_annual_sst_2010.tif
      │   ├── average_annual_sst_2011.tif
      │   ├── average_annual_sst_2012.tif
      │   ├── depth.tif
      │   ├── potential_finfish_species.csv
      │   ├── wc_regions_clean.dbf
      │   ├── wc_regions_clean.prj
      │   ├── wc_regions_clean.shp
      │   └── wc_regions_clean.shx
      ├── figures
      │   ├── heatmap
      │   │   └── species_vs_region_heatmap.png
      │   ├── maps
      │   │   ├── NULL_map.png
      │   │   ├── anoplopoma_fimbria_map.html
      │   │   ├── anoplopoma_fimbria_map.png
      │   │   ├── ...
      │   └── tables
      │       ├── potential_species_kable.html
      │       ├── spatial_properties_kable.html
      │       ├── spatial_properties_kable_sst_bath.html
      │       ├── spatial_properties_kable_sst_bath_transform.html
      │       └── top_regions_kable.html
      ├── marine-aquaculture.Rproj
      └── structure.txt
```

# References

<div id="refs" class="references csl-bib-body hanging-indent"
entry-spacing="0">

<div id="ref-fishbase2024" class="csl-entry">

FishBase Consortium. 2024. “FishBase: A Global Information System on
Fishes.” <https://www.fishbase.org.au/v4>.

</div>

<div id="ref-flanders2024" class="csl-entry">

Flanders Marine Institute (VLIZ). 2024. “Maritime Boundaries
Geodatabase: Exclusive Economic Zones (EEZ).” Flanders Marine Institute
(VLIZ); <https://www.marineregions.org/eez.php>.

</div>

<div id="ref-gebco2024" class="csl-entry">

GEBCO Compilation Group. 2024. “General Bathymetric Chart of the Oceans
(GEBCO).” General Bathymetric Chart of the Oceans (GEBCO);
<https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area>.

</div>

<div id="ref-noaa_crw_sst_2024" class="csl-entry">

NOAA Coral Reef Watch. 2024. “Coral Reef Watch Daily 5km Satellite Sea
Surface Temperature (SST) (V3.1).” National Oceanic; Atmospheric
Administration (NOAA);
<https://coralreefwatch.noaa.gov/product/5km/index_5km_sst.php>.

</div>

<div id="ref-noaa_west_coast" class="csl-entry">

NOAA Fisheries: West Coast. 2024. “Sustainable Seafood.”
<https://www.fisheries.noaa.gov/species-directory>.

</div>

</div>
