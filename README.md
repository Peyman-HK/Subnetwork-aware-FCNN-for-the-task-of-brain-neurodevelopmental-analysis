# Explainable subnetwork-aware FCNN for the brain neurodevelopmental analysis

There are three input datsets that should be read:
1- BOLD fMRI N-Bck data that is stored in the Mat file.
2- Power atlas template which encompasses information for the original ROIs and brian subnetworks
3- phenotypic information which include information such as age, IQ, etc. 

The model extract Pearson correlation from BOLD signals and then separate them to different lists of data based on their subnetwork information which is accessible by ROIs. 

The proposed FCNN, load all 14 lists of datasets since we have 14 subnetworks. This is computationally efficient since we group neurons of each subnetwork to the next layer instead of using a dense layer. 


![Fig1-Framework](https://github.com/Peyman-HK/Subnetwork-aware-FCNN-for-the-task-of-brain-neurodevelopmental-analysis/assets/30543473/3c093431-0ea3-4c0a-821c-366db2723439)






