# Doc
## 概述
- 掌控公式里可操作的对象是一个数据流
- 您可以创建一个公式指标，使用公式A+A*2 等方式得到你想要的新的数据流
- 数据流的描述方式是A[index]，代表在当前index下A的值，可以缩写成A
- 您可以用A[index-1]的方式获取上一个数据的值

## FUNCTION
###### daily
	daily([8])是一个 transition 指标，他会在每天0:00:00值为1
###### hour
	hour([8]) 会返回当前index下的小时
###### minute
	minute() 会返回当前index下的分钟
###### match
	match (1,A[1..index]) 会返回指标 A 在当前 index 前上一个值为 1 的 index
###### sum
	sum (B[match (1,A[1..index])..index]) 会返回 从指标A上一个值为1的位置开始到当前的累积求和
	
## API
###### Auth

###### 创建指标

## Component
### Mobile
###### 文本
###### 指标
###### 指标（小）

## 数据接入 & 设备参考设计

###### 注意
- 新手指引： [起步走 - 接入传感器数据](www.zhangkong365.com) 

### 概念

掌控可以接入任何符合传输协议的时序数据，他可以是由传感器获得的实时状态数据，也可以是设备工作的过程数据。


###### 指标（Indicator）
- 物联网的数据接入概念
- 指标的格式定义(Float)
- 指标是唯一的
- 指标ID的生成是通过掌控来完成
- 可以通过 [API](www.zhangkong365.com) 来自动创建指标
