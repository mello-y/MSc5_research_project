# Data- and Projectmanagement

This section provides a description on the dataset and its evaluation. Further, projectmanagement aspects are addressed.  

## Dataset description and evaluation 

The underlying data of this project originates from the study "Functional MRI connectivity accurately distinguishes cases with psychotic disorders from healthy controls, based on cortical features associated with brain network development" by [Morgan et al. (2020)](https://doi.org/10.1101/19009894). It can be accessed on [figshare](https://figshare.com/articles/dataset/Data_for_Functional_MRI_connectivity_accurately_distinguishes_cases_with_psychotic_disorders_from_healthy_controls_based_on_cortical_features_associated_with_brain_network_development_/12361550), the respective github repository can be found [here](https://github.com/jmyoung36/fMRI_connectivity_accurately_distinguishes_cases) where everything is well documented and provided clearly. All the data is preprocessed and analyses were run with Matlab. 

### Five different MRI metrics

The data contains three different samples being Dublin, Maastricht and Cobre and five different MRI metrics for each sample (while in the Cobre dataset not every MRI metric was assessed). These are 

	- Macrostructural MRI
	- Microstructural MRI
	- Functional MRI
	- fMRI Connectivity and Network Analysis
	- Structural Connectivity.

In the following, the assessment of each metric is briefly explained.

#### Macrostructural MRI: cortical thickness (CT)

For the **macro-structural data**, T1-weighted MPRAGE images were used. The images were aquired with MPRAGE sequences, capturing high tissue contrast and providing high spatial resolution with whole brain coverage in a short scan time [(Wang et al.,2014)](https://doi.org/10.1371/journal.pone.0096899). These were already preprocessed by a prior pipeline [(Withtaker et al., 2016)](https://pubmed.ncbi.nlm.nih.gov/27457931/), using the command from FreeSurfer called "recon-all" [(Dale et al., 1999)](https://pubmed.ncbi.nlm.nih.gov/9931268/). The surface was parcellated according to the Desikan-Killiany atlas [(Desikan et al., 2006)](https://www.sciencedirect.com/science/article/abs/pii/S1053811906000437?via%3Dihub) (also see [here](https://mello-y.github.io/MSc5_research_project/code/Data_exploration.html#demographic-data)). For each of those regions cortical thickness was estimated.



#### Microstructural MRI: Mean Diffusivity (MD) and Fractional Anisotropy (FA)

Cortical measures of MD and FA were estimated for all brain regions from diffusion weighted images (DWI) using FreeSurfer’s trac-all command. DWIs were aquired using echo-planar sequences (EPI). 

#### Functional MRI (fMRI)

FMRI data were acquired using EPI sequences. For more concrete information on the EPI sequence parameters and the fMRI images for each sample consult “Functional MRI” ([Morgan et al. (2020), p. 2](https://doi.org/10.1101/19009894)). 

#### fMRI Connectivity and Network Analysis

To estimate a functional connectivity matrix for each subject from the regional, normalized wavelet coefficients, sparse inverse covariance were used.

#### Structural Connectivity and DWI Tractography

Parcellated T1-weighted MRI images were registered to corrected DWI images, a diffusion profile for each voxel was created and white matter tracts were identified with deterministic streamline tractography. 

### Demographic Data 

For each sample demographic data such as age and gender are also provided.


For this project, however, only the **macro and micro-structural** data will be used (also see [reflection on the research process](https://mello-y.github.io/MSc5_research_project/general_information/Discussion.html). On top of that, the data for only Dublin is going to be explored since it provides the best image quality (see Table 1 in [Young et al., 2020)](https://doi.org/10.1101/19009894)) and not every modality was measured for the Cobre dataset.

## Projectmanagement

In the following, information on projectmanagement-related aspects are provided. These include version control, documentation, FAIRness principles and the computational environment. 

### Version control

Version control makes it feasible to monitor and track the progress in projects. Changes made with progress, version control allows to access different versions of the files. 
In this project, Git is used for version control and Github as an online platform to document this project. The respective repository can be accessed [here](https://github.com/mello-y/MSc5_research_project). The project is also documented on [OSF](https://osf.io/g8j2c/). The literature used for this project is documented in [Zotero](https://www.zotero.org/mello_y/collections/MWC4DX9B). 

### Computational Environment

To ensure the reproducibility of this project and code, there is a requirements_code.txt file in the content/code folder of repository. This file contains all the packages and modules that are needed to run the code. To install the modules, the file can be downloaded from the repository. To create the same computational environment, create a new conda environment (for further information on conda environments see [here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)). When the conda environment is created, activate it and run the following command in the terminal:

```pip install -r requirements_code.txt ```

Now, you should be set up with all the neccessary modules and packages to run the code. 

### Openlab notebook

The openlab notebook serves the purpose of documenting the monthly progress of the project. It is structured in a way with a list of goals when working on the project and things to tackle working next time on the project. Click [here](https://mello-y.github.io/MSc5_research_project/open_lab_notebook/html) to get to the openlab notebook.

### Is the project/data “FAIRified”?

The FAIR principles stand for Findability, Accessibility, Interoperability, and Reuse of digital assets and were first published in 2016 in [“FAIR Guiding Principles for scientific data management and stewardship”](https://www.go-fair.org/fair-principles/). These principles imply that data must be easy to find and discoverable with metadata, available and obtainable, interoperable in terms of both syntactically parseable and semantically understandable allowing the exchange and reuse between researchers, institutions and organizations and most importantly explicitly described and shared with the least restrictive licenses making it feasible to optimize the reuse of the data so that they can be replicated.
The data used in this project meets all criteria. It is clearly described, where and how the data can be found and accessed. Also, the code to do so is provided. Interoperability is also assured. 
The data is reusable since it is shared without license, everything is well documented and described. 




