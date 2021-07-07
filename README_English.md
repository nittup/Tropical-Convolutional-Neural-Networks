Traditional-Convolutional-Neural-Networks
-----------------------------------------------------------------------------------------------------------------------------------------------
Traditional Convolutional Neural Networks ICCDA2021-An Alternative Practice of Tropical Convolution to Traditional Convolutional Neural Networks https://ui.adsabs.harvard.edu/abs/2021arXiv210302096F/abstract

Operating environment
-----------------------------------------------------------------------------------------------------------------------------------------------
python 3.6.5 + pytorch 1.7.0； // import numpy as np

import torch

from torch import optim, nn

from torch.nn import init

import torch.nn.functional as F

from torch.utils.data import TensorDataset, DataLoader

from torch.utils.tensorboard import SummaryWriter

from torch.autograd import Variable

from torch.nn.parameter import Parameter

from torchsummary import summary

from torchvision import transforms, datasets

from sklearn.metrics import accuracy_score

from matplotlib import pyplot as plt

from optparse import OptionParser

from matplotlib import pyplot

from collections import OrderedDict

import warnings warnings.filterwarnings('ignore')

Set parm:
-----------------------------------------------------------------------------------------------------------------------------------------------
You can refer to options_func to set your parm，and you should add your own path of your dataset in the code.
Running case ： python .\Traditional_Convolutional_Neural_Networks.py --net net0

-----------------------------------------------------------------------------------------------------------------------------------------------

The code incudes

1.  6 types of tropical convolutional layers：

MinPlus-Sum_Conv Layer (MinP-S)

MaxPlus-Sum-Conv Layer (MaxP-S)

MinPlus-Max-Conv Layer (MinP-Max)

MaxPlus-Min-Conv Layer (MaxP-Min)

MinPlus-Min-Conv Layer (MinP-Min)

MaxPlus-Max-Conv Layer (MaxP-Max)

See the paper for details.

2、 Several TCNNs

![image](https://user-images.githubusercontent.com/86921131/124767651-94beed00-df6a-11eb-8748-63f7a62282ee.png)


See the paper for details.