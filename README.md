# IMDB-NLP-Classification
# 自然语言处理 IMDB 情感分析数据集任务
- 算法验证集准确度：总体88% -> Transformer模型，准确度总体提升5.8%。
- [x] Version 0: TF-IDF - Logistic
     * Logistic Score: 0.90000 

- [x] Version 1: Word2Vec - Word Embedding method using Machine Learning Model (cpu)
     * Random Forest Score: 0.82248
     * Logistic Score: 0.87944
     * XGBoost Score: 0.86352

- [x] Version 2: Bert-pretrained model + Transformer
     * Transformer Score: 0.93800

- [x] Version 3: Bert-pretained + Attention mask + Bert Model
     * Bert Score: 0.90000

## 总结、反思与展望

- 实验环境：
>![image](https://user-images.githubusercontent.com/84648756/167340706-dd5b4757-7f60-47a0-8f94-682e0e916d4e.png)

- Transformer:
>![image](https://user-images.githubusercontent.com/84648756/167340831-9dceb11b-b9d1-4a30-988c-0f692f683b50.png)

- Bert:
>![image](https://user-images.githubusercontent.com/84648756/167340901-f2608fb3-6c3e-4905-adc6-84538dc73e83.png)

- 反思：
    1. 电脑从Win10更新到Win11，因为没有重新配置导致，本机GPU无法使用。教训：遇到问题不应该拖延，应该第一时间记录或者解决。
    2. 第一次使用Colab，数据集难以上传。展望：疫情之后开自己的信用卡Visa，使用Google Cloud。
    3. 如果是个人项目，Kaggle就足以满足练手的需求。教训：要利用好现有的条件，而不是盲目无方向。
- 收获：
    1. 本项目融合了四种不同的实验（统计方法、机器学习方法、深度学习方法：Transformer 模型、深度学习方法：Bert 模型），回顾了传统机器学习的方法，学会使用正则表达式进行文本预处理。
    2. 读了 Transformer 论文，仔细研究了 Encoder-Decoder 架构以及注意力机制，并且了解了 Bert 模型对于 Transformer 的改进之处。
    3. 学会在不同平台使用 GPU 和预训练模型。
- 展望：
    1. 本次实验过程中，使用 Bert 预训练的 Transformer 的准确率却高于完整 Bert 的模型，可能是因为偶然性因素，具体尚不清楚。使用深度学习模型，部署模型是可调节的参数是批量大小、Padding 的序列最大长度、学习率、训练周期和丢弃率，在模型架构不变动的基础上，训练准确率提升较难。未来需要学习不调包 Transformer 和 Bert 的方式，从0实现自定义 Transformer 和 Bert 模型结构进行实验，进一步提升结果准确率。
    2. 发现对于英文的自然语言处理相比中文比较简单，因为中文需要关注分词的粒度和歧义的问题，未来的展望：使用自然语言处理技术做中文分词和情感分析的实验。
------
（以下 2022 年 5 月 17 日星期二 更新）
- Bert 和 Transformer 模型作为目前自然语言处理领域 SOTA 的模型，捕获序列能力强，虽然模型训练成本高，但是可以直接部署预训练模型进行迁移学习和参数微调，进行模型训练用于捕获序列特征，为下游任务进行训练。
- 未来展望：多模态的自然语言处理的情感分析，是未来研究方向的蓝海之一（目前瓶颈：高质量的标注数据少）。
------
（以下 2022 年 5 月 24 日星期二 更新）
- 目前，GPT-2（General Pretrained Transformer 2.0）在自然语言处理领域使用也较多，GPT-1 推出早于 Bert，Google 推出的 Bert 模型是目的是为了对标 GPT-1 在 2019 年达到了 SOTA 的水平。GPT-2 是 GPT-1 的升级版，是生成式的语言预测模型，使用无监督的方式、40GB 的爬虫语料库、堆叠 48 层单向 Transformer模块、扩大序列长度和网格参数级，因此，通过了 GLUE 标准的 7 个测试。此外，GPT-3 已经在 2020 年推出，GPT-2 和 GPT-3 都可以用于创造性写作（包括：新闻、小说、诗歌、歌曲等，甚至自动生成全栈代码），但是由于商业价值 OpenAI和微软并没有开源。
- 对于Transformer 的未来展望：是在 GPT 系列基础上优化成通用 Transformer-based 预训练语言模型，并尝试解决语言重复和曝光问题。

