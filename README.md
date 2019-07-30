# NAS
神经架构搜索

#强化学习  <br>
ENAS1802:[paper](https://arxiv.org/abs/1802.03268) <br>
#可微 <br>
DARTS1806:[paper](https://arxiv.org/abs/1806.09055v2),[code](https://github.com/quark0/darts)  <br>

PDARTS1904:[paper](https://arxiv.org/abs/1904.12760),[code](https://github.com/zihaozhang9/pdarts)  <br>

#连续优化 <br>
NAO1804:[paper]https://arxiv.org/abs/1808.07233v4),[code](https://github.com/zihaozhang9/NAO)  <br>

[网络搜索之DARTS, GDAS, DenseNAS, P-DARTS, PC-DARTS](https://mp.weixin.qq.com/s/CqIQuocfVMqLF5vl0cZaDA): <br> 
DARTS [1]：第一个能work的 end2end 基于梯度反传的 NAS 框架，当然你也可选择ENAS（重点是开源了，而且代码写得易懂，后面几个文章都是基于这个做的）。 <br> 
GDAS [2]：百度出品，提出了可微的operation sampler，故每次只需优化采样到的部分子图，故特点就是一个字：快 （4 GPU hours）。  <br>
DenseNAS [3]：地平线出品，提出了可以同时搜 block的宽度和空间分辨率的可微分NAS，story讲得还行，实验部分有点虚。  <br>
P-DARTS [4]：华为出品，致力于解决在proxy训练与target测试的模型depth gap问题，参考李飞飞 PNAS 的思路用在block间。  <br>
PC-DARTS [5]：华为出品，针对现有DARTS模型训练时需要 large memory and computing问题，提出了 channel sampling 和 edge normalization的技术，故两个字：更快更好 （0.1 GPU-days）。  <br>

ProxylessNAS1812:[paper](https://arxiv.org/abs/1812.00332) 
