# WearableEEG-ChronicPain-FeatureData

This repository contains feature matrices derived from dual-channel wearable EEG recordings used in the study:  
**"Assessment and biomarker exploration of chronic pain using a wearable EEG device"**  
(Chen et al., 2025, Discover Sensors).

## Dataset Description
- **Participants**: 20 patients with chronic pain (7 mild, 7 moderate, 6 severe).  
- **Recording device**: Custom dual-channel wearable EEG system (Fp1, Fp2).  
- **Preprocessing**: Bandpass (0.5–45 Hz), notch filter (50 Hz), SSA-ICA artifact removal.  
- **Segmentation**: 5-second non-overlapping epochs.  
- **Features extracted**:  
  - 34 time-domain  
  - 18 frequency-domain  
  - 26 nonlinear (including differential entropy across 5 frequency bands)  
  - **Total = 78 features per segment**  

The repository provides anonymized **feature matrices and class labels**. Raw EEG signals are not included due to ethics restrictions, but controlled access may be requested from the corresponding author.

## File Structure
- `allfeature.mat` – Feature matrix of all 960 segments
- `features_description.csv` – Names and descriptions of the 78 features
- `example.ipynb` – Example scripts for loading and exploring the feature matrices

## Usage
These data can be used to reproduce or extend the machine learning analyses reported in the paper. 

## Citation
If you use this dataset, please cite:  
Chen Y., Tian Y., Zhou H., Xu J., Sun Y., Zhao C., Liu H. (2025).  
*Assessment and biomarker exploration of chronic pain using a wearable EEG device.* Discover Sensors.  

## License
This dataset is made available under the [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).  
