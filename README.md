# Deteksi Pneumonia dari Rontgen (CNN)

CNN sederhana dari nol (PyTorch) untuk mengklasifikasi foto rontgen dada menjadi `NORMAL` atau `PNEUMONIA`.

## Install

```bash
pip install torch torchvision scikit-learn jupyter
```

## Download dataset

Dataset: [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) dari Kaggle (~1,2 GB).

```bash
mkdir -p data
curl -L -o data/chest-xray.zip https://www.kaggle.com/api/v1/datasets/download/paultimothymooney/chest-xray-pneumonia
cd data
unzip chest-xray.zip
cd ..
```

Kalau `curl` gagal, download manual dari link Kaggle di atas, lalu ekstrak ke folder `data/`.

Struktur akhirnya:

```
data/
└── chest_xray/
    ├── train/
    ├── val/
    └── test/
```

## Jalankan

Buka `pneumonia_cnn.ipynb`, lalu jalankan semua cell.
