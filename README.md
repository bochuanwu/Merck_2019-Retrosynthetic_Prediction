# “默克”杯逆合成反应预测大赛/Merck_2019-Retrosynthetic_Prediction

#比赛链接/The Competition Address:[link](https://www.kesci.com/home/competition/5c35b0aa4ea711002cafcaa6)

#数据说明/Dataset announcement
1. 数据来源/Dataset resource: Lowe, Daniel (2017): [Chemical reactions from US patents (1976-Sep2016). figshare. Fileset.](https://figshare.com/articles/Chemical_reactions_from_US_patents_1976-Sep2016_/5104873)

2. 数据格式/Dataset format:
反应物（reactants），反应试剂（reagents），反应产物（production）
{ID，反应物1.反应物2.反应物3...>反应试剂1.反应试剂2...>反应产物1.反应产物2.反应产物3...
{ID, reactants1/reactants2...>reagents1.reagents2...>production1.production2.production3...

3. 数据内容/Dataset content:
训练集(training Data):
1,112,557个化学反应 / 1,112,657 reactions 
测试集(test Data):
277,746个化学反应 / 277,746 reactions


#可能性尝试/Possible solution:
1. sequence2sequence
2. Translator
3. ????

#参考代码及灵感/reference paper and code:
1. 代码/code [Schwaller, Philippe, et al. "“Found in Translation”: predicting outcomes of complex organic chemistry reactions using neural sequence-to-sequence models." Chemical science 9.28 (2018): 6091-6098](https://github.com/frnsys/retrosynthesis_planner)

2. 论文/papper Bowen,Ramsundar,et al. "Retrosynthetic Reaction Prediction Using Neural Sequence-to-Sequence Models"

3. 代码/code [A TensorFlow Implementation of the Transformer: Attention Is All You Need](https://github.com/Kyubyong/transformer)

4. 论文/papper [Linking the Neural Machine Translation and the Prediction of Organic Chemistry Reactions](https://arxiv.org/abs/1612.09529)


#数据分析，预处理/data analysis, Preprocessing：
 绝大多数化学式产物数都小于6：  
 product_num_count: [(1, 1029164), (2, 74762), (3, 6928), (4, 1266), (5, 377), (6, 88), (7, 43), (8, 22), (9, 3), (10, 3), (13, 1)]  
 
 反应产物以及反应物的长度分布：  
 ![error](https://github.com/bochuanwu/Merck_2019-Retrosynthetic_Prediction/raw/master/img/plwt2q22e.png)  
      
