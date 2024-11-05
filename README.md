# Friction-coeffs
This model takes friction coefficient polygons supplied by the user, clips the data to the domain and ensures the data is in the correct projection.

## Description
The CityCAT model can use friction coefficient polygons to set the permeability in specific locations. This model accepts data in .gpkg format, clips the data to the selected area, and ensures all data is in the same projection. If the file sizes are too large, multiple .gpkgs can be added directly, or zipped.

The new friction coefficient is set as "Value" in the gpkg file

## Input Parameters


## Input Files (data slots)
* Boundary
  * Description: A .gpkg of the geographical area of interest. 
  * Location: /data/inputs/boundary
* Parameters
  * Description: location and projection
  * Location: /data/inputs/parameters
* Friction-ceffs
  * Description: A .gpkg with the new friction coeffs set as "Value"
  * Location: /data/inputs/friction_coeffs
 

## Outputs
* The model should output only one file - a .gpkg file of the chosen area containing the friction coeffs of interest with the friction coefficientsset as the "Value"
  * Location: /data/outputs/friction_coeffs
