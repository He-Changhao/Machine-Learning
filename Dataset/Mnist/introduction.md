# Orig.mat - Complete MNIST Dataset
## Contains 70000 samples.
## Variables: 'fea' and 'gnd'.
## Each row of 'fea' is a sample, and 'gnd' is the corresponding label.

# 2k2k.mat - Subset of MNIST Dataset
## Contains 4000 samples drawn from the MNIST dataset.
## Variables: 'fea', 'gnd', 'trainIdx', and 'testIdx'.
## Each row of 'fea' is a sample, and 'gnd' is the corresponding label.
## 'trainIdx' and 'testIdx' contain 2000 sample labels each.

# Python Code to Load Orig.mat

from scipy.io import loadmat
MNIST = loadmat('Orig.mat')
fea = MNIST['fea']  # Samples
gnd = MNIST['gnd']  # Labels

# Python Code to Load 2k2k.mat

from scipy.io import loadmat
_2k2k = loadmat('2k2k.mat')
trainIdx = _2k2k['trainIdx'].ravel() - 1
testIdx = _2k2k['testIdx'].ravel() - 1
train_data = _2k2k['fea'][trainIdx]
train_index = _2k2k['gnd'][trainIdx]
test_data = _2k2k['fea'][testIdx]
test_index = _2k2k['gnd'][testIdx]
