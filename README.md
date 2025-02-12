# A seismic integrated deep learning approach for prediction of off-shore wind site Cone Penetration Test Data
This is a PyTorch implementation of deep learning model for Cone Penetration Test (CPT) Data prediction on ArcgisPro.

<p align="center">
<img src="misc/fig_1.png" width=60% height=60% class="center">
</p>

Figure 1:Fig.1. Deep Learning Model for CPT Data Prediction. The CPT and seismic data are utilized as input to the SNAM, which comprises two components: Neighborhood Selection and Feature Aggregation. In SNAM, the green dots represent the central points for feature aggregation, while the red dots denote the neighboring points. In the Feature Learning Module, the green dots indicate the aggregated CPT borehole points, and the black rectangles represent the sliding windows.
<br/>
<br/>

<p align="center">
<img src="misc/fig_2.jpg" width=60% height=60% class="center">
</p>

Figure 2:  CPT Data Prediction Results. Using cone resistance (QC) as an example. (a) Voxel interpolation results of the QC. The red cone-shaped markers indicate CPT borehole locations used for validation. (b), (c) Validation curves at the CPT borehole locations, with dashed lines indicating stratigraphic boundaries.
<br/>
<br/>
## Install

Our toolbox runs on ArcGIS Pro 3.2 with Python 3.8 and PyTorch 1.13.Please install ArcGIS Pro and use conda to install PyTorch 1.13.Please refer the [arcgis online help](https://pro.arcgis.com/en/pro-app/latest/help/projects/connect-to-a-toolbox.htm) to install the toolbox to arcgis pro

## source code
Please refer the [arcgis online help](https://pro.arcgis.com/en/pro-app/3.3/arcpy/geoprocessing_and_python/editing-script-tool-code.html) to view the sorce code.

## Additional Tools
Additional tools including import geology dataset, such as sesmic data(sgy fomart), CPT holes data(office excel format), stratigraphic horizon (ascii grid data), visualization are also provided. A install.exe provide to intsall [these additional tools](tools/install.exe).
## Model parameters
As shown in Figure 3, open the toolbox in ArcGIS Pro.
<br/>
CPT Validation: Enter the CPT borehole number to be validated.
<br/>
Seismic Profile Validation: Enter the seismic profile to be predicted.
<br/>
Prediction of Geotechnical Parameters: Select the geotechnical parameter to be predicted, such as cone resistance (QC).
<br/>
Seismic Attributes: Select the seismic attributes to be used, such as "Amplitude," "Envelope," "Phase," and "Frequency."
<br/>
Depth: Choose between Absolute Depth or Normalized Depth.
<br/>
Path: Enter the output path.
<br/>
Neighborhood Size and Sliding Window Size: Enter the respective parameters.
<p align="center">
    <img src="misc/fig_3.png" width=60% height=60%">
</p>
Figure 3:  Toolbox interface


