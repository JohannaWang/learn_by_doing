# learn_by_doing

2019/6/26
learn_by_doing_daily_work

Introduction time series with R, 结构是why model, synthetic data, model and plotting 

1. main feature and variation, season

2.variable is measured sequentially in time over or at a fixed interval(sampling ingterval) -- time series data

discrete-time stochastic process

trend, season, correlated (serially dependent)


2019/6/28
https://pypi.org/project/dtaidistance/



2019/10/4


2020/1/22 how time flies! 

Kaggle: web traffic prediction学习第一名的解题思路：
## 关键词：
trend continue.. (auto-regression model)
spike, gradullay decay (moving average model)
spike on the holidays (seasonal model)

## Feature Engeneering :
target: web traffic or hit, log(web traffic+1)
day of week, year-to-year/quarter-to-quarter autocorrelation, 其他one-hot feature 

## Mode: 
CRU + attention 

## how to handle long time series 
day365 = day-365 autocorrelation 
day90= day-90 autocorrelation 

atten365 = 0.25* day_364 + 0.5* day_365 + 0.25* day_366 (平滑)

## 目标函数(losses and regularization)
mape在零点不可导，用其他的方法定义一个优化目标函数，或者对log(raw data+1)按照mae来优化

## training and validation 
1) walk forward split
2) side by side split 

## ensemble 
1) 从某一个model step开始，记录10个check point 
2) 3 model with different seed
3) average SGD

## 超参
调参的package, feature比model architecture重要

## 优化器
gradient clipping, learning rate auto adjust 


2020/9/2
激活函数：https://www.jianshu.com/p/857d5859d2cc  










