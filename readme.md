
## 项目背景
https://www.kaggle.com/competitions/home-credit-default-risk/overview  
捷信公司在2018年举办的数据竞赛  
在用户发起一笔贷款申请的时候，违约率预测模型是自动化审批中的重要一环。对于违约概率高的用户，拒绝其申请或进入人工审核

## 预测目标
二分类问题，预测用户是否违约，逾期定义为在一定天数内逾期一定天数  
模型评价指标为AUC，只要求预测结果在测试集中的排序型

## 数据特征

### 特征概述
用户基本信息+征信机构提供的历史信用数据+用户在捷信的历史信用数据

### 数据文件
![alt text](data_files.png)
#### application_{train|test}.csv
训练/测试样本，包含申请用户的基本信息+当比贷款信息  
一行=一笔贷款

#### bureau.csv
第三方征信机构提供，用户在其他金融机构的信用数据  
一笔贷款可能有多条记录

#### bureau_balance.csv
第三方征信机构提供，用户每笔历史贷款(消费贷、信用贷)的月末还款状态
一行=一笔历史贷款+一个观察月

#### POS_CASH_balance.csv
#### credit_card_balance.csv
自有数据，历史消费贷、现金贷、信用卡的每月还款情况  
一行=一笔历史贷款+一个观察月

#### installments_payments.csv
自有数据，历史分期记录  
一行=一次分期还款
#### previous_application.csv
自有数据，用户的历史申请记录  
一行=一次申请

#### HomeCredit_columns_description.csv
所有特征的文字描述

### 我们的目标
#### 描述性统计
#### 特征工程
#### 数据建模
#### 模型部署

### 讨论区链接
https://www.kaggle.com/competitions/home-credit-default-risk/discussion/57175