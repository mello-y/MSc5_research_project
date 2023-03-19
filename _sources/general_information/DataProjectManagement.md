# Data- and Projectmanagment

This section carries information on the used dataset and its evaluation. Further, it provides information on the version control and the computational environment within wich the project was conducted. Also, the whole process is described in the openlab notebook.

## Dataset description and evaluation

The data I am going to use for the project is available on [figshare](https://figshare.com/articles/dataset/Data_for_Functional_MRI_connectivity_accurately_distinguishes_cases_with_psychotic_disorders_from_healthy_controls_based_on_cortical_features_associated_with_brain_network_development_/12361550) and originates from the paper "Functional MRI connectivity accurately distinguishes cases with psychotic disorders from healthy controls, based on cortical features associated with brain network development" by [Young et al. (2020)](https://doi.org/10.1101/19009894). The github repository for the study can be accessed [here](https://github.com/jmyoung36/fMRI_connectivity_accurately_distinguishes_cases).

### What does the data contain? General overview

The already pre-processed data contains different metrics for three different samples being Dublin, Maastricht and Cobre. 

For the **macro-structural** data ***cortical thickness (CT)*** was estimated for 308 cortical regions according to a derived version of the Desikian-Killiany atlas [(Desikan et al, 2006)](https://www.sciencedirect.com/science/article/abs/pii/S1053811906000437?via%3Dihub). The files for the derived and adjusted atlas can be found in this [github repository](https://github.com/RafaelRomeroGarcia/subParcellation), the respective paper [here](https://doi.org/10.1016/j.neuroimage.2011.10.086).

The **micro-structural** data contains diffusion weighted images (DWI) from which regional cortical measures such as ***mean diffusivity (MD)*** and ***fractional anisotropy (FA)*** were estimated.

There are further metrics such as ***functional magnet resonance imaging data (fMRI), fMRI connectivity and network data*** and ***structural connectivity*** and ***DWI tractography***. For project purposes, only the **macro and micro-structural** data will be used. On top of that, the data for only Dublin is going to be explored since it provides the best image quality (see Table 1 in [Young et al., 2020)](https://doi.org/10.1101/19009894) and not every modality was measured for the Cobre dataset. 

The data also contains demographic data such as age and gender.
## Version control

Version control makes it feasible to monitor and track the progress in projects. Changes made with progress, version control allows to access different versions of the files. 
In this project, Git is used for version control and Github as an online platform to document the project. The repository can be accessed [here](https://github.com/mello-y/MSc5_research_project). The project is also documented on [OSF](https://osf.io/g8j2c/).
## Openlab notebook

The openlab notebook serves the purpose of documenting the monthly progress of the project. It is structured in a way with a list of goals when working on the project and things to tackle working next time on the project. Click [here](https://mello-y.github.io/MSc5_research_project/open_lab_notebook/html) to access the openlab notebook.


## Computational environment

In order to make the code reproducible for others, the specifications for the computing environment with the relevant modules and packages are documented in the requirements_code.txt file. The file can be found [here](https://github.com/mello-y/MSc5_research_project/tree/main/content/code).










