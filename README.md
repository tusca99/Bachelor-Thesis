# 'Studio della superficie potenziale della molecola d’acqua tramite machine learning' Data Repository

Welcome to the data repository for Tuscano Alessio's Bachelor Thesis, titled 'Studio della superficie potenziale della molecola d’acqua tramite machine learning'. 
This repository hosts all the data used and generated during the research conducted for the thesis.

## Overview

The research focuses on developing a neural network capable of predicting the properties that can be calculated by a DFT driven simulation such as the one in 'pw.x' code from quantum-espresso.
For more details see the bachelor thesis document.

## Contents

The repository is organized as follows:

- **[water_dnn/model_graphs_[scenario]]**: folders for predictions with various scenario
  - Under these folders you can find graphs for multiple neural networks predictions: every image is named with the primary hyperparameters that has been changed during the development of the final neural network, so it is easy to refer to the corresponding saved model.
- **[water_dnn/model_plots]**: folder where a given model loss function plot can be found.
- **[water_dnn/saved_model]**: folder where the developed trained models are saved in '.keras' format
  - These models use the same naming scheme that is used for their corresponding graphs and plots for ease of retrieval.
- **[water_dnn/saved_dataset]**: folder where all generated datasets are stored
  - all datasets are stored with less rigid naming. Be aware of that.
  - note: 'Picle_dataset_merge.ipynb' is a macro that has been used to merge similar smaller datasets in a larger one with the possibility of filtering during the merge.
- **[water_dnn/water_dnn.ipynb]**: neural network training and test notebook.
- **[water_dnn/pwbase_workflow_datasetcreation_aiida.ipynb]**: simulation and dataset creation notebook



## Usage

All the jupyter notebooks are written in python.
To use the simulation code you need Aiida with aiida-quantumespresso connected to a functioning pw.x code, plus some other libraries mentid in the code.
To use the neural network code you need Tensorflow with Keras.

## Citation

If you use any data from this repository in your own research or projects, please cite the following repository and/or the relative paper.
## License

This repository is licensed under the GNU GPLv3 license.

## Contact

If you have any questions, feedback, or issues regarding the data in this repository, please feel free to contact:

- Alessio Tuscano: alessio@tuscano.it

## Acknowledgments

All the papers and libraries used can be found within the bibliografy of the Thesis.
