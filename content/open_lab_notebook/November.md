# November, 2022

## Wednesday, 02/11/2022
What I did today: 
- Read the paper "Functional MRI connectivity accurately distinguishes cases with psychotic disorders from healthy controls, based on cortical features associated with neurodevelopment" by Morgan et al. (2019) until the data section
- Made a list of literature to read for psychosis as a brain network disorder
- Made an overview of the data and what the data contains (google doc)
- Made a list of questions regarding the data I don't understand (google doc)
- Went through the first section of course website (Cortical Maps)

To-do for next time working on the project:
- read psychosis paper (ET Bullmore, S Frangou, and RM Murray. The dysplastic net hypothesis: an integration of developmental and dysconnectivity theories of schizophrenia. Schizophrenia Research, 28: 143–156, 1997.)
- go through the list of questions regarding the data and research to get a better undestanding of the data
- work on notebook and the data exploration section
- briefly read the ML section (Morgan et al., 2019)

## Thursday, 03/11/2022
What I did today:
- read the paper ET Bullmore, S Frangou, and RM Murray. The dysplastic net hypothesis: an integration of developmental and dysconnectivity theories of schizophrenia. Schizophrenia Research, 28: 143–156, 1997
- went through some of the questions in the list 
- went through the MRI section on the course website

To-do for next time working on the project:
- research on the other questions
- maintain github repo and notebook
- briefly read the ML section (Morgan et al., 2019)

## Friday, 04/11/2022
What I did today:
- went trough some more questions in the list to get a better understanding of the data at hand
- went through the morphometric analyzes and diffusion MRI section on the course website
- read the ML section (Morgan et al., 2019) and made some pointers re things to do further research on
- updated github repo (added badges and requirements file)

To-do for next time working on the project:
- work on data exploration notebook
- add more info re the project to the README.md

## Saturday, 12/11/2022
What I did today:
- tried to find the derived atlas (from the Desikan-Killiany) that was used in the paper with 308 cortical regions
- researched about how to plot brain atlases (FreeSurfer, Nilearn, ggseg R module)

To-do next time working on the project:
- find the atlas and load it in jupyter notebook

## Wednesday, 16/11/2022
What I did today:
- tried to use the ggseg module and find a way how to use R within python since ggseg is a R module; to load the standard Desikan-Killiany atlas because I was not able to find the files for the derived atlas
- ggseg module did not work, could not figure it out

To-do next time working on the project:
- find the atlas and load it in jupyter notebook without using ggseg

## Friday, 18/11/2022
What I did today:
 - found the files for the derived form of the Desikan-Killiany atlas with 308 cortical regions
 - link for the repo: https://github.com/RafaelRomeroGarcia/subParcellation 

To-do next time working on the project:
- load the atlas in jupyter notebook

## Monday, 21/11/2022
What I did today:
- loaded the atlas in jupyter notebook
- provided more infos for github repo

To-do next time working on the project:
- provide more information regarding the atlas, other plotting tools, find out how to visualize the 308 cortical regions
- provide more information for github repo
- reorganize data exploration notebook

## Tuesday, 22/11/2022
What I did today:
- tried other plotting tools (3D)
- reorganized the structure of data exploration notebook
- started to provide information regarding demographic data 
- added more comments and descriptions in the notebook 

To-do next time working on the project:
- explore demographic data for both CT and DWI data subsets, visualize the data
- look for the .annot files, whether they provide more information regarding the regions in sense of visualizing the regions
- start exploring the CT data 

## Wednesday, 23/11/2022
What I did today::
- explored demographic data for both CT and DWI data subsets
- tried to visualize the data but it did not work: my idea was to use a grouped bar chart to visualize the amount of participants in the control and patient group with respect to their gender, for that tried to use matplotlib and seaborn

To-do next time working on the project:
- visualize the demographic data
- look for the .annot files, whether they provide more information regarding the regions in sense of visualizing the regions
- start exploring the CT data 

## Monday, 28/11/2022
What I did today:
- loaded the atlas in jupyter notebook with respective labels
- started CT data exploration section (explained what CT is and loaded data)
- added information and comments to the notebook
- after talking to my instructor, there is no need to visualize the demographic data
- watched a video about [Gradient descent](https://www.youtube.com/watch?v=3XOe0LwJw1s) and [Backpropagation](https://www.youtube.com/watch?v=Ilg3gGewQ5U)

To-do next time working on the project:
- get a better idea of how to explore the CT data 
        - what is the range of values in the data
        - what is the distribution of the values
        - separate for control and patient group?
        - what does the values mean?
- maintain github repo and notebook

## Tuesday, 29/11/2022
What I did today:
- plotted mean distribution of CT values for control and patient group using a violin plot
- started micro-structural data section with information regarding Mean Diffusivity (MD) and Fractional Anisotropy (FA)
- added information and comments to the notebook

To-do next time working on the project:
- look for specific brain regions to compare between control and patient group in CT
- start exploring the micro-structural data