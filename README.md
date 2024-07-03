# The Global Biodiversity Framework can be leveraged to better manage transboundary watersheds

These script accompany the publication by Kuempel and Suarez-Castro published in PNAS (2024).


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
