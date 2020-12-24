# 使用 Cloudformation 部署多层架构

## 目录


在本文中, 我们来一起学习和动手实践 AWS Cloudformation] (https://aws.amazon.com/cloudformation/). 我们将通过两个 AWS Cloudformation 模板, 部署一套可靠的多层 AWS 云端架构. 其中一个模板是用来部署一个 Amazon VPC, 另一个模板是用来部署一个搭建在跨 AZ(Available Zone) 的多EC2 实例的三层 web 服务器.

## 目的
在完成本文阅读和时间后, 我们将能够:
* 掌握如何自动化部署基础设施
* 理解自动化部署如何保证架构稳定


## 前提准备
在开始我们的动手实验之前, 我们需要保证我们有足够的 AWS 权限来部署