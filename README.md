## Overview

This repository contains six CSV files derived from three laboratory-scale photobioreactor prototypes investigated as bioactive shading systems. The datasets include region-of-interest-based illuminant features and sparse 3D point-cloud features extracted from multi-view experimental images.

The data support an AI-assisted prediction method developed to estimate biomass density and spatial diffusion in building-integrated photobioreactors under limited-data and variable-illuminance conditions. The study examines how image-derived illuminant and spatial features can be associated with biomass distribution and subsequently used to assess the shading performance of PBR-based façade configurations.

## Research Purpose

The purpose of the dataset is to support the development and validation of a limited-data prediction workflow for estimating biomass density and spatial diffusion in photobioreactors.

The research specifically investigates the relationship between:

* pixel-wise illuminant characteristics extracted from predefined regions of interest;
* sparse three-dimensional spatial features reconstructed from multi-view images;
* biomass density and spatial diffusion within three laboratory-scale PBR prototypes; and
* The potential contribution of predicted biomass distribution to the visual-comfort performance of PBR-based façade shading systems.

The prediction workflow combines illuminant feature extraction using an LSMI-U-Net, SIFT-based sparse 3D point-cloud reconstruction, and few-shot model-agnostic meta-learning with a fully connected neural network as the base learner.

## Dataset Contents

The repository contains two corresponding feature datasets for each experimental case.

### Illuminant Feature Datasets

1. **`case_1_illuminant_features_by_roi.csv`**
   Pixel-wise and regional illuminant features extracted from predefined regions of interest in Experimental Case 1.

2. **`case_2_illuminant_features_by_roi.csv`**
   Pixel-wise and regional illuminant features extracted from predefined regions of interest in Experimental Case 2.

3. **`case_3_illuminant_features_by_roi.csv`**
   Pixel-wise and regional illuminant features extracted from predefined regions of interest in Experimental Case 3.

### Sparse 3D Point-Cloud Feature Datasets

4. **`case_1_sparse_3d_point_cloud_features_by_roi.csv`**
   Spatial and geometric features extracted from the ROI-based sparse 3D point-cloud reconstruction of Experimental Case 1.

5. **`case_2_sparse_3d_point_cloud_features_by_roi.csv`**
   Spatial and geometric features extracted from the ROI-based sparse 3D point-cloud reconstruction of Experimental Case 2.

6. **`case_3_sparse_3d_point_cloud_features_by_roi.csv`**
   Spatial and geometric features extracted from the ROI-based sparse 3D point-cloud reconstruction of Experimental Case 3.

## Methodological Context

The illuminant features were extracted from predefined image regions using an LSMI-U-Net-based pixel-wise feature-extraction workflow. Sparse 3D point-cloud features were generated from multi-view image observations using SIFT-based feature detection and matching.

These complementary feature categories were used to model the relationship between illuminant conditions, biomass density, and biomass spatial diffusion. A few-shot MAML framework with an FCNN base learner was used to examine whether this relationship could be learned and adapted under limited-data conditions.

The resulting predictions were further considered in a scaffold-guided biomass-redistribution workflow for evaluating photobioreactors as adaptive bioactive shading systems.

## Application-Level Evaluation

The associated study evaluates the shading configurations in a reference office model derived from Case 600 of ASHRAE Standard 140. The investigated configurations include passive louvers, non-adaptive PBR panels, and an AI-supported scaffolded-PBR configuration.

Performance is assessed using:

* glare autonomy;
* daylight glare probability; and
* visual comfort performance.

The dataset therefore supports both prediction-model validation and the investigation of biomass density and spatial diffusion as potential shading-control variables in PBR-based façades.

## Intended Use

The data may be used for research concerning:

* prediction of biomass density and spatial diffusion;
* analysis of illuminant–biomass relationships;
* limited-data and few-shot learning;
* image-based monitoring of photobioreactors;
* sparse 3D reconstruction of biomass distribution;
* assessment of PBR-based bioactive shading systems; and
* future scaffold-guided and airflow-driven biomass redistribution.

## Associated Research

The dataset was generated for a study that develops an AI-supported method for predicting biomass density and spatial diffusion in building-integrated photobioreactors through a combined experimental and simulation-based workflow.

The method is evaluated using three laboratory-scale PBR prototypes, limited multi-view image datasets, and task-specific illuminance simulations. Its outputs are used to investigate PBRs as bioactive façade-shading systems and to assess the potential role of biomass density and spatial diffusion as variables for future adaptive shading regulation.

Publication details and the permanent dataset DOI will be added following publication and archival release.

## License

This dataset is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

Users may share and adapt the dataset for any purpose, provided that appropriate credit is given, a link to the license is included, and any modifications are clearly indicated.
