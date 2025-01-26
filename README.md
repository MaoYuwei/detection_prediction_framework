# A deep learning framework for layer-wise porosity prediction
This repository contains the code for A deep learning framework for layer-wise porosity prediction in metal powder bed fusion using thermal signatures. The code provides the following functions:

- detection module to detect porosity using thermal signatures
- prediction module to predict future layer's porosity using previous layers' history information.

## Installation Requirements
The basic requirement for using the files is a Python 3.8.19 environment with PyTorch 2.3.0

## Source Files
Here is a brief description of the files and folder content:

- detection_module.py: to detect porosity labels using thermal signatures.
- prediction_module.py: to predict future layer's porosity labels using previous layers' history information.

## Running the code
To generate the dataset, run detection_module.py file to detect porosity labels first. Next, run prediction_module.py to predict future layer's porosity labels using previous layers' history information.

## Developer Team
The code was developed by Yuwei Mao from the [CUCIS](http://cucis.ece.northwestern.edu/) group at the Electrical and Computer Engineering Department at Northwestern University.

## Publication
1. Mao, Yuwei, Hui Lin, Christina Xuan Yu, Roger Frye, Darren Beckett, Kevin Anderson, Lars Jacquemetton et al. "A deep learning framework for layer-wise porosity prediction in metal powder bed fusion using thermal signatures." Journal of Intelligent Manufacturing 34, no. 1 (2023): 315-329. [PDF](https://link.springer.com/article/10.1007/s10845-022-02039-3)

## Disclaimer
The research code shared in this repository is shared without any support or guarantee on its quality. However, please do raise an issue if you find anything wrong and I will try my best to address it.

email: yuweimao2019@u.northwestern.edu

Copyright (C) 2023, Northwestern University.

See COPYRIGHT notice in top-level directory.

## Funding Support
This work was primarily supported by the following financial assistance award 70NANB19H005 from U.S. Department of Commerce, National Institute of Standards and Technology as part of the Center for Hierarchical Materials Design (CHiMaD). Partial support from Predictive Science and Engineering Design Cluster (PS &ED, Northwestern University); DOE awards DE-SC0019358, DE-SC0021399; and NSF award CMMI-2053929 is also acknowledged.








# Porosity_prediction

First use detection module to get detected labels, then use prediction module to predict the next layer labels.

The example input data is test.npy file, where have 15 layers. Using the first 6 layers, the framework can predict the next layer labels, i.e. 7-th layer. Then, the 8-th layer can be predicted using the information of 2-7 layers.

