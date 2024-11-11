---
title: 'A course on the setup, running, and analysis of biomolecular simulations'
tags:
  - molecular simulation
  - python
  - graduate level
authors:
  - name: Matteo T. Degiacomi
    orcid: 0000-0003-4672-471X 
    affiliation: "1, 2"
  - name: Richard J. Gowers
    orcid: 0000-0002-3241-1846 
    affiliation: "3"
  - name: Micaela Matta
    orcid: 0000-0002-9852-3154
    affiliation: "4"
  - name: Antonia S. J. S. Mey
    orcid: 0000-0001-7512-5252
    affiliation: "2"

affiliations:
 - name: School of Informatics, University of Edinburgh, Informatics Forum, 10 Crichton St, Edinburgh EH8 9AB, United Kingdom 
   index: 1
 - name: EaStCHEM School of Chemistry, University of Edinburgh, Joseph Black Building, David Brewster Road, Edinburgh, EH9 3FJ, United Kingdom 
   index: 2
 - name: CHARM Therapeutics Ltd, 7 Pancras Square, London, N1C 4AG
   index: 3 
 - name: Department of Chemistry, King's College London, London, SE1 1DB, United Kingdom
   index: 4


date: 11 November 2024
bibliography: paper.bib
---

# Summary

We present an open-source course teaching how to set-up and analyse molecular dynamics (MD) simulations of biomolecules using proteins as a use-case. The course consists a blend of lectures and practical sessions using Jupyter notebooks.

# Statement of Need

Biomolecular systems were one of the first systems used in molecular dynamics (MD) simulations [@levitt1975computer]. As such biomolecular simulations build on a rich half a century history rich of methodological developments, embodied in a wide range of specialised software. The improvement in physical models dictating interatomic interactions coupled with an ever-increasing availability of computational power have enabled MD simulations to establish themselves as a technique complementary to experimental data [@hollingsworth2018molecular] [@ciccotti2022molecular]. Starting from the simulation of small proteins for only a few nanoseconds [@levitt1975computer], nowadays large biomolecular complexes featuring millions of atoms can be simulated for timescales orders of magnitude longer [@lindorff-larsen2011howa]. The data produced by MD simulations is noisy and high-dimensional though, and its usefulness is directly dependent on how faithfully the molecular system simulated recapitulates the physiochemical conditions of its real-world counterpart. Since the mid-1970s, significant progress has been made in automating the preparation of biologically relevant atomistic models and the analysis of simulation data. Nonetheless, modern computational scientists must still make critical decisions on how to assemble and simulate the system, as well as which quantities to extract from the resulting data to accurately explain or predict experimental outcomes.

The material presented in this course has been developed as training material for the CCPBioSim consortium. Since 2022, it has been delivered to three cohorts of 25-35 international postgraduates attending the UK-based CCP5 Summer School on Molecular simulation. A first key aspect of this course is that, under the same hood, it provides information on both the set-up and the analysis of MD simulations, typically presented separately. A second key aspect is that it demonstrates how machine learning techniques can be integrated in the analysis of MD simulations and used to extract relevant information from an MD simulation.


# Overview, Content, and Structure

## Target Audience 

This is a graduate-level course, aimed at beginners in biomolecular simulation. It is expected that students are already familiar with key concepts of molecular dynamics simulation theory, and have a basic working knowledge of Python and its core scientific packages (numpy, scipy, matplotlib).

## Content

The objective of this course is not to make students proficient in one or few selected software for MD simulation preparation, execution, or analysisis. Instead, it is aimed at providing students with a general overview of the key decision-making required to carry out MD simulations of biomolecules and extracting quantitative data from them. In this context, the course is subdivided in two Units featuring practical sessions and lectures. Practical sessions demonstrate how key concepts in molecular modelling are put into practice by exposing student to authentic tasks leveraging on commonly used Python packages, such as MDAnalysis [@michaud-agrawal2011mdanalysis] [@oliver_beckstein-proc-scipy-2016] [@alibay2023building] and scikit-learn [@pedregosa2011scikitlearn]. Lectures are software-agnostic and provide additional material to the course. While each practical session can be run by students on their own computer, these are also available in Google colab. This solution, requiring no local installation, is especially suitable for those unfamiliar with how to set-up a Python environment, or having limited access to computational resources.

### Unit 1: Simulation Preparation

The first Unit is dedicated to providing background on protein structure, and how to prepare a protein for biomolecular simulation. In this Unit, students learn about how to critically observe a protein structure, and make informed decisions required to set-up a simulation that faithfully recapitulates a biologically relevant system.

