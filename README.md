<p align="center">
  <img width="50%" src="https://github.com/tmscarla/improving-transfer-learning/blob/master/img/logo_polimi_harvard.png">
</p>
<br>

# Improving Domain-specific Transfer Learning for Image Recognition and Differential Equations

This repository contains my Master's thesis in Computer Engineering at **[Politecnico di Milano](https://polimi.it)**, developed in collaboration with the **[Institute of Applied and Computational Science](https://iacs.seas.harvard.edu)** at Harvard University.


## Context and problem statement
In recent years, deep neural networks have become an indispensable tool for a wide range of applications, on which they have achieved extremely high predictive accuracy. A considerable huge amount of data is a fundamental, necessary condition for training deep learning architectures, since is in their nature to be extremely *data hungry* models. An approach that helps overcoming the problem of computational cost is **transfer learning**, that consists of leveraging the knowledge acquired by a model, trained on a source task, to solve a target task, saving time and energy.  


## Proposed solution
This thesis explores the field of transfer learning in two very different scenarios: image recognition and resolution of differential equations. In both cases, we investigated previous research works in the literature, trying to improve and extend proposed techniques on one hand, and developing new ideas and new approaches on the other.

### Image recognition
In the image recognition task, which is a supervised learning scenario, we focus on the problem of data impact in a transfer learning setting. In this scenario, we developed different criteria to select a subsample (i.e. perform a data selection) of the target dataset, in order to train in a smarter and faster way. We tested the different criteria on a variety of combinations of datasets, distortions and models, finding that results are poorly generalizable.

<p align="center">
  <img width="60%" src="https://github.com/tmscarla/improving-transfer-learning/blob/master/img/embedding_shift.png">
</p>

### Differential equations
In the scenario of resolution of differential equations, instead, we have no actual data, hence we focused on the problem of the perturbation of the initial conditions and the parameters of the equations, investigating how transfer learning helps with this particular type of distortions, and proposing new network architectures. We show how transfer learning accelerates the resolution of several systems of differential equations and that it becomes even more helpful with our modifications to the source-trained network.

<p align="center">
  <img width="60%" src="https://github.com/tmscarla/improving-transfer-learning/blob/master/img/nn_architecture.png">
</p>

## Thesis structure
The structure of the thesis is organized as follows:
 * **Background:** defines and explains the background knowledge and concepts on which this thesis is based on.
 * **Related Work:** provides an overview of other studies in the literature that addressed the same problem that we have covered.
 * **Methodology:** explains the methodology we followed in our research, describing each step in details.
 * **Implementation:** describes the major technologies, libraries and tools we employed, along with deployment strategies.
 * **Experiments:** is devoted to show the outcomes of the experiments performed to validate our approaches.
 * **Conclusion:** wraps up the discussion with concluding remarks and advises possible future works to be carried on.
 
 
## Repository overview
In this repository, in the root level, you can find the pdf version of the thesis, the Power Point final presentation and two different folders which gather the code for the image recognition and the differential equations scenario. More specifically:
* /image-recognition
  * data: contains all the images of the different datasets used in our experiments
  * *constants.py*: contains all the constants used in the whole project
  * *datasets.py*: download datasets (if not present in the data folder) and split them into train/validation
* /differential-equations
  * *constants.py*: contains all the constants used in the whole project


## Collaborators
* **[Tommaso Scarlatti](https://github.com/tmscarla)**
