# 使用 Cloudformation 部署多层架构

## 目录
- [目的](#目的)
- []
在这个系列中, 我们通过部署一套电视节目推荐系统, 来学习如何使用 [AWS Cloudformation](https://aws.amazon.com/cloudformation/) 配置和部署可靠且低耦合的架构 (本文的全部时间内容来自 [AWS Well-architected Labs](https://wellarchitectedlabs.com/) )

## 目的
我们将通过两个 AWS Cloudformation 模板, 部署一套可靠的多层 AWS 云端架构. 其中一个模板是用来部署一个 Amazon VPC, 另一个模板是用来部署一个搭建在跨 AZ(Available Zone) 的多 EC2 实例的三层 web 服务器:



在完成本文阅读和时间后, 我们将能够:
* 掌握如何自动化部署基础设施
* 理解自动化部署如何保证架构稳定


## 前提准备
在开始部署之前, 我们需要保证我们有足够的 AWS 权限来部署