| Session                            | Materials |
|------------------------------------|-----------|
| L1: Introduction to Proteins | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/1_Introduction/Lecture_1_Introduction.pdf) | 
| L2: Understanding Protein Systems | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/2_Protein_Preparation/Lecture_2_Protein_Prep.pdf)
| L3: Protein-Ligand Docking                 |  [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/3_Docking/Lecture_3_Docking.pdf)| 
| P: Protein-Ligand Docking                 |  [![Docking](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/3_Docking/3_Docking.ipynb)| 
| L4: Simulation Setup          | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/4_Simulation_Setup/Lecture_4_Simulation_setup.pdf) |
| P: Simulation Setup          | [![Simulation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/4_Simulation_Setup/4_Simulation_Setup.ipynb) |

### Unit 2: Simulation Analysis

The second Unit is dedicated to providing the students with means to extract relevant quantitative information from a molecular dynamics simulation trajectory. A key aspect of this Unit lies in the demonstration of how machine learning techniques (clustering, dimensionality reduction, classification) can be used to extract meaningful information from noisty and high-dimensional data associated with biomolecular MD simulations.

| Session                                             | Materials |
|-----------------------------------------------------|-----------|
| L5: Simulation Basic Analyses             | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/5_Analysis_MDAnalysis/Lecture_5_Analysis_MDAnalysis.pdf)|
| P: Simulation Basic Analyses             | [![Analysis_0](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/5_Analysis_MDAnalysis/5_Analysis_MDAnalysis.ipynb)|
| L6: Dimensionality Reduction                   | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/Lecture_6_DR.pdf)  |
| P: Dimensionality Reduction, part 1           |  [![Analysis_1](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/6_Analysis_part1.ipynb)|
| P: Dimensionality Reduction, part 2           | [![Analysis_2](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/6_Analysis_part2.ipynb)|
| L7: Clustering   | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/7_Analysis_clustering/Lecture_7_Clustering.pdf)|
| P: Clustering   | [![Analysis_3](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/7_Analysis_clustering/7_clustering.ipynb) |
| L8: Data Classification    | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/8_Analysis_classification/Lecture_8_classification.pdf) | 
| P: Data Classification  | [![Analysis_4](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/8_Analysis_classification/1_classification.ipynb) |


# Assessment and feedback

Each Jupyter notebook contains information on a specific topic, as well as tasks the student is asked to carry out independently. The tasks range from interpreting data previously produced, to running presented code with different parameters, to solving a specific problem by implementing a short Python code. Solutions to all questions are provided in each notebook as drop-down cells, enabling students to self-assess their understanding.

In our teaching practice, we provide students with post-its of two different colours that can be displayed on their computer screen --- yellow indicating that everything is clear, pink indicating that help is required. At the end of each practical session, studends are asked to use these same post-its to provide instructors with feedback on something they liked (yellow post-it), and something that requires improvement (pink post-it). In the three years we have delivered this course, this appoach has enabled us to gather comprehensive feedback, helping us fine-tuning the teaching material and our own delivery style. A key observation is that students, when presented with a new notebook, especially appreciate the instructors spending few minutes describing the overall notebook structure and the tasks it features, before working through the beginning of it.


# Conclusion

Thanks to the increasing availability of computational power and software automating many of the processes associated with biomolecular simulation and analysis, the palette of questions addressable with MD is broadening. While this is positive, it remains crucial for computational scientists to have a clear understanding of what is being simulated and how. Indeed, to date many decisions associated with system building and analysis cannot be delegated to a machine without human verification. In this context, we see our course as a first stepping-stone, detailing the key decisions that need to be made, providing examples of how this can be done in practice, and directing learners to relevant software and specialized analysis techniques for further education.

Despite its long history, MD remains an evolving field. New techniques that push the boundaries of what is possible keep emerging, as exemplified by the current revolution associated with the integration of modern machine learning techniques in molecular modelling pipelines. While we expect that majority of the concepts presented in this course will be valid for many years to come, we are endeavouring to keeping the course material up-to-date by highlighting current methodological trends. For instance in the latest iteration of this course we have introduced a discussion on how how to interpret and use models produced by AlphaFold [@jumper2021highly].


# Contributions to the course

MTD and ASJSM conceived the course with contributions from RJG and MM.


# Acknowledgements 

Parts of the material in this course have been adapted from other sources with the agreement of respective authors. In this context, we would like to acknowledge Matt Thompson, Jeff Wagner, and Josh Mitchell for the material featured in the OpenFF tutorials, César Ramírez-Sarmiento and collaborators for material featured in the Autodock tutorial. We also wish to acknowledge Charlie Laughton for inspiration on discussing RMSD in conjunction with equilibration, and Irfan Alibay and Rohan Gorantla for help with setting up Colab environments.


# References
