---
title: 'Course Materials for an Introduction to Data-Driven Chemistry'
tags:
  - molecular simulation
  - python
  - graduate level
authors:
  - name: Matteo T. Degiacomi
    orcid: 0000-0003-4672-471X 
    affiliation: "1"
  - name: Micaela Matta
    orcid: xxx
    affiliation: "2"  
  - name: Antonia S. J. S. Mey
    orcid: 0000-0001-7512-5252
    affiliation: "3"

affiliations:
 - name: Department of Physics, Durham University, South Road, Durham, DH1 3LE, United Kingdom 
   index: 1 
 - name: xxxx
   index: 2
 - name: EaStCHEM School of Chemistry, University of Edinburgh, Joseph Black Building, David Brewster Road, Edinburgh, EH9 3FJ, United Kingdom 
   index: 3


date: 12 August 2024
bibliography: paper.bib
---

# Summary

We present an open-source course featuring a blend of lectures and practical sessions teaching how to set-up and analyse molecular dynamics (MD) simulations of biomolecules, with a particular focus on proteins. The material presented in this course has been delivered since 2022 to cohorts of 30-40 postgraduates attending the UK-based CCP5 Summer School on Molecular simulation.

# Statement of Need

Biomolecular systems have been the first to be subjected to molecular dynamics (MD) simulations, and are thus underpinned by half a century history rich of methodological developments, embodied in a vast array of available software. The improvement in physical models dictating interatomic interactions couple with an ever-increasing availability of computational power have enabled MD simulations to establish themselves as a technique complementary to experimental data. Starting from the simulation of small proteins for only a few nanoseconds, nowadays large biomolecular complexes featuring millions of atoms can be simulated for timescales orders of magnitude longer. The data produced by MD simulations is noisy and high-dimensional though, and its usefulness is directly dependent on how faithfully the molecular system simulated recapitulates the phisiochemical conditions of its real counterpart.
While since the mid-70s strides have been made to automate the preparation of biologically-relevant atomistic models and the analysis of simulation data, the modern computational scientist is still required to make critical decisions on how the system should be assembled and simulated, and on which quantities should be extracted from the resulting simulation so as to precisely and accurately explain, or predict, experimental data.

# Overview, Content, and Structure

## Target Audience 

This is a graduate-level course, aimed at beginners in biomolecular simulation. It is expected that students are already familiar with key concepts of molecular dynamics simulation theory, and have a basic working knowledge of Python and its core scientific packages (numpy, scipy, matplotlib).

## Content

The objective of this course is not to make students proficient in one or few selected software for MD simulation preparation, execution, or analysisis. Instead, it is aimed at providing students with a general overview of the key decision-making required to carry out MD simulations of biomolecules and extracting quantitative data from them. In this context, the course is subdivided in two Units featuring lectures and practical sessions. Lectures are software-agnostic, whereas practical sessions demonstrate how those concepts could be put into practice by exposing student to authentic tasks leveraging on commonly used Python packages. While each practical session can be run by students on their own computer, these are also available in Google colab. This solution, requiring no local installation, is especially suitable for those unfamiliar with how to set-up a Python environment, or having limited access to computational resources.

### Unit 1: Simulation Preparation

The first Unit is dedicated to providing background on protein structure, and how to prepare a protein for biomolecular simulation. In this Unit, students learn about how to critically observe a protein structure, and make informed decisions required to set-up a simulation faithfully recapitulating a biologically relevant system.

