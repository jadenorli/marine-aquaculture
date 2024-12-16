Sustainable Growth: Exploring Integrative Multi-Trophic Aquaculture on
the West Coast
================

# Contents

This repository (knitted HTML linked here:
[marine_aquaculture](https://jadenorli.github.io/marine-aquaculture/code/marine_aquaculture.html))
contains an analysis of potential locations within the Economic
Exclusion Zones (EEZ) along the West Coast of the US that are
potentially suitable locations for integrative multi-trophic aquaculture
(IMTA).

# Techniques

This repository highlights a variety of skills and techniques including:

1.  Data Management
    - Wrangling and tidying data using (Wickham et al. 2019), (Müller
      2020), and (Firke 2023)

    - Visualizations with (Wickham 2016) and (Tennekes 2018)

    - Clear documentation and folder structures for reproducibility,
      collaboration, and modularity

    - Integration of conditional statements and custom checks to
      increase reproducibility, error handling, and modularity

    - Development of generalizable functions to allow for
      reproducibility and flexibility in analyses
2.  Geospatial Analysis
    - Handling spatial data with (Hijmans 2024) and (Pebesma 2018)

    - Generating informative interactive maps with (Tennekes 2018)

    - Map algebra with spatial objects within (Hijmans 2024) and
      (Pebesma 2018)
3.  Sustainable Fisheries Science
    - Adapting concepts from (Gentry et al. 2017) and (Troell et
      al. 2010) to analyze potential locations within the West Coast
      EEZs that are suitable for integrative multi-trophic aquaculture
      (IMTA) with oysters and a variety of potential finfish species

    - Integration of flexible species-specific tolerances throughout the
      spatial analyses

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

<div id="ref-janitor" class="csl-entry">

Firke, Sam. 2023. *Janitor: Simple Tools for Examining and Cleaning
Dirty Data*. <https://CRAN.R-project.org/package=janitor>.

</div>

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

<div id="ref-gentry2017" class="csl-entry">

Gentry, Rebecca R., Halley E. Froehlich, Daniel Grimm, Peter Kareiva,
Megan Parke, Michael Rust, Steven D. Gaines, and Benjamin S. Halpern.
2017. “Mapping the Global Potential for Marine Aquaculture.” *Nature
Ecology & Evolution* 1 (9): 1317–24.
<https://doi.org/10.1038/s41559-017-0257-9>.

</div>

<div id="ref-terra" class="csl-entry">

Hijmans, Robert J. 2024. *Terra: Spatial Data Analysis*.
<https://CRAN.R-project.org/package=terra>.

</div>

<div id="ref-here" class="csl-entry">

Müller, Kirill. 2020. *Here: A Simpler Way to Find Your Files*.
<https://CRAN.R-project.org/package=here>.

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

<div id="ref-sf" class="csl-entry">

Pebesma, Edzer. 2018. “<span class="nocase">Simple Features for R:
Standardized Support for Spatial Vector Data</span>.” *The R Journal* 10
(1): 439–46. <https://doi.org/10.32614/RJ-2018-009>.

</div>

<div id="ref-tmap" class="csl-entry">

Tennekes, Martijn. 2018. “<span class="nocase">tmap</span>: Thematic
Maps in R.” *Journal of Statistical Software* 84 (6): 1–39.
<https://doi.org/10.18637/jss.v084.i06>.

</div>

<div id="ref-troell2009" class="csl-entry">

Troell, Max, Andrew Joyce, Thierry Chopin, Amir Neori, Alejandro H.
Buschmann, and Jian-Gang Fang. 2010. “Ecological Engineering in
Aquaculture — Potential for Integrated Multi-Trophic Aquaculture (IMTA)
in Marine Offshore Systems.” *Aquaculture* 297 (1-4): 1–9.
<https://doi.org/10.1016/j.aquaculture.2009.09.010>.

</div>

<div id="ref-ggplot2" class="csl-entry">

Wickham, Hadley. 2016. *Ggplot2: Elegant Graphics for Data Analysis*.
Springer-Verlag New York. <https://ggplot2.tidyverse.org>.

</div>

<div id="ref-tidyverse" class="csl-entry">

Wickham, Hadley, Mara Averick, Jennifer Bryan, Winston Chang, Lucy
D’Agostino McGowan, Romain François, Garrett Grolemund, et al. 2019.
“Welcome to the <span class="nocase">tidyverse</span>.” *Journal of Open
Source Software* 4 (43): 1686. <https://doi.org/10.21105/joss.01686>.

</div>

</div>
