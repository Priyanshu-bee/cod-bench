m# cod-bench
We present cod-bench containing 11 operators and 8 datasets.
# data
The datasets used for benchmarking can be downloaded from here.
https://drive.google.com/drive/folders/1HZ-fHYBVSPHBdl7Lf8wxbuBdh2ilL0dY?usp=share_link


The codebase contains 4 major modules.
1. Loader Modules: Provides functionality of turning datasets to PyTorch DataLoaders.
2. Operator Modules: Contains Implementation of all models benchamrked in the paper in fully functional form using PyTorch Framework.
3. Utility Modules: Helper functions providing utilities such as transforms, loss functions, optimizers etc.
4. Trainer Module: Provides a common interface for training and testing any pair of model, dataset.

Loader Modules:

1. dataloader.py:
   Provides the functionality of processing the raw dataset provided and split it into pytorch tensors of train, validation and test set.
   eg.
PATH = 'data/Biaxial_N70000_D28.npz'

2. loader_1d.py, loader_2d.py:
   Provides the tool to convert the pytorch tensors of data into Pytorch dataloader that can be directly used in the traning process.
   eg.

3. loader_gnot.py:
   GNOT combines all data in the form of a graph before training phase. This module allows to create the graph dataloader for all datasets    for use with the GNOT model.
