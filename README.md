# MNBVC(Massive Never-ending BT Vast Chinese corpus)超大规模中文语料集

## 请媒体朋友们不要报道我们，让我们有更长久的时间可以收集整理数据。您让我们保持低调，就是对中文算法圈做了大的贡献！

响应[符尧博士的号召](https://yaofu.notion.site/GPT-3-5-360081d91ec245f29029d37b54573756)，危机存亡之秋，为避免技术断代，为将几千年历史的中文之美传承给AI。

中文互联网上最古老最神秘(没有之一)的[里屋社区](http://mnbvc.253874.net/)于2023.1.1庄重宣布:

**在英明神武的里屋管子带领下，决心发挥社区所长(哪都长)，帮助开源社区长期更新一份最大的中文互联网语料集**

MNBVC数据集不但包括主流文化，也包括各个小众文化甚至火星文的数据。MNBVC数据集包括新闻、作文、小说、书籍、杂志、论文、台词、帖子、wiki、古诗、歌词、商品介绍、笑话、糗事、聊天记录等一切形式的纯文本中文数据。数据均来源于互联网收集。

### 进度

目前总数据量3518.6GB，目标是达到chatGPT的40T数据，目前进度8.9%。

### 数据说明
压缩包密码为253874

压缩包内中文语料均清洗为txt和json（包括jsonl）格式

压缩包根目录的links.txt里有每个子文件夹数据来源的url

每个子文件夹内有一张png格式的图片，是数据来源的网页截图

收录的数据将去掉大于等于8位的数字串进行脱敏

压缩包内数据只做了粗加工,例如html&xml转txt、csv&tsv转json等

### 索引和分类

我们没有能力对数据来源进行版权审核。虽然本数据集包括了数据来源信息，但为了长而持久的提供数据集的更新和下载，为了尽量避免版权争议，本数据集不提供压缩包内数据的索引和分类。并恳请大家克制住自己的分享欲，不要讨论压缩包的索引及所包含具体内容的信息。请大家更多的关注大数据量语料本身的应用，拜托大家低调的使用数据。

### 大中文语料清洗工具

为处理大规模的中文语料，MNBVC项目组的同学在现有开源软件基础上做了优化，提供了更高效的版本:  

更快速且准确的中文编码检测工具：[charset_mnbvc](https://github.com/alanshi/charset_mnbvc)    
将txt批量转成jsonl并挑出段落重复度高的文件：[deduplication_mnbvc](https://github.com/aplmikex/deduplication_mnbvc)    

### 代码仓库爬虫工具

现有各个开源代码语料集都有很严重的人为过滤现象，这让追赶chatGPT变得更为困难。为避免重复劳动，提供经过MNBVC大规模验证后的代码仓库爬虫代码。

 + 爬取代码仓库meta信息：[publicRepos_mnbvc](https://github.com/washing1127/publicRepos_mnbvc)
 + 爬取代码仓库最新版本代码：待提供
 + 爬取commit记录：待提供

### huggingface

清洗完成的分类数据将陆续放到：[https://huggingface.co/datasets/liwu/MNBVC](https://huggingface.co/datasets/liwu/MNBVC)

### 一人行快，众人行远（摇人加速）

 + OCR转码小组（被GPT4逼成了包含文字-图片的多模态语料组，增加编制），目前5人，缺5人（需有CV、NLP算法背景，想用nlp辅助ocr转码，有业内此领域顶尖大佬带队指导）
 + 问答语料小组，目前3人，缺4人（目前全是写python代码对齐问答项并人肉检查的苦力活，后面想利用算法模型做自动对齐）
 + 语料增强小组，目前3人，缺2人（想利用nlp补全缺字的语料，并进行文本质量检测等）
 + 代码语料小组和平行语料小组还缺几个打杂（后面由组长来决定到底干嘛）
 + 待建古文研究小组（研究地方志等古籍的转码，语料很多，难度很大）

### 语料集下载信息(每个压缩包都会随着清洗进度更新):

通过[p2p微力](http://www.verysync.com/manual/)同步全部压缩包并接收更新    
建议关闭tcp穿透、关闭udp传输的微力设置。如不关闭，微力有可能堵塞路由器（同时也许传输速度更快）    
>微力密钥: B4MVPVJTK3DOOAOPVLJ3E7TA7RWW4J2ZEAXJRMRSRHSBPDB7OAFHUQ    
>[微力直达链接](https://link.verysync.com/#f=MNBVC%40xclimbing&sz=105E4&k=P4AJDJXHY3RCCOCDJZX3S7HO7FKK4X2NSOLXFAFGFVGPDRP7COTVIE&d=SJZHVB7GAZZLS2ZN43D3NNEBHPMU&t=1&tm=1676793101554&v=v2.16.0&a=1
)

20221224.zip 压缩包4.57GB，原始13.45GB   
[百度网盘](https://pan.baidu.com/s/19DWSU68IukKWQqoEgjuVRQ?pwd=dh2n) 

20221225.zip 压缩包7.53GB，原始17.68GB   
[百度网盘](https://pan.baidu.com/s/1PXhoGY7g_GXpfKHi7Gyp9A?pwd=gr63) 

20230101.zip 压缩包7.34GB，原始17.11GB   
[百度网盘](https://pan.baidu.com/s/1TLEkczf5_pQlWcXwLPPcEw?pwd=78uq) 

20230102.zip 压缩包9.67GB，原始32.33GB   
[百度网盘](https://pan.baidu.com/s/1oVt7e-MfTRYv7h_aaAX7yw?pwd=nnkc) 

20230103.zip 压缩包9.77GB，原始32.59GB   
[百度网盘](https://pan.baidu.com/s/1ZO7_RgcEmHW40gOh2BfGfA?pwd=cnv3)

20230104.zip 压缩包12.36GB，原始34.85GB   
[百度网盘](https://pan.baidu.com/s/1cmEA15Y0Bk7sMo3BlIBMyg?pwd=v7me)

20230105.zip 压缩包8.17GB，原始26.87GB   
[百度网盘](https://pan.baidu.com/s/1KEZxJtatTHXQgp7g01jRWg?pwd=mh8s) 

20230106.zip 压缩包7.15GB，原始22.69GB   
[百度网盘](https://pan.baidu.com/s/1pUvxDaXL_rYzEz4MSMRN4A?pwd=eyvq) 

20230107.zip 压缩包6.2GB，原始13.14GB   
[百度网盘](https://pan.baidu.com/s/1NfuytYsAHqtACTs2Yfv-XA?pwd=eape) 

20230108.zip 压缩包9.56GB，原始25.84GB  
[百度网盘](https://pan.baidu.com/s/1ZA3ljZ18LcLeUrjHyWH9Uw?pwd=kywq) 

20230109.zip 压缩包7.63GB，原始20.84GB   
[百度网盘](https://pan.baidu.com/s/1weZmOaz4SwHWf9-h8RdHBw?pwd=441t) 

20230110.zip 压缩包5.79GB，原始15.6GB   
[百度网盘](https://pan.baidu.com/s/1YjiYGe6AZfgR6qNFc9SwCw?pwd=8vf9) 

20230112.zip 压缩包11.26GB，原始23.92GB   
[百度网盘](https://pan.baidu.com/s/1mtCQ8Sz7ImZ9U-0cM-qdcQ?pwd=b9sr) 

20230113.zip 压缩包8.21GB，原始17.54GB   
[百度网盘](https://pan.baidu.com/s/1tv6ghAgXuHO7nCqn7YVfjA?pwd=fa49) 

20230114.zip 压缩包5.65GB，原始14.79GB   
[百度网盘](https://pan.baidu.com/s/18dY4-7TeJksStIVYXCkJlw?pwd=i6sd) 

20230115.zip 压缩包7.53GB，原始23.1GB   
[百度网盘](https://pan.baidu.com/s/1NRz_0pz2XfhJRH8r59zYhQ?pwd=2qnj) 

20230116.zip 压缩包3.29GB，原始10.81GB   
[百度网盘](https://pan.baidu.com/s/1tIArlWw_pcoxEAtcYkrblg?pwd=ysqy) 

20230117.zip 压缩包11.71GB，原始29.54GB   
[百度网盘](https://pan.baidu.com/s/1YgOMZjFAzx3WKSPEN056rg?pwd=biew) 

20230118.zip 压缩包11.71GB，原始31.47GB   
[百度网盘](https://pan.baidu.com/s/1gFIbANFo4xU7GjE0zFBxLA?pwd=x9yu) 

20230119.zip 压缩包11.21GB，原始31.33GB   
[百度网盘](https://pan.baidu.com/s/1h3QFWz-kQvvs38a7mcus_w?pwd=xsa9) 

20230120.zip 压缩包12.32GB，原始31.45GB   
[百度网盘](https://pan.baidu.com/s/1PxwJE5JqEIpjBmEWqFLoMA?pwd=kr3f) 

20230121.zip 压缩包13.44GB，原始32.08GB   
[百度网盘](https://pan.baidu.com/s/1dgUIxXaA14fO5ZzdCRHzYA?pwd=82cs) 

20230122.zip 压缩包12.49GB，原始29.5GB   
[百度网盘](https://pan.baidu.com/s/18JwXVhakYsrvHW7pZL2vgQ?pwd=bjnj) 

20230123.zip 压缩包11.84GB，原始28.08GB   
[百度网盘](https://pan.baidu.com/s/1l8JdVh6dC3mVaPWSbGrLUw?pwd=issx)  

20230124.zip 压缩包10.57GB，原始27.16GB   
[百度网盘](https://pan.baidu.com/s/18t6cOMo00f0vKfk5fUo0Hw?pwd=fuyi) 

20230125.zip 压缩包6.15GB，原始26.25GB   
[百度网盘](https://pan.baidu.com/s/14HkIN5rvab74-bv6NQxTjQ?pwd=6quh) 

20230126.zip 压缩包9.12GB，原始26.44GB   
[百度网盘](https://pan.baidu.com/s/18wrH6ptSiU_BlZIbRIpb4A?pwd=mzte) 

20230127.zip 压缩包10.73GB，原始27.12GB   
[百度网盘](https://pan.baidu.com/s/1WpxRHn9BUe92KzY4gZp_Ew?pwd=47kr) 

20230128.zip 压缩包8.94B，原始27.31GB   
[百度网盘](https://pan.baidu.com/s/1fBGdv2V8ZHjJCA_Snjc5Bw?pwd=4de7) 

20230129.zip 压缩包9.76GB，原始32.36GB   
[百度网盘](https://pan.baidu.com/s/188AqbYAEmPHgq0y3LYWe0g?pwd=36vt) 

20230130.zip 压缩包7.61GB，原始19.97GB   
[百度网盘](https://pan.baidu.com/s/1HfVDxg8KatDnvsvHOjeEQg?pwd=k8ue) 

20230131.zip 压缩包10.39GB，原始31.62GB   
[百度网盘](https://pan.baidu.com/s/11Yi8-BQyr-jSMW-6m_I2ow?pwd=rjmt) 

20230132.zip 压缩包9.41GB，原始28.9GB   
[百度网盘](https://pan.baidu.com/s/1bw1SdL0eDoc_gE0pbfXmNg?pwd=6ic3) 

20230133.zip 压缩包9.39GB，原始29.51GB   
[百度网盘](https://pan.baidu.com/s/1dGz9PytYNRes8Hu9VIJrHg?pwd=ju2j) 

20230134.zip 压缩包5.20GB，原始21.87GB   
[百度网盘](https://pan.baidu.com/s/1mNrLcphIo7K3RugtvsMcDA?pwd=t3xd) 

20230135.zip 压缩包4.57GB，原始18.55GB   
[百度网盘](https://pan.baidu.com/s/1M7ECTb8Z7zTYcqXR1iObRA?pwd=xka2)

20230136.zip 压缩包5.16GB，原始20.94GB   
[百度网盘](https://pan.baidu.com/s/1aVHgZ2007WEUrnx_P8KIDA?pwd=9w9x)

20230137.zip 压缩包4.99GB，原始20.39GB   
[百度网盘](https://pan.baidu.com/s/1CEhDlgBc6agh4b3GbqsiWg?pwd=nawt)

20230138.zip 压缩包4.06GB，原始16.35GB   
[百度网盘](https://pan.baidu.com/s/1LH4uMauuv5ebYG5JISNq1A?pwd=8sda)

20230139.zip 压缩包4.60GB，原始18.58GB   
[百度网盘](https://pan.baidu.com/s/1ccbLT2jbuCWicZCT6CuBVQ?pwd=vt6a)

20230140.zip 压缩包4.45GB，原始17.95GB   
[百度网盘](https://pan.baidu.com/s/1QJo80JXKHGNJL8SjGR9aZQ?pwd=jb5n)

20230141.zip 压缩包4.59GB，原始20.41GB   
[百度网盘](https://pan.baidu.com/s/1ubwTEvoAeoDV5wk129EaUQ?pwd=3q8i)

20230142.zip 压缩包9.59GB，原始31.03GB   
[百度网盘](https://pan.baidu.com/s/1xXn5ryqwVJ3gaCTzc7tQEQ?pwd=gjci) 

20230143.zip 压缩包8.24GB，原始27.07GB   
[百度网盘](https://pan.baidu.com/s/1k7H_LGf3MiQhAVWYHnQWuA?pwd=dcju) 

20230144.zip 压缩包6.42GB，原始32.05GB   
[百度网盘](https://pan.baidu.com/s/1qBNIAo_uEmhY3yO1TaVV0A?pwd=ea8r)  

20230145.zip 压缩包6.41GB，原始32.03GB   
[百度网盘](https://pan.baidu.com/s/10r9cH6Dy1cmAL_PdkDMNpQ?pwd=k31g) 

20230146.zip 压缩包6.39GB，原始31.91GB   
[百度网盘](https://pan.baidu.com/s/1wU-XR-ljexZoux5hjl9OLQ?pwd=5gkm) 

20230147.zip 压缩包6.40GB，原始32GB   
[百度网盘](https://pan.baidu.com/s/1tHKqnnde7fP_vDqIzL1lRA?pwd=ezci) 

20230148.zip 压缩包6.42GB，原始32.1GB   
[百度网盘](https://pan.baidu.com/s/1p100axKypE1MERzV4iJz4g?pwd=wwbp)  

20230149.zip 压缩包6.40GB，原始31.91GB   
[百度网盘](https://pan.baidu.com/s/1wIaRx5_ZMGhnYmAWeBVfXQ?pwd=ar95) 

20230150.zip 压缩包6.43GB，原始32.1GB   
[百度网盘](https://pan.baidu.com/s/1P5EaxHjLmBlV3w971b58VQ?pwd=xtsu) 

20230151.zip 压缩包6.42GB，原始32.09GB   
[百度网盘](https://pan.baidu.com/s/1PGJb6BpZ6rl1HXBDGtAtvA?pwd=9fas) 

20230152.zip 压缩包6.45GB，原始32.2GB   
[百度网盘](https://pan.baidu.com/s/1m_9qzJ4kv34yz3QEq43TBQ?pwd=huqa) 

20230153.zip 压缩包6.42GB，原始32.04GB   
[百度网盘](https://pan.baidu.com/s/1Q35RkVXmIBzY3gWxl5gH5g?pwd=kmqj) 

20230154.zip 压缩包6.43GB，原始32.1GB   
[百度网盘](https://pan.baidu.com/s/10W6QUugiA860QoRWXi7hmQ?pwd=mniw) 

20230155.zip 压缩包6.41GB，原始32.04GB   
[百度网盘](https://pan.baidu.com/s/1sLVXOR8C9d91O016khNV2A?pwd=5k3c) 

20230156.zip 压缩包6.42GB，原始32.06GB   
[百度网盘](https://pan.baidu.com/s/1te8mJqiqnjY9FvBahbAgGA?pwd=3w3h) 

20230157.zip 压缩包6.42GB，原始31.99GB   
[百度网盘](https://pan.baidu.com/s/1sKeKWDuva726Hoi1FljtaA?pwd=b6u7) 

20230158.zip 压缩包6.42GB，原始32.09GB   
[百度网盘](https://pan.baidu.com/s/1GDQLM_rQvcAb_kFob7s1AQ?pwd=d8xp) 

20230159.zip 压缩包6.38GB，原始31.94GB   
[百度网盘](https://pan.baidu.com/s/1hPiYfbnwSCfN1J7EOzY_Sw?pwd=6f5v) 

20230160.zip 压缩包6.41GB，原始32.05GB   
[百度网盘](https://pan.baidu.com/s/1rWQeabjaY_OZi26QDHiUnA?pwd=w4hm) 

20230161.zip 压缩包6.4GB，原始31.89GB   
[百度网盘](https://pan.baidu.com/s/1olRDOCdqmWQmbUbdLgfMBQ?pwd=ge4u) 

20230162.zip 压缩包6.42GB，原始32.06GB   
[百度网盘](https://pan.baidu.com/s/1d_LW_ABm62z2CnllTRR-MA?pwd=5pwq) 

20230163.zip 压缩包6.42GB，原始32.11GB   
[百度网盘](https://pan.baidu.com/s/17cX7EUc8oEsquQ908zukXQ?pwd=28fg) 

20230164.zip 压缩包6.42GB，原始32.1GB   
[百度网盘](https://pan.baidu.com/s/1p-NjP8J1TpSnpEeYvG9s9Q?pwd=8vds) 

20230165.zip 压缩包6.4GB，原始32.02GB   
[百度网盘](https://pan.baidu.com/s/1iJv7_kxh6nSqeZ2QtU0q9A?pwd=uxeq) 

20230166.zip 压缩包6.45GB，原始32.19GB   
[百度网盘](https://pan.baidu.com/s/1BgLe7zOYqkxBVFRtcFJNzg?pwd=n28t) 

20230167.zip 压缩包6.4GB，原始32.05GB   
[百度网盘](https://pan.baidu.com/s/10BAdvVDbycVhgXENDDlc_w?pwd=k279) 

20230168.zip 压缩包6.42GB，原始32.02GB   
[百度网盘](https://pan.baidu.com/s/1upJEVCsNqnn3JHkNX2q2iA?pwd=i9t4) 

20230169.zip 压缩包6.42GB，原始32.04GB   
[百度网盘](https://pan.baidu.com/s/1VOiLvosbq8FFMNs1C2nZIg?pwd=gdyk)  

20230170.zip 压缩包6.42GB，原始32.03GB   
[百度网盘](https://pan.baidu.com/s/1qJ77NMjxPS9nWgciG3NvLw?pwd=441v) 

20230171.zip 压缩包6.41GB，原始29.81GB   
[百度网盘](https://pan.baidu.com/s/1y7yA7AmunAJmtG8JsmJnGw?pwd=31xd) 

20230172.zip 压缩包2.03GB，原始8.75GB   
[百度网盘](https://pan.baidu.com/s/1EAh-ud5wt2y_P4b2KBhGeg?pwd=2grk) 

20230173.zip 压缩包9.70GB，原始25.02GB   
[百度网盘](https://pan.baidu.com/s/1XnA6P04mNQm0J_tRnWYy_w?pwd=hi2s) 

20230174.zip 压缩包5.51GB，原始14.56GB   
[百度网盘](https://pan.baidu.com/s/19AU0h27WrdAZMfSSBh2UIQ?pwd=bant) 

20230175.zip 压缩包10.23GB，原始31.73GB   
[百度网盘](https://pan.baidu.com/s/1eFYqfGqM46sWebHBCyl0pA?pwd=53q9) 

20230176.zip 压缩包7.1GB，原始18.74GB   
[百度网盘](https://pan.baidu.com/s/16wb-5DdKn0RRqtivt8KSXA?pwd=x721) 

20230177.zip 压缩包7.7GB，原始18.8GB   
[百度网盘](https://pan.baidu.com/s/1bZey3ZDRtXsteaUAWr7Uqg?pwd=wr5q) 

20230178.zip 压缩包7.78GB，原始18.26GB   
[百度网盘](https://pan.baidu.com/s/1PDc_r8GOK_2hNa0DeJq-RQ?pwd=tm53) 

20230179.zip 压缩包8.81GB，原始20.55GB   
[百度网盘](https://pan.baidu.com/s/1XDA30rs92YCQVWxuT7NSIg?pwd=uw7c) 

20230180.zip 压缩包9.56GB，原始22.08GB   
[百度网盘](https://pan.baidu.com/s/1cljUdAP7nT0gTkC_bY8JpA?pwd=n3be) 

20230181.zip 压缩包9.06GB，原始20.47GB   
[百度网盘](https://pan.baidu.com/s/1wtyEpIV22LpS8Ac4kKHMng?pwd=sbfr) 

20230182.zip 压缩包9.22GB，原始20.82GB   
[百度网盘](https://pan.baidu.com/s/1sbc9gJHspeJSlPcEBYM3MA?pwd=jzv7) 

20230183.zip 压缩包9.13GB，原始20.18GB   
[百度网盘](https://pan.baidu.com/s/1yKczRjZjl1Tvvmfw9CAwkA?pwd=gmpe) 

20230184.zip 压缩包8.11GB，原始18.87GB   
[百度网盘](https://pan.baidu.com/s/1BmJ__Ka_5Me5NH6craz_Yg?pwd=dsef) 

20230185.zip 压缩包11.52GB，原始24.72GB   
[百度网盘](https://pan.baidu.com/s/1K9OLSk_ifXEyPvPj6GYNwQ?pwd=n2a9) 

20230186.zip 压缩包10.57GB，原始35.28GB   
[百度网盘](https://pan.baidu.com/s/1bJgyNItkRu6H-NFBaHjYpw?pwd=xqbf) 

20230187.zip 压缩包11.12GB，原始37.01GB   
[百度网盘](https://pan.baidu.com/s/1LSD0EQpL6OLvPWExVXVpFA?pwd=am58) 

20230188.zip 压缩包10.43GB，原始34.78GB   
[百度网盘](https://pan.baidu.com/s/1sJFp5Ia6TBIylJU_VVEgcg?pwd=35x4) 

20230189.zip 压缩包8.25GB，原始27.31GB   
[百度网盘](https://pan.baidu.com/s/12S5a-1ljqcp-UQ5_3D4E3A?pwd=wc75) 

20230190.zip 压缩包9.20GB，原始30.38GB   
[百度网盘](https://pan.baidu.com/s/1ZA_TRw3gSAjzH8u2PmFJ4w?pwd=a8ce) 

20230191.zip 压缩包7.13GB，原始22.7GB   
[百度网盘](https://pan.baidu.com/s/1SNDtlRPnHP_Q3SrlBv-IgA?pwd=hvg1) 

20230192.zip 压缩包10.19GB，原始33.39GB   
[百度网盘](https://pan.baidu.com/s/1wE0hsN_HP1P2l7QPCOi4zA?pwd=4b3g) 

20230193.zip 压缩包10.51GB，原始34.59GB   
[百度网盘](https://pan.baidu.com/s/13xlR40gtMXN0JV7GHn1tyg?pwd=5288) 

20230194.zip 压缩包10.40GB，原始33.9GB   
[百度网盘](https://pan.baidu.com/s/1_gmdRVK-zWJHMDkrlS_0Cw?pwd=rw37) 

20230195.zip 压缩包5.39GB，原始17.93GB   
[百度网盘](https://pan.baidu.com/s/1mI1GVi-Ytnh92APH7U4PgQ?pwd=ms9t) 

20230196.zip 压缩包3.28GB，原始10.31GB   
[百度网盘](https://pan.baidu.com/s/18-Mdtg3bfN-m5wfMt5GxQg?pwd=73p7) 

20230301.zip 压缩包2.09GB，原始36.09GB   
[百度网盘](https://pan.baidu.com/s/1VtBXTfZdmu-ZqAkl669eUQ?pwd=326v) 

20230302.zip 压缩包2.54GB，原始44.53GB   
[百度网盘](https://pan.baidu.com/s/15zvXGUPAa-tVaEkQ-SDclA?pwd=fip7) 

20230303.zip 压缩包2.47GB，原始45.32GB   
[百度网盘](https://pan.baidu.com/s/1rL4unTTocL1kqI1FalMI0g?pwd=bs7a) 

20230304.zip 压缩包2.51GB，原始45.63GB   
[百度网盘](https://pan.baidu.com/s/1fUF5uorCd5CMgPe5oE3CZw?pwd=kewu) 

20230305.zip 压缩包2.75GB，原始50.3GB   
[百度网盘](https://pan.baidu.com/s/1jtux-hmi5-aOvbxPK_RvzA?pwd=529z)

20230306.zip 压缩包2.61GB，原始48.18GB   
[百度网盘](https://pan.baidu.com/s/1VJOpdWbv-3PuKZhMkKRM0g?pwd=6gd5) 

20230307.zip 压缩包2.62GB，原始48.24GB   
[百度网盘](https://pan.baidu.com/s/1sCxLzEGQrKN3pmniPjFdWA?pwd=n8dg) 

20230308.zip 压缩包2.59GB，原始47.55GB   
[百度网盘](https://pan.baidu.com/s/1wkrs40xWmXE0KYY8_gHQ0Q?pwd=3yrx) 

20230309.zip 压缩包2.74GB，原始50.27GB   
[百度网盘](https://pan.baidu.com/s/1fTzsRPeVTT4qHjZK0ow2yg?pwd=f985) 

20230310.zip 压缩包2.82GB，原始51.62GB   
[百度网盘](https://pan.baidu.com/s/17znl0fpkXziC5B6HFAI5rA?pwd=xmwy) 

20230311.zip 压缩包2.63GB，原始48.22GB   
[百度网盘](https://pan.baidu.com/s/1Sa1dqp6J0i7LbZmawtRZrQ?pwd=5p84) 

20230312.zip 压缩包2.65GB，原始48.4GB   
[百度网盘](https://pan.baidu.com/s/1q6Iwnxo4dMtwT1EIW6h1zQ?pwd=f9xn) 

20230313.zip 压缩包2.60GB，原始47.15GB   
[百度网盘](https://pan.baidu.com/s/1slkwtW6QiqCr7etCLn5s7A?pwd=4u9r) 

20230314.zip 压缩包2.83GB，原始51.72GB   
[百度网盘](https://pan.baidu.com/s/1if2aypPWpBBp2tBiODei2w?pwd=pn3c) 

20230315.zip 压缩包2.79GB，原始51.48GB   
[百度网盘](https://pan.baidu.com/s/13cxlSuNm9ydXeSF5gudFjQ?pwd=ctas) 

20230316.zip 压缩包2.82GB，原始51.72GB   
[百度网盘](https://pan.baidu.com/s/192LJy4H_yyZ7_7UypKJmCw?pwd=vngv) 

20230317.zip 压缩包2.59GB，原始47.78GB   
[百度网盘](https://pan.baidu.com/s/1wutho4Gi-v6ijIcGN9B6UA?pwd=gb82) 

20230318.zip 压缩包2.52GB，原始46.36GB   
[百度网盘](https://pan.baidu.com/s/17dM3cTVj1JPmCQWOCsNdTw?pwd=j2mx) 

20230319.zip 压缩包2.57GB，原始47.59GB   
[百度网盘](https://pan.baidu.com/s/144sTA-1-SCQeOK0ICPZhUA?pwd=3jd4) 

20230320.zip 压缩包2.59GB，原始47.92GB   
[百度网盘](https://pan.baidu.com/s/1X4ITkMwqCNDCddyOOJDRqQ?pwd=1iw8) 



