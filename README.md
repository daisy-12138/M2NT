# Enhancing the Generalization of Facial Forgery Detection via Multi-branch Multi-feature Network

## Introduction

This is the implementation of Enhancing the Generalization of Facial Forgery Detection via Multi-branch Multi-feature Network


## Table of Contents

- [Requirements](#requirements)
- [Dataset](#dataset)
- [Usage](#usage)
  - [Model Training](#model-training)
  - [Model Testing](#model-testing)


## Requirements
<pre>
    * Python 3.x
    * PyTorch
    * numpy
    * torch
    * torchvision
    * tqdm
    * decord
    * dlib
    * opencv
    * face_recognition
    * timm
</pre>

## Dataset
FF++, CelebDF-v1, CelebDF-v2, DFDC, and UADFV datasets can be available at https://github.com/SCLBD/DeepfakeBench.

WildDeepfake dataset can be available at https://github.com/OpenTAI/wild-deepfake.

Diff dataset can be available at https://github.com/OpenTAI/wild-deepfake.

HybirdGenFace dataset can be available at https://pan.baidu.com/s/1zWvf5GpoXJtgRY4Tkup8gQ?pwd=38k5(38k5).

## Usage

1. Clone this repository:

```bash
git clone https://github.com/daisy-12138/M2NT
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Model Training

To train the M2NT model, follow these steps:

1. Prepare the training data according to the following structure and place it in the `sample_train_data` folder:
<pre>
    train:
        - fake
        - real
    valid:
        - fake
        - real
    test:
        - fake
        - real
</pre>
 

2. Run the training script:

```bash
python train.py
```

The model weights and metrics are saved in the `weight` folder.


## Model Testing

To run the code, use the following command:

```bash
python test.py
```
