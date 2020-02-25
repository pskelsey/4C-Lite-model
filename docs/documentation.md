<p align="left">
  <img width="212" height="166"  src="https://github.com/pskelsey/4C/blob/gh-pages/4CLogo.png">
</p>


# DOCUMENTATION

# Table of Contents
* [Background](#background)
  * [Climate data](#climate-data)
  * [Crop data](#crop-data)
* [Basic operation](#basic-operation)
* [Model Tab](#model-tab)
  * [Create your own model](#create-your-own-model)
  * [Fit a model to your own data](#fit-a-model-to-your-own-data)
  * [Plot a model](#plot-a-model)
  * [Final model selection](#final-model-selection)
* [Projections tab](#projections-tab)
  * [Emissions panel](#emissions-panel)
  * [Landscapes panel](#landscapes-panel)
    * [How to incorporate cell areas](#how-to-incorporate-cell-areas)
    * [Select a distribution of locations](#select-a-distribution-of-locations)
    * [Artificial landscape generation](#artificial-landscape-generation)
  * [Dispersal panel](#dispersal-panel)
    * [Choose the type of dispersal](#choose-the-type-of-dispersal)
    * [Create the dispersal function](#create-the-dispersal-function)
  * [Plots panel](#plots-panel)
    * [Making maps](#making-maps)
    * [Plotting projected values](#plotting-projected-values)
    * [Saving results](#saving-results)
  

# Background
The app uses gridded crop distribution and climate change data, and allows you to build a weather-dependent model from your own data that is a function of one- or two-climate variables, and apply it in selected crop grid cells under various climate change scenarios. A unique feature of the app is the ability to define spatial relationships (e.g. risk of pest or pathogen dispersal) among grid cells via various dispersal options. These spatial relationships can be used to modify projected values. 

### Climate data
The app uses raw seasonal 12 km gridded (52 x 39 cells) climate data from the UK Met Office Climate Projections database ([UKCP18](http://ukclimateprojections.metoffice.gov.uk/)) 12-member ensemble of regional projections for RCP8.5. These data provide the best estimates for modelling and summarising the potential effects of future climates on spatial processes in GB as they are fully coherent across different locations, allowing the user to consider climate change at more than one location in a way that captures the relationship between the different locations, and to average projections across user defined land areas. They include both internal modelling variability (using perturbed physics ensembles) and external modelling variability (from the use of different General Circulation Models, or GCMs), as well as information on climate variability. The SCPs provide 11 equally plausible snapshots of climate change; i.e. a range of 11 future values are provided for each climate variable in each grid cell. UKCP09 1961-1991 baseline data are also included for comparison, i.e. for computing a change relative to the current climate.
