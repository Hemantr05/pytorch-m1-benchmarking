# PYTORCH-M1 BENCHMARKING


## Setup


1. setup virtual environment

```
$ conda create -n torch-m1 python3.8
$ conda deactivate && conda activate torch-m1
```

2. download pytorch for m1

```
$ pip3 install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cpu
```

3. navigate to model/data type (in this repository)

```
example:

$ cd mnist/
```

## Benchmark

cpu benchmarking:

```
$ python main.py --epoch 1 --device "cpu"
```

apple m1 silicon benchmarking:

```
$ python main.py --epoch 1 --device "mps"
```
