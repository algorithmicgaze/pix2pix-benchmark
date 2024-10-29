# pix2pix benchmarks

This repository tests a number of approaches to get the best results from pix2pix.

To ensure reproducibility, the random seeds for Python, numpy and PyTorch are "locked". We also do our best to set determistic behavior for layers like Dropout, as well as for DataLoaders that run on multiple CPUs. That should mean that running the same code twice should have the exact same results.

You need a dataset to run on. If you want you can use the faces dataset provided here:

<https://algorithmicgaze.s3.amazonaws.com/datasets/faces_contour.zip>

## Training On Your Own Machine

The `train_vanilla.ipynb` notebook runs in Jupyter Notebook. Here's some setup to do first:

In the terminal, clone the repository:

```bash
git clone https://github.com/algorithmicgaze/pix2pix-benchmark.git
cd pix2pix-benchmarks
```

Install the required Python packages:

```bash
pip install tqdm matplotlib
```

Run Jupyter notebook:

```bash
jupyter notebook
```

Open the `train_vanilla.ipynb` notebook and follow the instructions.

## Training on Runpod

1. Create a Pod with PyTorch 2.4
2. Connect to Jupyter Lab
3. Open a terminal
4. Clone the repository:

    ```bash
    git clone https://github.com/algorithmicgaze/pix2pix-benchmarks.git
    cd pix2pix-benchmarks
    ```

5. Install dependencies:

    ```bash
    apt update && apt install -y unzip
    pip install tqdm matplotlib
    ```
