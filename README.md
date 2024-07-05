# The Global Biodiversity Framework can be leveraged to better manage transboundary watersheds

These script accompany the publication by Kuempel and Suarez-Castro published in PNAS (2024).

# Raw data

The raw data to reproduce these analyses can be downloaded from the following sources and should be placed within corresponding folders into a raw_data folder within the R project before running the scripts.

[GADM36 country boundaries](https://gadm.org/download_country36.html)
[EEZ - Maritime Boundaries v11](https://www.marineregions.org/downloads.php)
[HdyroBasins](https://www.hydrosheds.org/products/hydrobasins)
[Global Sedimentation - Suarez Castro et al. 2021](https://datadryad.org/stash/dataset/doi:10.5061/dryad.g4f4qrfqq)
[RiverAtlas](https://www.hydrosheds.org/hydroatlas)


# Scripts

Run scripts in sequential order as follows:

1. 1_Basin_country_overlap.Rmd - This script intersects level 8 watersheds from the HydroBASINS dataset with country boundaries to determine transboundary watersheds
2. 2_Sediment_export_basin_iso3.Rmd - This script calculates the sediment export from transboundary watersheds based on data from Suarez-Castro et al. 2021
3. 3_Identify_pourpoints.Rmd - This script identifies the endpoints (pourpoints) of rivers draining into the ocean globally from the RiverATLAS v10 data.
4. 4_Trans_land_sediments.Rmd - This script identifies mismatches in location between countries that export the most sediment in a basin and the country where the pourpoints are located
5. 5_Sediment_at_pourpoints.Rmd - This script distributes sediment among pourpoints to use in sediment ocean transport model
6. 6_Terrestrial_trans_mismatch.Rmd - This script identifies mismatches in where sediment comes from and where it is released at pourpoints
7. 7_Results.Rmd 
8. 8_Figure1.Rmd