| Session                            | Materials |
|------------------------------------|-----------|
| L1: Introduction to Proteins | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/1_Introduction/Lecture_1_Introduction.pdf) | 
| L2: Understanding Protein Systems | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/2_Protein_Preparation/Lecture_2_Protein_Prep.pdf)
| P: Understanding Protein Systems, contd. | [Webserver](https://server.poissonboltzmann.org/pdb2pqr)|
| L4: Protein-Ligand Docking                 |  [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/3_Docking/Lecture_3_Docking.pdf)| 
| P: Protein-Ligand Docking                 |  [![Docking](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/3_Docking/3_Docking.ipynb)| 
| L3: Simulation Setup          | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/4_Simulation_Setup/Lecture_4_Simulation_setup.pdf) |
| P: Simulation Setup          | [![Simulation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/4_Simulation_Setup/4_Simulation_Setup.ipynb) |


### Unit 2: Simulation Anaylsis

The second Unit is dedicated to providing the students with means to extract relevant quantitative information from a molecular dynamics simulation trajectory. A key aspect of this Unit lies in the demonstration of how machine learning techniques (clustering, dimensionality reduction, classification) can be used to extract meaningful information from noisty and high-dimensional data associated with biomolecular MD simulations.

| Session                                             | Materials |
|-----------------------------------------------------|-----------|
| L5: Simulation Basic Analyses             | [Lecture Slides](5_Analysis_MDAnalysis/Lecture_5_Analysis_MDAnalysis.pdf)|
| P: Simulation Basic Analyses             | [![Analysis_0](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/5_Analysis_MDAnalysis/5_Analysis_MDAnalysis.ipynb)|
| L6: Dimensionality Reduction                  | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/Lecture_6_DR.pdf)  |
| P: Dimensionality Reduction, part 1           |  [![Analysis_1](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/6_Analysis_part1.ipynb)|
| P: Dimensionality Reduction, part 2           | [![Analysis_2](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/6_Analysis_DR/6_Analysis_part2.ipynb)|
| L7: Clustering   | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/7_Analysis_clustering/Lecture_7_Clustering.pdf)|
| P: Clustering   | [![Analysis_3](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/7_Analysis_clustering/7_clustering.ipynb) |
| L8: Data Classification    | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/8_Analysis_classification/Lecture_8_classification.pdf) | 
| P: Data Classification  | [![Analysis_4](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/8_Analysis_classification/1_classification.ipynb) |
| L9: Markov State Modelling  | [Lecture Slides](https://github.com/CCPBioSim/Into_to_MD_simulation_and_analysis/blob/main/9_Analysis_MSM/Lecture_9_MSM.pdf) |


# Assessment and feedback

Each Jupyter notebook contains information on a specific topic, as well as task the student is asked to carry out independently. The tasks range from interpreting data previously produced, to running presented code with different parameters, to solving a specific problem by implementing a short Python code. Solutions to all questions are provided in the notebook as drop-down cells.

In our own teaching practice, we provide students with post-its of two different colours that can be displayed on their computer screen --- yellow indicating that everything is clear, pink indicating that help is required. At the end of each practical session, studends are asked to use these same post-its to provide instructors with feedback on something they liked (yellow post-it), and something that requires improvement (pink post-it). In the three years we have delivered this course, this appoach has enabled us to gather comprehensive feedback, helping us fine-tuning the teaching material and our own delivery style. A key observation is that students, when presented with a new notebook, especially appreciate the instructors spending few minutes describing the overall notebook structure and the tasks it features, before working through the beginning of it.


# Conclusion

Thanks to the increasing availability of computational power and software automating many of the processes associated with biomolecular simulation and analysis, the palette of questions addressable with MD is broadening. While this is positive, it is still crucial that the computational scientist has a clear understanding of what is being simulated, and how. Indeed, to date many decisions associated with system building and analysis cannot be delegated to a machine without human verification. In this context, we see our course as a first stepping-stone, detailing the key decisions that need to be made, providing examples of how this can be done in practice, and signposting relevant software and specialised analysis techniques for further education.

Despite its long history, MD is still an evolving field. New techniques pushing the boundary of what is possible keep emerging, as exemplified by the current revolution constituted by the advent of modern machine learning techniques. While we expect that majority of the concepts presented in this course will be valid for many years to come, we are endeavouring to keeping the course material up-to-date by highlighting current methodological trends. For instance, in the most recent interation presented in this publication a discussion on how models produced by AlphaFold should be interpreted and used is introduced.


# Contributions to the course

MTD, MM, and ASJSM conceived the course.

# Acknowledgements 

Part of the material in this course was adapted from other sources with the agreement of respective authors. In this context, we would like to acknowledge Matt Thompson, Jeff Wagner, and Josh Mitchell for the material featured in the OpenFF tutorials, César Ramírez-Sarmiento and collaborators for material featured in the Autodock tutorial, and Ifan Alibay and Richard Gowers for material in the MDAnalysis tutorial. We also wish to acknowledge Charlie Laughton for inspiration on discussing RMSD in conjunction with equilibration, and Rohan Gorantla for help with with setting up Colab environments.

# References
