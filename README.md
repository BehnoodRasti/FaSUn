# FaSUn
Fast Semisupervised Unmixing (FaSUn) is an innovative semi-supervised unmixing technique that leverages the assumption that real endmembers can be represented as convex combinations of the library endmembers. Building upon the principles of archetypal analysis, we propose a new model formulation for sparse unmixing. The motivation behind this method is to address mismatches commonly encountered between endmembers from spectral libraries and endmembers from a dataset, which often manifest as scaling factors. These mismatches can arise from various sources such as noise, atmospheric effects, illumination variations, and the intrinsic variability of materials. In contrast to conventional sparse unmixing methods, SUnAA estimates both the endmembers and abundances by utilizing the endmember library as a reference.

## Citation
If you use this code please cite the following paper

B. Rasti, A. Zouaoui, J. Mairal and J. Chanussot, "SUnAA: Sparse Unmixing using Archetypal Analysis," in IEEE Geoscience and Remote Sensing Letters, doi: 10.1109/LGRS.2023.3284221.

## Installation instructions

1. Clone the repository and move to the repository

```shell
git clone git@github.com:BehnoodRasti/FaSUn.git
cd FaSUn
```

2. We recommend using `conda` to install the package, as follows:

```shell
conda create --name FaSUn python=3.10
```
3. Activate your freshly created environment
```shell
conda activate FaSUn
```

4. Install the required python packages:
```shell
pip install -r requirements.txt
```

## Running the demo

We provide a simple demo script alongside the data to run it (DC1 in our paper).

You can run it at the desired SNR (here 20) using the following command:

```shell
python demo.py -N 40 -r 1 -p 5 -m1 50 -m2 10 -T 5000 -T1 5 -T2 5
```

Take a look at the `demo.py` file to better understand the parameters that can be tweaked as well as changing the dataset to fit your needs.
