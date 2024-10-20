# MNBVC(Massive Never-ending BT Vast Chinese corpus)超大规模中文语料集

## 请媒体朋友们不要报道我们，让我们有更长久的时间可以收集整理数据。我们最怕捧杀了，您让我们保持低调，就是对中文算法圈做了大的贡献！

中文互联网上最古老最神秘(没有之一)的[MOP里屋社区](http://mnbvc.253874.net/)于2023.1.1庄重宣布:

**在英明神武的猫扑管子带领下，决心发挥社区所长(哪都长)，帮助开源社区长期更新一份最大的中文互联网语料集**

[MNBVC语料集](https://wiki.mnbvc.org) 不但包括主流文化，也包括各个小众文化甚至火星文的数据。MNBVC数据集包括新闻、作文、小说、书籍、杂志、论文、台词、帖子、wiki、古诗、歌词、商品介绍、笑话、糗事、聊天记录等一切形式的纯文本中文数据。数据均来源于互联网收集。

### 进度

目前总数据量35590GB，目标是达到chatGPT3.5的40T数据，目前进度88.97%。  

### 数据说明
压缩包密码为253874

压缩包内中文语料包括txt、json、jsonl和parquet（多模态专用）格式，最终会统一到jsonl和parquet格式。

压缩包根目录的links.txt里有每个子文件夹数据来源的url

每个子文件夹内有一张png格式的图片，是数据来源的网页截图

收录的数据将去掉大于等于8位的数字串进行脱敏

压缩包内数据只做了粗加工,例如html&xml转txt、csv&tsv转json等

### 索引和分类

我们没有能力对数据来源进行版权审核。虽然本数据集包括了数据来源信息，但为了长而持久的提供数据集的更新和下载，为了尽量避免版权争议，本数据集不提供压缩包内数据的索引和分类。并恳请大家克制住自己的分享欲，不要讨论压缩包的索引及所包含具体内容的信息。请大家更多的关注大数据量语料本身的应用，拜托大家低调的使用数据。

### huggingface

清洗完成的分类数据将陆续放到：[https://huggingface.co/datasets/liwu/MNBVC](https://huggingface.co/datasets/liwu/MNBVC)

### 一人行快，众人行远（摇人加速 发送邮件 MNBVC@253874.net）

各个小组长反映，数据清洗的苦力代码工作比较多，技术落地有点慢，希望有大量时间的同学来帮忙，会用python就行，有人手把手指导。请来帮忙的同学先阅读[项目的三条红线](https://wiki.mnbvc.org/doku.php/xmhx)。

 + OCR转码小组（被GPT4逼成了包含文字-图片的多模态语料组，增加编制），目前5人，缺5人（需有CV、NLP算法背景，想用nlp辅助ocr转码，有业内此领域顶尖大佬带队指导）
 + 问答语料小组，目前3人，缺4人（目前全是写python代码对齐问答项并人肉检查的苦力活，后面想利用算法模型做自动对齐）
 + 语料增强小组，目前3人，缺2人（想利用nlp补全缺字的语料，并进行文本质量检测等）
 + 代码语料小组和平行语料小组还缺几个打杂（后面由组长来决定到底干嘛）
 + 待建古文研究小组（研究地方志等古籍的转码，语料很多，难度很大）
 + 待建测试组（请测试同学加入，帮助我们提升数据质量，希望本组同学可以研究用llm直接生成测试用例和测试代码）

即使没空帮助项目做开发，也可以通过参加 ([语料元气弹](https://mnbvc.253874.net/upload/form.htm)) 项目，随手上传语料文档，来参与MNBVC语料集的建设。

### 中文大语料清洗工具

为处理大规模的中文语料，MNBVC项目组的同学在现有开源软件基础上做了优化，提供了更高效的版本:  

 + 更快速且准确的中文编码检测工具：[charset_mnbvc](https://github.com/alanshi/charset_mnbvc)    
 + 将txt批量转成jsonl并挑出段落重复度高的文件：[deduplication_mnbvc](https://github.com/aplmikex/deduplication_mnbvc)   
 + 从多层目录中按关键词采样一定数量的文件并保留目录结构：[scan_copy_files_mnbvc](https://github.com/wanng-ide/scan_copy_files_mnbvc)   
 + 将MNBVC语料格式统一的格式检查工具：[DataCheck_MNBVC](https://github.com/X94521/DataCheck_MNBVC)

### 代码仓库爬虫工具

现有各个开源代码语料集都有很严重的人为过滤现象，这让追赶chatGPT变得更为困难。为避免重复劳动，提供经过MNBVC大规模验证后的代码仓库爬虫代码。

 + 爬取github代码仓库meta信息：[publicRepos_mnbvc](https://github.com/washing1127/publicRepos_mnbvc)
 + 爬取github代码仓库最新版本代码：[github_downloader_mnbvc](https://github.com/imgingroot/github_downloader_mnbvc)
 + 爬取notabug代码仓库：[notabug_download_mnbvc](https://github.com/gezi2333/notabug_download_mnbvc)
 + 爬取bitbucket代码仓库：[bitbucket_crawl_mnbvc](https://github.com/chenzhwsysu57/bitbucket_crawl_mnbvc)
 + 将代码转为语料：[githubcode_extractor_mnbvc](https://github.com/LinnaWang76/githubcode_extractor_mnbvc)
 + 爬取commit记录：[get_github_commit_mnbvc](https://github.com/ppmmaiwo/get_github_commit_mnbvc)

### 多模态处理工具
 + PDF元信息抽取工具：[pdf_meta_data_mnbvc](https://github.com/MIracleyin/pdf_meta_data_mnbvc)       
 + PDF解析规则工具：[mmdp_mnbvc](https://github.com/MIracleyin/mmdp_mnbvc)
 + 第一版的pdf转txt工具：[pdf2txt_mnbvc](https://github.com/jayhenry/pdf2txt_mnbvc) 
 + Arxiv文档解析工具：[Arxiv_mllm_mnbvc](https://github.com/flychen59/Arxiv_mllm_mnbvc) 

### 各种清洗代码
 + wikihow清洗代码：[WikiHowQAExtractor-mnbvc](https://github.com/wanicca/WikiHowQAExtractor-mnbvc)  
 + 中国外交部发言清洗代码：[QA_with_reporters_from_the_Ministry_of_Foreign_Affair_mnbvc](https://github.com/UnstoppableCurry/QA_with_reporters_from_the_Ministry_of_Foreign_Affair_mnbvc)    
 + 各类数学题清洗代码：[Math_mnbvc](https://github.com/X94521/Math_mnbvc)   
 + stackexchange的清洗代码：[stackexchange_mnbvc](https://github.com/livehl/stackexchange_mnbvc)
 + 平行语料的清洗代码：[parallel_corpus_mnbvc](https://github.com/liyongsea/parallel_corpus_mnbvc)  
 + 试卷的清洗代码：[Exam-Question-Bank-Dataset-zh_mnbvc](https://github.com/UnstoppableCurry/Exam-Question-Bank-Dataset-zh_mnbvc)
 + 裁判文书网的清洗代码：[MNBVC-judgment](https://github.com/wormtooth/MNBVC-judgment)
 + 剧本杀的清洗代码：[MNBVC-pdf-extract](https://github.com/459737087/MNBVC-pdf-extract/)
 + DocLayNet的清洗代码：[DocLayNetPlus_mnbvc](https://github.com/luigide2020/DocLayNetPlus_mnbvc)

### 其他小工具
 + 从目录中指定文件后缀采样：[scan_copy_files_mnbvc](https://github.com/wanng-ide/scan_copy_files_mnbvc)
 + chinarxiv的爬虫：[chinaxivCrawler_mnbvc](https://github.com/wyzhangyuhan/chinaxivCrawler_mnbvc)
 + 从warc中提取文件：[warc_extractor_mnbvc](https://github.com/akira-l/warc_extractor_mnbvc)
 + psyarxiv、chemrxiv、biorxiv、medrxiv的爬虫：[xxarxiv_mnbvc](https://github.com/isLinXu/xxarxiv_mnbvc)
 
### 语料集下载信息(每个压缩包都会随着清洗进度更新):

1.通过[p2p微力](http://www.verysync.com/manual/)同步全部压缩包并接收更新    
建议关闭tcp穿透、关闭udp传输的微力设置。如不关闭，微力有可能堵塞路由器（同时也许传输速度更快）    
>微力密钥: B4MVPVJTK3DOOAOPVLJ3E7TA7RWW4J2ZEAXJRMRSRHSBPDB7OAFHUQ    
>[微力直达链接](https://link.verysync.com/#f=MNBVC%40xclimbing&sz=105E4&k=P4AJDJXHY3RCCOCDJZX3S7HO7FKK4X2NSOLXFAFGFVGPDRP7COTVIE&d=SJZHVB7GAZZLS2ZN43D3NNEBHPMU&t=1&tm=1676793101554&v=v2.16.0&a=1
)

2.通过百度网盘下载：[每个压缩包的百度网盘下载链接](dupan/README.md)

### Citation

Please cite the repo if you use the data or code in this repo.

```
@misc{mnbvc,
  author = {{MOP-LIWU Community} and {MNBVC Team}},
  title = {MNBVC: Massive Never-ending BT Vast Chinese corpus},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/esbatmop/MNBVC}},
}
```
