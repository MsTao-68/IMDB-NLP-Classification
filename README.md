# IMDB-NLP-Classification
# 自然语言处理 IMDB 情感分析数据集任务

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
    1. 未来需要学习不调包 Transformer 和 Bert 的方式，从0实现自定义 Transformer 和 Bert 模型结构进行实验，进一步提升结果准确率。
