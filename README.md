# Pneumonia Detection from Chest X-Rays (CNN)

A simple CNN built from scratch in PyTorch that classifies chest X-ray images as `NORMAL` or `PNEUMONIA`.

## Install

```bash
pip install torch torchvision scikit-learn jupyter
```

## Download the dataset

Dataset: [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) on Kaggle (~1.2 GB).

```bash
mkdir -p data
curl -L -o data/chest-xray.zip https://www.kaggle.com/api/v1/datasets/download/paultimothymooney/chest-xray-pneumonia
cd data
unzip chest-xray.zip
cd ..
```

If `curl` fails, download it manually from the Kaggle link above and extract it into the `data/` folder.

Expected structure:

```
data/
└── chest_xray/
    ├── train/
    ├── val/
    └── test/
```

## Run

Open `pneumonia_cnn.ipynb` and run all cells.
