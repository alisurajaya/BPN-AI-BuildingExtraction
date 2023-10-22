## Ekstraksi Tapak Bangunan menggunakan model M-VT
Repositori ini berisi prosedur ekstraksi tapak bangunan pada data orthophoto menggunakan model Modified Vision Transformer (M-VT) yang dikembangkan oleh Tim Peneliti Departemen Teknik Geodesi UGM dalam rangka Pilot Project BPN-AI Kementerian ATR/BPN RI.

Prosedur lengkap dapat dilihat pada file Prosedur-Ekstraksi-Tapak-Bangunan-MVT.ipynb (Jupyter Notebook).


## Installation

```
git clone https://github.com/s1m0nS/mapAI-regularization.git
cd mapAI-regularization
conda create --name mapai python=3.10
conda activate mapai
pip install -r requirements.txt
```
Installing GDAL inside a conda environment can be tricky. Follow the steps below according to your OS.

**Linux:**

```
sudo apt-get update && sudo apt upgrade -y && sudo apt autoremove 
sudo apt-get install -y cdo nco gdal-bin libgdal-dev-
python -m pip install --upgrade pip setuptools wheel
python -m pip install --upgrade gdal
conda install -c conda forge libgdal
conda install -c conda-forge libgdal
conda install -c conda-forge gdal
conda install tiledb=2.2
conda install poppler
```

**Windows:**

Get the appropriate .whl file for your Python version from: https://www.lfd.uci.edu/~gohlke/pythonlibs/#gdal
For Python 3.10 use either: 
- GDAL‑3.4.3‑cp310‑cp310‑win_amd64.whl or
- GDAL‑3.4.3‑cp310‑cp310‑win32.whl.

then install the appropriate one as:
```
conda activate mapai
python -m pip install C:\Users\...\GDAL‑3.4.3‑cp310‑cp310‑win_amd64.whl
```

Run our Jupyter Notebooks and enjoy the process. If you encounter errors post an issue.

Feedback and new ideas are welcome.



