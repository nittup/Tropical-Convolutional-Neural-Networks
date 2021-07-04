# Traditional-Convolutional-Neural-Networks
 Traditional Convolutional Neural Networks

An Alternative Practice of Tropical Convolution to Traditional Convolutional Neural Networks
的实现代码；
---------------------------------------------------------------------------------------------------------------------------
运行环境：
python 3.6.5 + pytorch 1.7.0；
import numpy as np
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
import warnings
warnings.filterwarnings('ignore')
from tqdm import tqdm, trange
import time
import sys
import os
import math
import gzip
---------------------------------------------------------------------------------------------------------------------------

运行参数参考options_func，并注意在load_data中需要添加你需要的数据集及其存放的位置；

运行示例：
python .\Traditional_Convolutional_Neural_Networks.py --net net0

---------------------------------------------------------------------------------------------------------------------------

代码中包括
1、6种tropical convolution layers：
MinPlus-Sum_Conv Layer (MinP-S)
MaxPlus-Sum-Conv Layer (MaxP-S)
MinPlus-Max-Conv Layer (MinP-Max)
MaxPlus-Min-Conv Layer (MaxP-Min)
MinPlus-Min-Conv Layer (MinP-Min)
MaxPlus-Max-Conv Layer (MaxP-Max)
详见论文；

2、6中网络结构
详见论文；

