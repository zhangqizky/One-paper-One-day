## Residual Dense Network for Image Super-Resolution

本篇论文主要是提出了一个RDB的sub-module结构，可以将不同层卷积提取到的局部特征进行更好的融合，再去学习到一个更加丰富的特征。
本文的主要思想就是更好的利用深度神经网络不同卷积层提取到的特征，如何将他们更好的进行融合，从而提高网络的效果，以及提高训练的稳定性。
每个rdb模块内部还采用了残差学习的思想。
不同rdb模块之间并不再采用dense的链接，而是都直接连到最后的GFF(Global Feature Fusion)模块上去。
同一个rdb模块内部采用dense的链接，每一层都能看到其之前其他层的特征信息。

