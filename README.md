# Molecular Dynamics Simulation and Analysis workshop

## Target audience

This is a course aimed at beginners in biomolecular simulation. It is expected that students are already familiar with key concepts of molecular dynamics simulation theory, and have a basic working knowledge of [Jupyter notebooks](https://jupyter-notebook.readthedocs.io/en/stable/), Python (especially the [NumPy library](https://numpy.org/)), and the bash shell.


## Schedule

The course is constituted of lectures (L1-8) and practical (P) sessions, subdivided in two units. Unit 1 is dedicated to providing foundations on protein structure and their preparation for molecular dynamics (MD) simulation. Unit 2 is dedicated to describing means of extracting information from the MD simulation of a protein.

### Unit 1: Simulation Preparation

| Session                            | Materials |
|------------------------------------|-----------|
| L1: Introduction to Proteins | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/1_Introduction/Lecture_1_Introduction.pdf) | 
| L2: Understanding Protein Systems | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/2_Protein_Preparation/Lecture_2_Protein_Prep.pdf)
| P: Understanding Protein Systems, contd. | [Webserver](https://server.poissonboltzmann.org/pdb2pqr)|
| L3: Protein-Ligand Docking                 |  [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/3_Docking/Lecture_3_Docking.pdf)| 
| P: Protein-Ligand Docking                 |  [![Docking](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/3_Docking/3_Docking.ipynb)| 
| L4: Simulation Setup          | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/4_Simulation_Setup/Lecture_4_Simulation_setup.pdf) |
| P: Simulation Setup          | [![Simulation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/4_Simulation_Setup/4_Simulation_Setup.ipynb) |


### Unit 2: Simulation Anaylsis


| Session                                             | Materials |
|-----------------------------------------------------|-----------|
| L5: Simulation Basic Analyses             | [Lecture Slides](5_Analysis_MDAnalysis/Lecture_5_Analysis_MDAnalysis.pdf)|
| P: Simulation Basic Analyses             | [![Analysis_0](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/5_Analysis_MDAnalysis/5_Analysis_MDAnalysis.ipynb)|
| L6: Dimensionality Reduction                  | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/Lecture_6_DR.pdf)  |
| P: Dimensionality Reduction, part 1           |  [![Analysis_1](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/6_Analysis_DR_part1.ipynb)|
| P: Dimensionality Reduction, part 2           | [![Analysis_2](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/6_Analysis_DR_part2.ipynb)|
| L7: Clustering   | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/7_Analysis_clustering/Lecture_7_Clustering.pdf)|
| P: Clustering   | [![Analysis_3](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/7_Analysis_clustering/7_Analysis_clustering.ipynb) |
| L8: Data Classification    | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/8_Analysis_classification/Lecture_8_classification.pdf) | 
| P: Data Classification  | [![Analysis_4](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/8_Analysis_classification/8_Analysis_classification.ipynb) |


## Running the workshop


### Google Colab

The workshop is designed to run on Google Colab and all workshop notebooks run directly from your browser, no installation is required. In particular, please note that the Open Force Field material in the Jupyter notebook of session [4_Simulation_Setup](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/4_Simulation_Setup) will not natively run on Windows machines. For extra information [see here](https://docs.openforcefield.org/en/latest/install.html#openff-on-windows).


### Setting up your own Python environment 

Instructions for setting up your environment to run this workshop locally are provided in [`INSTALL.md`](INSTALL.md).
A full list of the required Python packages can be seen inside [`environment.yml`](environment.yml).

## Contributing to the resource and raising issues

Contributions to the learning resource are welcome. Contributions can be made through creating an issue or a pull request.

### For issues
- To create an issue, contributors are encouraged to follow the [GitHub quickstart guide on creating an issue.](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue)
- Make sure to include the following into your issue:
	-  Are you using the Colab or a local install version
	-  If it is a local install version what version of the different packages are you running?
	-  Are you using it as a student or instructor
	-  Is the issue reporting a bug, an enhancement, or a feature request		

### For pull requests
- To create a pull request, contributors are encouraged to follow the [GitHub quickstart guide on creating a fork and submitting a pull request.](https://docs.github.com/en/get-started/quickstart/contributing-to-projects)

### Telling us about how you are using the resource
If you just want to tell us how you have been using the resource just send us an email or raise an issue pointing to your work. 

## Reusing and building on the material for your own course

The easiest way is by cloning the material and adapting it to your needs. This can be just using some partial material or expanding on the existing material. The best way to do this is by either [cloning](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) the repo and building up on it, or using the current repository as a [template repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) for your own or your organisations GitHub account, for more details see the [overview](overview.md) document. 



## Licenses

- The MDAnalysis logo and its derivatives are licensed under the [Creative Commons Attribution-NoDerivs 3.0 Unported License](https://creativecommons.org/licenses/by-nd/3.0/).
- The MDAnalysis material in folder [5_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/5_Analysis_MDAnalysis) is licenced under CC-BY 4.0 
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" title='This work is licensed under a Creative Commons Attribution 4.0 International License.' align="right"/></a>
- The Docking material in folder [3_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/3_Docking) is licensed under and Apache-2.0 and MIT license.
- The Open Force Field material in folder [4_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/4_Simulation_Setup) is licensed under MIT license.
- Material in folders [1_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/1_Introduction),
[2_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/2_Protein_Preparation),
[6_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/5_Analysis_DR),
[7_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/6_Analysis_clustering)
[8_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/8_Analysis_classification), and
[9_\*](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/tree/main/9_Analysis_MSM) is licenced under CC-BY-SA 4.0.
<a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="width=50" src="https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png" title='This work is licensed under a Creative Commons Attribution 4.0 International License.' align="right"/></a>


## Authors

- [Dr Matteo Degiacomi, University of Edinburgh](https://degiacomi.org)
- [Dr Antonia Mey, University of Edinburgh](https://mey-research.org/)
- [Dr Micaela Matta, King's College London](https://www.kcl.ac.uk/people/micaela-matta)
- Dr Richard Gowers
