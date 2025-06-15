
---

````markdown
# 🧠 Deep Learning Projects for Image Classification

This repository contains a collection of deep learning experiments implemented in Python using TensorFlow. The notebooks demonstrate image classification tasks, including digit recognition using MNIST and binary classification of cats vs. dogs using Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (LSTM).

---

## 📁 Included Notebooks

| Notebook | Description |
|----------|-------------|
| `1.ipynb` | MNIST digit classification using a fully connected neural network. |
| `7.ipynb` | MNIST digit classification using an LSTM-based architecture. |
| `2.ipynb` | Image preprocessing and dataset creation for the Cats vs. Dogs dataset. |
| `3.ipynb` | Basic CNN model for cat/dog classification. |
| `5.ipynb` | Model tuning with different combinations of convolutional and dense layers. |
| `6.ipynb` | Image prediction using a trained model and OpenCV. |

---

## ⚙️ Setup Instructions

### 1. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

Download and install Miniconda (Python 3.6 version) for your operating system.

### 2. Create and Activate a Conda Environment

```bash
conda create --name dl-env python=3.6
conda activate dl-env
````

### 3. Install Required Libraries

```bash
pip install tensorflow numpy matplotlib opencv-python pickle-mixin notebook
```

---

## 📦 Downloading MNIST Dataset

The MNIST dataset (images of handwritten digits) is automatically downloaded by TensorFlow when you run:

```python
from tensorflow.keras.datasets import mnist
(x_train, y_train), (x_test, y_test) = mnist.load_data()
```

No manual download is needed.

However, if you face any download issues (e.g., behind a proxy), you can manually fetch it from:

* [Yann LeCun's MNIST page](http://yann.lecun.com/exdb/mnist/)
* Place the four `.gz` files in a local directory, and use `tf.keras.utils.get_file` with a `file://` path to load them manually.

---

## 🐱🐶 Preparing Cats vs. Dogs Dataset

To run `2.ipynb`, place two folders named `Cat/` and `Dog/` in a parent directory (e.g., `Documents/`), each containing the respective images.

Update the `DATADIR` variable:

```python
DATADIR = "/path/to/Documents"
```

You can download the dataset from [Kaggle - Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats/data) (requires Kaggle account).

---

## 📚 Citation

If you use our work in your research, please cite:

1. **Navigating Malignancy: Deep Learning for Mediastinal Lymph Node Classification**
   A. A. Nayan, B. Kijsirikul, and Y. Iwahori, *IEEE Access*, 2024.
   DOI: [10.1109/ACCESS.2024.3491414](https://doi.org/10.1109/ACCESS.2024.3491414)

2. **Mediastinal Lymph Node Detection and Segmentation using Deep Learning**
   A. A. Nayan, B. Kijsirikul, and Y. Iwahori, *IEEE Access*, 2022.
   DOI: [10.1109/ACCESS.2022.3198996](https://doi.org/10.1109/ACCESS.2022.3198996)

3. **A Deep Learning Approach for Brain Tumor Detection using MRI**
   A. A. Nayan et al., *IJECE*, 2023.
   DOI: [10.11591/ijece.v13i1.pp1039-1047](https://doi.org/10.11591/ijece.v13i1.pp1039-1047)

4. **Detection of Objects from Noisy Images**
   A. A. Nayan et al., *IEEE STI*, 2020.
   DOI: [10.1109/STI50764.2020.9350521](https://doi.org/10.1109/STI50764.2020.9350521)
5. **Real Time Multi-Class Object Detection and Recognition Using Vision Augmentation Algorithm**
    A. A. Nayan et. al., *International Journal of Advanced Science and Technology*,2020, (https://doi.org/10.48550/arXiv.2003.07442)
---

## 🎓 Acknowledgments

This research was supported by:

* **Chulalongkorn University’s Graduate Scholarship Program for ASEAN or Non-ASEAN Countries**
* **Japan Society for the Promotion of Science (JSPS) Grant-in-Aid for Scientific Research (C)** under Yuji Iwahori (Grant Number: **20K11873**)

---

## 🤝 Contributions & Contact

Pull requests are welcome. For major changes, please open an issue first to discuss your ideas.
For questions or collaboration, feel free to reach out via GitHub Issues or email: asquiren@gmail.com

---

```
