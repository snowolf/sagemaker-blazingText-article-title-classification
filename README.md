# sagemaker-blazingText-article-title-classification

This is a demo for Amazon SageMaker build-in algo [BlazingText](https://docs.aws.amazon.com/sagemaker/latest/dg/blazingtext.html) on Chinese article title classification. BlazingText could apply to word2vec and text classification.

本示例为Amazon SageMaker内置算法BlazingText在中文新闻标题分类的一个Demo。BlazingText可以做word2vec和文本分类。

The origin data is from https://github.com/skdjfla/toutiao-text-classfication-dataset
原始数据集来源于：https://github.com/skdjfla/toutiao-text-classfication-dataset

数据格式：

```
6552431613437805063_!_102_!_news_entertainment_!_谢娜为李浩菲澄清网络谣言，之后她的两个行为给自己加分_!_佟丽娅,网络谣言,快乐大本营,李浩菲,谢娜,观众们
```

每行为一条数据，以`_!_`分割的个字段，从前往后分别是 新闻ID，分类code（见下文），分类名称（见下文），新闻字符串（仅含标题），新闻关键词



分类code与名称：

```
100 民生 故事 news_story
101 文化 文化 news_culture
102 娱乐 娱乐 news_entertainment
103 体育 体育 news_sports
104 财经 财经 news_finance
106 房产 房产 news_house
107 汽车 汽车 news_car
108 教育 教育 news_edu 
109 科技 科技 news_tech
110 军事 军事 news_military
112 旅游 旅游 news_travel
113 国际 国际 news_world
114 证券 股票 stock
115 农业 三农 news_agriculture
116 电竞 游戏 news_game
```



数据规模：

共382688条，分布于15个分类中。



采集时间：

2018年05月

