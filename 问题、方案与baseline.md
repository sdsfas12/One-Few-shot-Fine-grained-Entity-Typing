# 0.问题设置
考虑大量训练样本无标签但带有实体边界（NER或Link得到，不采用NER的标签），同时分类ontology下每一条目均带有少量带有完整标签的样例

# 1.解决方案
迭代框架下两种用pre-trained LM的策略

a) contrastive learning + kNN（参考[A Theory-Driven Self-Labeling Refinement Method for Contrastive Representation Learning](https://panzhous.github.io/assets/pdf/2021-NIPS-SLR.pdf) (Zhou, Xiong & Yuan, et al, NIPS 2021)）

b) prompt-tuning
# 2. 基线系统
a) few-shot方法（需文献调研，尽量考虑在类似的setting下容易想到/广泛认可的方法）

b) self-training方法（考虑以[An Attentive Fine-Grained Entity Typing Model with Latent Type Representation](https://aclanthology.org/D19-1641) (Lin & Ji, EMNLP 2019)中模型作为基础模型）
