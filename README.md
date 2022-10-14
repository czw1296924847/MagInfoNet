[![DOI](https://zenodo.org/badge/483172829.svg)](https://zenodo.org/badge/latestdoi/483172829)
# MagInfoNet
MagInfoNet is a Neural Network model used to estimate earthquake magnitudes. <br>
Compared with traditional Machine Learning and previous Deep Learning models, MagInfoNet combines seismic signals with relevant information to improve the prediction accuracy. <br>
The paper is available in 

## Installation
MagInfoNet is based on [Pytorch](https://pytorch.org/docs/stable/index.html) and [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/index.html)<br>
Firstly please create a virtual environment for yourself<br>
`conda create -n your-env-name python=3.9`<br><br>
Then, there are some Python packages need to be installed<br>
`conda install pytorch torchvision torchaudio cudatoolkit=11.3`<br>
`conda install pyg -c pyg`<br>
`conda install matplotlib`<br>
`conda install h5py==2.10.0`<br>

## Dataset Preparation
The Dataset used in our paper can be downloaded from [https://github.com/smousavi05/STEAD](https://github.com/smousavi05/STEAD). Before running, you should donwload and  store the data file in the folder [dataset](https://github.com/czw1296924847/MagInfoNet/tree/main/dataset) like<br>

![image](https://github.com/czw1296924847/MagInfoNet/blob/main/dataset_structure.png)

## Program Description
### Training and Testing Models
After the preparation of Dataset, you can run the programs in the foloder [run](https://github.com/czw1296924847/MagInfoNet/tree/main/run) to test the performance : <br>
`python run_MagInfoNet.py`

<!---
### Anti-Interfernce
You can testing the anti-interfernce abilities of these models by using:<br>
`python anti_interference.py`

### Explain layers
You can compare the role of RM by using:<br>
`python load_to_extract.py`

### Plotting Images
Aftering training and testing steps, you can plot the results in different ways as follows in the folder [](): <br>
`python plot_result.py`: the distribution of magnitudes; the true magnitudes and the predicted magnitudes on the plane map;
-->
