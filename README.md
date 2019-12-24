# Crnn_chinese_characters_rec
chinese characters recognition

## Descriptions in chinese：https://blog.csdn.net/Sierkinhane/article/details/82857572

## (Please update pytorch to 1.1.0 https://pytorch.org/ )
## Update
* remove lmdb dataloader
* fix ctc loss
## Test
* [download model](https://pan.baidu.com/s/13Jk1q94BUZYvSYgPJkDr9Q) password:t99a  
There are images in test_images file, and you just run it as follow.
* python3 test.py

## Train
before traning, you should prepare the dataset of characters.(described in csdn blog)
* python3 preprocessing.py to prepare train.txt and test.txt or [download](https://pan.baidu.com/s/1rd4tm0sCq5fFgB2ziUxcrA) password:w877 
* [modify the path to images, train.txt and test.txt in crnn_main_v2.py](https://github.com/Sierkinhane/crnn_chinese_characters_rec/issues/124#issuecomment-515996489)
* python3 crnn_main_v2.py --cuda


## 3.6 million chinese characters dataset：
![](https://github.com/Sierkinhane/LearningRecords/blob/master/chinese_char.png)

## [Data generator](https://github.com/Sierkinhane/crnn_chinese_characters_rec/tree/master/data_generator):
![](https://github.com/Sierkinhane/crnn_chinese_characters_rec/blob/master/test_images/data_generator.png)

## Results：
![](https://github.com/Sierkinhane/crnn_chinese_characters_rec/blob/master/test_images/1.png)
![](https://github.com/Sierkinhane/crnn_chinese_characters_rec/blob/master/test_images/2.png)

## Training(accuray was 97.7% ultimately):
![](https://github.com/Sierkinhane/crnn_chinese_characters_rec/blob/master/test_images/3.png)
![](https://github.com/Sierkinhane/crnn_chinese_characters_rec/blob/master/test_images/4.png)

##(This repository is based on https://github.com/meijieru/crnn.pytorch)

# If interested in Face detection, you can refer to the other repository:
  MTCNN https://github.com/Sierkinhane/mtcnn-pytorch
  
  results:
  
  ![](https://github.com/Sierkinhane/mtcnn-pytorch/blob/master/results/r_1.jpg)
  ![](https://github.com/Sierkinhane/mtcnn-pytorch/blob/master/results/r_2.jpg)
  ![](https://github.com/Sierkinhane/mtcnn-pytorch/blob/master/results/r_3.jpg)
