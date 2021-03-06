# survey_additional_analysis

This repository contains specific analysis for the RSE survey 2017 UK. The full results are available on the following [repository](https://github.com/softwaresaved/international-survey) in this [notebook](https://github.com/softwaresaved/international-survey/blob/master/analysis/results_uk_2017_narrative.ipynb).
While the results in the original repository give an overview of the dataset, the notebooks here aims to answer specific questions and are more in-depth analysis.

## Analysis

* [interdisciplinary_aspects_of_research_software_engineers_in_uk.ipynb](interdisciplinary_aspects_of_research_software_engineers_in_uk.ipynb): Analysis of the interdisciplinary aspect of RSE and the flow between disciplines
* [dropping_participants_process.ipynb](dropping_participants_process.ipynb): Detail the reasons why participants are dropped from the raw data to create a cleaned dataset. NB: It is impossible to rerun this notebook as the raw data are not made publicly availabe

## Files

* [data](data/): contains the data file in csv format
* [include](include/): contains different modules needed for the analysis
* [.gitignore](.gitignore): contain the different files to ignore
* [LICENCE](LICENSE): the BSD 3-clause "New" licence file
* [README.md](README.md): this file
* [requirements.txt](requirements.txt): list of needed packages for the analysis

## Deployment

It is possible to run the different notebook or use different dataset if the structure match the UK survey (which mneans all the international surveys done in 2017), except when it is specified (in case of the raw data is needed).

1. Create a virtual environment for python3

`virtualenv venv`

2. Activate the virtual environment

`source venv/bin/activate`

3. Install the required packages

`pip install -r requirements.txt`

4. Activate the virtual environment for jupyter

`jupyter nbextension install ipykernel_launcher --user`

5. Activate the extension for the jupyter widget
`jupyter nbextension enable --py --sys-prefix widgetsnbextension  # can be skipped for notebook version 5.3 and above`

5. Run jupyter notebook

`jupyter notebook`

6. In the jupyter menu called 'Kernel', select 'Change Kernel', and then the kernel called 'venv' (if it is the name used for step 1 and 2)
