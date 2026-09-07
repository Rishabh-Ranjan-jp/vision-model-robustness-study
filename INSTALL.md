Installation Guide
For CPU (Mac / Windows / Linux)
1. Create and activate the environment
conda create -y -n majorProject python=3.10
conda activate majorProject

2. Install CPU-optimized PyTorch
conda install -y -c pytorch pytorch torchvision cpuonly

3. Install core libraries
conda install -y -c conda-forge \
    jupyterlab \
    ipykernel \
    numpy \
    pandas \
    matplotlib \
    scikit-learn \
    scikit-image \
    lime \
    tqdm \
    streamlit \
    optuna

4. Register the Jupyter kernel
python -m ipykernel install \
    --user \
    --name majorProject \
    --display-name "Python (majorProject - CPU)"

5. Launch JupyterLab
jupyter lab

For NVIDIA GPU
1. Create and activate the environment
conda create -y -n majorProject python=3.10
conda activate majorProject

2. Install dependencies

Make sure requirements.txt is present in the project directory, then run:

pip install -r requirements.txt

3. Launch JupyterLab
jupyter lab
