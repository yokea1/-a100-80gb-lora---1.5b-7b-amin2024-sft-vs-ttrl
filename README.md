# -a100-80gb-lora---1.5b-7b-aime2024-sft-vs-ttrl
1.背景介绍；大三学生 软件专业 集群显卡node没有nvlink 禁止p2p 走cpu通信发现双卡很慢 果断放弃走单卡复线小模型千问-math-1.5b&amp;7b 后续会双卡到7b model上
2.测试对象：aime2024（30 row） 开源模型：千问-math-2.5-1.5b&7b
3.目前结果：sft1.5b&7b结果 &TTRL 通线打通 
4.目前问题：多卡node nvlink没有 使用单卡 超参调低 单卡 a100 80step=42epoches（后续奖励函数好了 会上到80epoches）  lora 跑 TTRL通线没问题 针对于1.5b的奖励函数问题🙋 整体复现70%左右
