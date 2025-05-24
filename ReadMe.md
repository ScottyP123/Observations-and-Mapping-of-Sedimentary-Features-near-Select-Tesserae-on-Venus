# ReadMe for Scott Petersen's Undergraduate Senior Thesis
## TITLE: Observations and Mapping of Sedimentary Features near Select Tesserae on Venus
## AUTHORS: Petersen, S. K. (1) and Carter, L. M. (2)
## (1): Undergraduate, department of Planetary Sciences, University of Arizona
## (2): Professor, Lunar and Planetary Laboratory, University of Arizona
<br>

## Contact: Scott Petersen at scott.karl.petersen@gmail.com
<br>

### Introduction
The work contained in this data repository was done for Scott Petersen's undergraduate senior thesis for his major in Planetary Geoscience, with honors at the University of Arizona. Scott's thesis advisor was Prof. Lynn Carter. Over the course of one and a half years, we mapped and classified several types of sedimentary features in the vicinity of tesserae on Venus to better constrain tessera terrain's role in Venus's sedimentary cycle. We also created an adaptation of an algorithm to automatically map dune crestlines.

### Basic File Structure
<pre>.
├── README.md
├── LICENSE.txt
├── SemiAutomatedCrestlineMapping.ipynb
├── SedimentaryFeatureMap
│    ├── Dark_LowEpsilon
│    ├── MassWasting_HighConfidence
│    ├── MassWasting_LowConfidence
│    ├── Oultines_Bright
│    ├── Oultines_Dark
│    ├── Pits
│    ├── Streaks_Fan
│    ├── Streaks_Linear_Dense
│    ├── Streaks_Linear_Sparse
│    ├── Streaks_Transverse
│    └── Streaks_Wispy
├── ScottPetersen_SeniorThesis.pdf</pre>

#### README.md
This file.

#### LICENSE.txt
Licensing information for data and code contained in this repository.

#### SemiAutomatedCrestlineMapping.ipynb
This is a Python notebook with the code we developed based on Telfer et al. (2015)'s code to partially automatically map dune crestlines from a DEM. Documentation within the notebook describes the code's usage.

#### SedimentaryFeatureMap
This folder contains sub-folders of each class of feature mapped on Venus. Features were mapped as polygons in ArcGIS Pro version 3.2.0. The folders are named after the class of feature they contain the map for. Each map is saved in each folder as .cpg, .dbf, .prj, .sbn, .sbx, .shp, .shp.xml, and .shx files.
<br>.shp files should be used for best results in ArcGIS Pro.
<br> Please see ScottPetersen_SeniorThesis.pdf for a full description of each class of feature and a discussion of mapping results.
<br>

#### _Brief Description of Each Feature Class_
* Dark_LowEpsilon: Radar dark and low dielectric constant, suspected to be sedimentary.
* MassWasting_HighConfidence: Instances of mass wasting with confident interpretation.
* MassWasting_LowConfidence: Suspected instances of mass wasting, but not enough confidence to classify them as confirmed instances of mass wasting.
* Outlines_Bright: Radar-bright "halo" around topographic features. Often associated with LowConfidence_MassWasting
* Outlines_Dark: Radar-dark "halo" around topographic features. Often associated with wind streaks, and can be similar to Dark_LowEpsilon
* Pits: Chains of pits. While not sedimentary, these were noted anyway as some may be volcanic in nature, and thus could generate pyroclastic sediments.
* Streaks_Fan: Wind streaks with small length-to-width ratios, usually attached to a shield volcano.
* Streaks_Linear_Dense: Series of densely packed streaks with high length-to-width ratios.
* Streaks_Linear_Sparse: Wind streaks with high length-to-width ratios with few or no neighbors.
* Streaks_Transverse: Wind streaks that follow topography and have a homogenous appearance.
* Streaks_Wispy: Meandering radar-dark wind streaks.
<br> Wind streak classification is based on Greeley et al. (1995).

#### ScottPetersen_SeniorThesis.pdf
This is a .pdf file of Scott Petersen's senior thesis. Please read this document for a full description of the sedimentary map.

### Availability
This repository is also posted on the University of Arizona's ReDATA system with the DOI https://doi.org/10.25422/azu.data.29055653

### Acknowledgements
Travel to the 56th Lunar and Planetary Science Conference and parts of this work were funded by NASA grant 80NSSC23K0158 to L. Carter as part of the VenSAR Science Team.

### References
Greeley, R., Bender, K., Thomas, P. E., Schubert, G., Limonadi, D., Weitz, C. (1995). Wind-Related Features and Processes on Venus: Summary of Magellan Results. Icarus, 115, Pp. 399-420. Doi: https://doi.org/10.1006/icar.1995.1107

<br>Telfer, M. W., Fyfe, R. M., Lewin, S. Automated mapping of linear dunefield morphometric parameters from remotely-sensed data. Aeolian Research, 19, Pp. 215-224. Doi: http://dx.doi.org/10.1016/j.aeolia.2015.03.001
