# OBIs-Evolution-of-Chinese-characters
Including the data set created by himself, the content of the data set includes the evolution of 972 groups of oracle bones, from oracle bones to regular script. Using Siamese network to explore the rules of evolution between characters
#######Because the compressed files are too large, I uploaded them separately and put them into folders in the following order:
1. datasets
2.img
3.logs
4.model_data
5.nets
6.utils
7.predicts

### Content implementation
Siamese network is implemented in this warehouse for training character evolution. The backbone network used by the warehouse are VGG16,resnets 50,and alexnet.

### Environment configuration
tensorflow-gpu==2.2.0
keras=2.1.5
### Matters needing attention
**First of all, I conducted experiments with omniglot data set, and trained my data set to use two different formats, so I need to pay attention to the formatting.
**Then, three experiments were compared, and the codes were named respectively

### Prediction steps
#### 1、Use pre-trained weights
Run：predict.py，
Follow the steps to complete the prediction
#### 2、Use your own training weights
a、Follow the training steps.
b、In the siamese.py file, modify model_path to correspond to the trained file in the following sections；**Model_path corresponds to the weight file under the logs folder**。


#### 1、
The our dataset stores data in two levels：
```python
- image_background
	- Ai_01
			- 0000_01.png
			- 0000_02.png
			- ……
	- Bing_03
	- ……
```
The training steps are:
a、Run train.py to start training
#### 2、：
a、Put the dataset in the above format and under the dataset folder in the root directory.
b、Then set train_own_data in train.py to True.
c、 Run train.py to start training.
####  Dowmload Dataset
Link：https://pan.baidu.com/s/1WfQKcGXVe921kOdq_9fV-A 
Password：1640 


