# Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based Chatbots
This repository contains the source code and datasets for the EMNLP 2019 paper [Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based Chatbots]. <br>


## Dependencies
Python 3.x <br>
Pytorch 1.1.0

## Datasets and Trained Models
Your can download the processed datasets and the checkpoints of trained models for reproduce the experimental results in the paper. <br>
https://www.dropbox.com/sh/18gncqj296swzjg/AABtrQUpBi3JORai8zimNpNCa?dl=0

Unzip the dataset.rar file to the folder of ```dataset``` and unzip the checkpoint.rar file to the folder of ```checkpoint```.


## Train a new model
```
cd ./Dialogue/
python ./run.py --task "ubuntu" --is_training True
python ./run.py --task "douban" --is_training True
python ./run.py --task "alime" --is_training True
```
The training process is recorded in ```log/[ubuntu|douban|alime].msn.log``` file.

## Test a trained model
```
python ./run.py --task "ubuntu"
python ./run.py --task "douban"
python ./run.py --task "douban"
```

