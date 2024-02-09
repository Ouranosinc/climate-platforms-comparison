# climate-platforms-comparison
This repo stores the code for the paper "Canadian Climate Data Portals: A Comparative Analysis from a User Perspective".

## Instructions

 In order to run the code, you will need:
 1. To create an environnment based on the environnment.yml file.
 2. To create the xscen catalog `pcat_espo` with data from PC (ESPO-G6-R2). 
    - The daily timeseries can be found [here](https://pavics.ouranos.ca/twitcher/ows/proxy/thredds/catalog/datasets/simulations/bias_adjusted/cmip6/ouranos/ESPO-G/ESPO-G6-R2v1.0.0/catalog.html)
    - The indicators can be found [here](https://pavics.ouranos.ca/twitcher/ows/proxy/thredds/catalog/birdhouse/ouranos/portraits-clim-2.0/catalog.html)
    - The code to create that data, to compute the indicators and create the catalog can be found [here](https://github.com/Ouranosinc/ESPO-G).
 3. To download the data from CDCA. The catalog is created in the notebook `prepare_data.ipynb`.
    - The daily timeseries can be found [here](https://pavics.ouranos.ca/twitcher/ows/proxy/thredds/catalog/datasets/simulations/bias_adjusted/cmip6/pcic/CanDCS-U6/catalog.html)
    - The indicators data can be found [here](https://pavics.ouranos.ca/twitcher/ows/proxy/thredds/catalog/datasets/simulations/bias_adjusted/cmip6/climatedata_ca/ensemble_statistics/catalog.html)
 4. Put your own path in `paths_example.yml` and rename it `paths_pc.yml`.
 5. Prepare the data with the notebook `prepare_data.ipynb`.
 6. Calculate the missing indicators (not already calculated in their own platform/ another project) with the notebook `missing_indicators.ipynb` and `missing_ind.yml`.
 7. Compute the analysis for section Comparison of Core Climate Variables over Canada with the notebook `basic_variables.ipynb`.
 8. Compute the analysis for section Case Studies with the notebook `case_studies.ipynb`.


