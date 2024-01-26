code中代码介绍如下
data_engineering为特征工程
genGraph为通过data.npz文件生成图pkl文件
CNN为CNN模型
GCNdemo为提供的参考，并没有用到
grapgEmbedding为图嵌入尝试
SAGE为GraphSAGE模型
GNN为GCN/GAT/GIN/SGC模型

运行以上模型时先将data.npz放到该文件下。

CARE-GNN-master为Care-gnn模型，
其中，read_mat为生成mat格式文件，之后先用data_process生成4中边类型的邻接链表，之后运行train文件进行训练和预测，另外，edge_similarity为边相似度计算从而分组

PC-GNN-main为PC-gnn模型，
其中，把CARE-GNN-master中的data文件夹放到该文件下即可，运行main文件进行训练和预测

注意这里的CARE-GNN-master与PC-GNN-main与论文中提供的github下直接clone的不同，进行了大量修改。