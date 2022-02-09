{{site.description}}


# Table of Contents
1. [Introduction](#introduction)
2. [Background](#background)
3. [Methods](#methods)
4. [Results](#results)
5. [Discussion](#discussion)


## 1 Introduction
In recent years, wildfires have been growing into a much larger environmental and public safety threat. Fire seasons are larger, more destructive, and burning longer than ever before such that the US Forest Service has coined the term “fire year”. The exact causes for this behavior are not known, but scientists point to climate change, increased human activity from expansion into rural areas, and over-zealous fire prevention policies that have created environments ripe for wildfires with large buildups of combustible fire fuels. [1] This phenomenon is happening across the world, but is especially apparent in Northern California, which has historically been a global hotspot for wildfires. For example the 2018 fire season, the worst in California’s history, caused over $140 billion in damages and killed over 100 people. Our preliminary analysis also confirms that wildfires are more frequent and destructive. From 1990-2020 there has been a 267% increase in the number of fires annually and in the past 20 years there has been a 520% increase in the number of fire seasons that exceed 500,000 burned acres relative to the 50 years prior.

## What is Burn Severity?

To clarify the confusion on the meaning and usage of wildfire jargon, fire intensity is strictly used to describe the total amount of energy released by a fire and not the effect on the ecosystem and fire or burn severity describe the effect of fire on aboveground and belowground biomass. This includes measures like canopy cover, crown volume, surface litter, and soil hydrophobicity. These terms are often used interchangeably, but a minor distinction is that in certain applications burn severity can specifically refer to fire effects on soil. [2]
Our analysis uses remote sensing data to specifically focus on the effect of wildfire on above and belowground biomass, which we refer to interchangeably as fire or burn severity. This definition is widely used by federal fire mapping groups and past research on wildfires.

Burn severity maps are widely used by federal agencies and forest managers to map fire damage and extent and help manage forest recovery efforts, update vegetation and land cover maps, and monitor ecosystem health. Traditional methods of producing these maps are expensive and time-consuming since they require teams of surveyors and ecologists to gather in-situ data. For many fires, this is infeasible due to harsh weather and inaccessible terrain. These methods are still used for certain fires, but have been largely phased out with the introduction of Earth observing satellites that provide remotely sensed data. Fires can be mapped at a much faster and larger scale at a fraction of the cost relative to field surveys, while still maintaining high accuracy. Remote sensing data is widely used in many other applications, such as agriculture, climate change, and natural disasters, since they cover long time spans and are continuously updated with high resolution, multi-spectral data

[Burn Severity Details](./burnSeverity.md)



Fire mapping responsibilities are shared by several federal interagency groups, mainly Monitoring Trends in Burn Severity (MTBS), Rapid Assessment of Vegetation Condition after Wildfire (RAVG), and Burned Area Emergency Response (BAER).
Federal fire-mapping groups mainly use this image differencing method with dNBR, but with slight differences based on their organizational needs.


## 2 Data
Google Earth Engine (GEE) is a cloud-based distributed computing environment that greatly reduces the technical barriers to entry for large scale geospatial analysis and hosts a large catalog of data including satellite imagery, climate forecasts, and geophysical data.[6] We used the GEE platform to access and run computations on remote sensing data from Landsat 8, NASA SRTM, NLCD 2016, and GRIDMET.

Data on California wildfire seasons from 1950-2020 is provided by CALFIRE and includes information on a fire’s location, geometry, size, and duration.

## 2.1 Fire and Image Selection
In total, 17 fires were selected from a candidate set of 79 fires. The fires occurred across Northern California between 2013-2020 because this coincides with the launch of Landsat 8 (February 2013) and the California wildfire dataset doesn’t include any fires past the 2020 fire season. All selected fires are at least 10,000 acres in size because fires of this size are better documented and have more pixels to sample. 
To get optimal pre and post fire images from Landsat 8, we considered all images that occurred 60 days before and after a fire. Images were selected based on the presence of environmental factors that reduce image quality, including clouds, smoke, and snow,
and their proximity to a fire’s start or end. A majority of pre-fire images are within 14 days of a fire’s ignition, but some post-fire images occur much later due to poor image quality.

[Fire and Image Selection Details](./fireImageDetails.md)

## 2.3 Data Extraction


## Methods


## Results

## Discussion

## References


![ca](images/CA_landCover/ca.png)
![l8](images/gifs/l8.gif)
![landCover](images/gifs/landCover.gif)
![severity](images/gifs/severity.gif)
