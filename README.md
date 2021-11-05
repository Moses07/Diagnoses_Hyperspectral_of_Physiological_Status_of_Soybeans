# Diagnoses_Hyperspectral_of_Physiological_Status_of_Soybeans
Digital Solution - Stress Detection: Diagnosis of the Physiological Status of Soybean Crop by means of Hyperspectral Images
# Description of the solution
This solution is targeted at small, medium and large soybean growers and aims to allow the detection by remote sensing (via drone, vants) of the nutritional status of glycine max soybean plants under large-scale cultivation conditions (possible nutritional deficiencies of macro and micronutrients) and water stress (abiotic), from aerial images with hyperspectral camera.

## Technology involved
> Background
Use of hyperspectral imaging technology (spectrometry). Machine Learning algorithms for processing the images and detecting nutrient levels in plants and stress diagnosis. Visualization of the results through an online GIS platform (SaaS system) with visualizations of the diagnostic maps, allowing the generation of PDF reports, thematic maps and files in shapefile format to direct actions in the soybean fields.

> MACHINE LEARNING ALGORITHMS
For this, 204,800 (320x640) combinations are used. The following machine learning algorithms were used in this framework: k-Nearest Neighbor (kNN) and Random Forest (RF). The training methods were evaluated based on Cross-validation and exclusion. The Relief-F metric from the algorithms' prediction was used to determine the most contributory wavelength or spectral region associated with each nutrient or plant stress symptom.

## Dataset
Source : 
The operation of the product is based on remote sensing data (HIS Drone) to be collected at the soybean development stages V4 (30-35 DAP) and R1 (50-55 DAP) during the soybean crop cycle.
Combination of anomaly assessments (NDVI, crop yield) in soybean using drone imagery. Mapping and quantification of areas affected with nutrient deficiency or low, medium to high stress (and/or areas of low yield potential). Maps can be used for localized and accurate application of nutritional and physiological products during the crop cycle. They can also be used by plant nutrition and physiological product companies for marketing purposes, to demonstrate the benefits of the products that have been applied to the crop, to better position the products, and to allow comparison with the untreated area.

The Soybean Physiological Status Diagnosis product is based on capturing light waves that are invisible to human vision, using hyperspectral images, a technology originally developed by NASA. This allows Gamaya to extract much more information from a single pixel, enabling it to detect complex problems in fields, thus generating a hyper-realistic display of agricultural land across the entire range of wavelengths, from ultraviolet to infrared, in addition to the small spectrum that is detectable by human vision. The Gamaya camera is capable of detecting 31 bands between the visible and near infrared range, reaching a detection range between 350 - 2500nm.
Healthy plants reflect light in different ways than sick plants. So by capturing every last nuance of light in soybean fields, it is possible to create granular crop diagnostic maps that show farmers how to increase yields, avoid pests, and deliver the nutrients needed for a bountiful harvest. This is an innovative approach that is helping farmers meet their growing demands in a sustainable way.
For the calibration and training of the algorithm data is collected from soybean field trials, in experimental plots delimited in an area of known nutrient stress and deficiency (ground truth), leaf samples will be collected for analysis of nutrient levels and also from these same soybean plants spectral data measured with a Fieldspec ASD FieldSpec® HandHeld 2 spectroradiometer and the surface reflectance and first derivative spectra from the spectral range of 380 to 1020 nm are evaluated. A total of 320 spectral signatures are collected, and the leaf nutrient content (N, P, K, Mg, S, Cu, Fe,Mn, and Zn) is associated with them.
For this, 204,800 (320x640) combinations are used. The following machine learning algorithms were used in this framework: k-Nearest Neighbor (kNN) and Random Forest (RF). The training methods were evaluated based on Cross-validation and exclusion. The Relief-F metric from the prediction algorithms was used to determine the most contributory wavelength or spectral region associated with each nutrient or plant stress symptom.
This approach is able to return, with high predictions (R2), nutrients such as N (0.912), Mg (0.832), Cu (0.861), Mn (0.898), and Zn (0.855) and, to a lesser degree, P (0.771), K (0.763), and S (0.727). These accuracies were obtained with different algorithms, but RF was the best suited to model more of them. The results indicate that for soybean leaves, surface reflectance data are best suited to predict macronutrients and physiological stress, while first derivative spectra are best linked to micronutrients

The data consists of xx csv files from January 20xx to December 20xx in the form of daily prices of basic commodities. The data is still not 100% clean and neat, so it needs cleansing and formatting. The data dictionary of the dataset is as follows:
date: Daily date
Commodity: Commodity
Price: Price

## Data Analysis

## PEFORMANCE AND ACCURACY OF THE ALGORITHMS


