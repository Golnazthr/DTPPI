# DTPPI

Drug interactions prediction using a weighted drug-protein network

# Project Structure

The primary files used for this research can be found in the root directory of this project. `networks.ipynb` constructs the weighted DTPPI network and calculates the network-specific features. The weights for this network are created in `text_embeddings.ipynb`.

The main file, `predictor.ipynb`, runs various comparisons between network, traditional, and combined features using an MLP.

There are data, embeddings, and network directories next to the Jupyter Notebook files. The `/data` directory contains DDI, DPI, negative_fileted and PPI data used to construct the DTPPI network and MLP comparisons. The actual constructed network is saved in `/networks`. The embeddings used to weight the network are found in `/embeddings`.

# How to run

To run this project python 3.9 is required to be installed on your local machine, newer versions can possibly not be supported. Create a
venv by running:
```
python3.9 -m venv .venv
```
Activate the virtual environment by running:
```
source .venv/bin/activate
```
And install the dependencies found in requirements.txt:
```
pip install -r requirements.txt
```
