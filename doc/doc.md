# Doc
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

## DATA ACCESS

###### Application layer protocol

	{"hello":world}
	
###### MQTT
iothub.thingworks.cn:1883
	
## Component
### Mobile
###### 文本
###### 指标
###### 指标（小）

## Device Ref Design & tools

###### 注意
- 新手指引： [起步走 - 接入传感器数据](www.zhangkong365.com) 
- 上报格式协议请参考 [DOC - DATA ACCESS](www.zhangkong365.com) 


### 概念

###### 指标（Indicator）
- 物联网的数据接入概念
- 指标的格式定义(Float)
- 指标是唯一的
- 指标ID的生成是通过掌控来完成
- 可以通过 [API](www.zhangkong365.com) 来自动创建指标

### 参考设计

###### 设备部署
- 设备部署的时候需要对指标进行命名

###### 安全
password

###### 连接

### 安装引导
