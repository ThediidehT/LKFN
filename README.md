# LKFN
Large Kernel Frequency-enhanced Network for Efficient Single Image Super-Resolution

Jiadi Chen, Chunjiang Duanmu and Huanhuan Long

## Environment

- [PyTorch >= 1.7](https://pytorch.org/) **(Recommend >= 1.11)**
- [BasicSR = 1.4.2](https://github.com/XPixelGroup/BasicSR)

### Installation

```
pip install -r requirements.txt
python setup.py develop
```

## How To Test

- Refer to `./options/test/LKFN` for the configuration file of the model to be tested, and prepare the testing data and pretrained model.
- The pretrained models are available in `./experiments/pretrained_models/LKFN`.
- Then run the follwing codes (taking `LKFN_x4.pth` as an example):

```
python basicsr/test.py -opt options/test/LKFN/test_LKFN_x4.yml
```

The testing results will be saved in the `./results` folder.

## How To Train

- Refer to `./options/train` for the configuration file of the model to train.
- Preparation of training data can refer to [this page](https://github.com/XPixelGroup/BasicSR/blob/master/docs/DatasetPreparation.md).
- The training command is like:

```
python basicsr/train.py -opt options/train/LKFN/train_LKFN_x4.yml
```

More training commands can refer to [this page](https://github.com/XPixelGroup/BasicSR/blob/master/docs/TrainTest.md).

The training logs and weights will be saved in the `./experiments` folder.


## Contact

If you have any question, please email zjnucjd@163.com.
