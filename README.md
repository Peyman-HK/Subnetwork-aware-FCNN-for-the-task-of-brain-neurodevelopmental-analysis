# Explainable subnetwork-aware FCNN for the brain neurodevelopmental analysis

There are three input datsets that should be read:
1- BOLD fMRI N-Bck data that is stored in the Mat file.
2- Power atlas template which encompasses information for the original ROIs and brian subnetworks
3- phenotypic information which include information such as age, IQ, etc. 

The model extract Pearson correlation from BOLD signals and then separate them to different lists of data based on their subnetwork information which is accessible by the ROIs. 

The proposed FCNN, load all 14 lists of datasets since we have 14 subnetworks. This is computationally efficient since we group neurons of each subnetwork to the next layer instead of using a dense layer. 

