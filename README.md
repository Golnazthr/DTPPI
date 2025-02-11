# DTPPI

Drug interactions prediction using a weighted drug-protein network

# Project Structure

The primary files used for this research can be found in the root directory of this project. `networks.ipynb` is used to construct the weighted DTPPI network and calculates the network specific features. The weights for this network are created in `text_embeddings.ipynb`.
The main file, `predictor.ipynb` is used to run the various comparisons between network, traditional and combined features using an MLP.

Next to the jupyter notebook files there are data, embeddings and networks directories. The `/data` directory contains DDI, DPI, negative_fileted and PPI data used to in the construction of the DTPPI network and MLP comparisons. The actual constructed network is saved in `/networks`. The embeddings used to weight the network are found in `/embeddings`

# How to run

To run this project python 3.9 is required to be installed on your local machine, newer versions can possibly not be supported. Create a
venv by running:

```
python3.9 -m venv .venv
```

Activate the virtual environment by running

```
source .venv/bin/activate
```

And install the dependencies found in requirements.txt

```
pip install -r requirements.txt
```
