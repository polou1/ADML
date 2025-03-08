## Requirements
- python 3.8.13
- torch 1.8.0
- torchvision 0.9.0
- scikit-learn 1.2.2
- POT 0.9.3

# Prepare Datasets
Put SYSU-MM01 and RegDB dataset into data/sysu and data/regdb, run prepare\_sysu.py and prepare\_regdb.py to prepare the training data (convert to market1501 format).

## Dataset Preprocessing
```shell
python prepare_sysu.py   # for SYSU-MM01
python prepare_regdb.py  # for RegDB
```
You need to change the dataset path to your own path in the `prepare_sysu.py` and `prepare_regdb.py`.


## Training
```shell
sh run_train_sysu.sh     # for SYSU-MM01
sh run_train_regdb.sh    # for RegDB
```
## Testing
```shell
sh test_sysu.sh          # for SYSU-MM01
sh test_regdb.sh         # for RegDB
```
