
# SSAIS：Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研

## 项目简介

在发论文之前，需要调研相关论文并看论文，才能知道发展现状，并找到差异化和创新点。同理，在创业之前，需要调研相关的创业公司并研究产品、市场和商业模式，才能知道发展现状，并找到差异化和创新点。SSAIS（Survey of Startups on Artificial Intelligence Software）是一个AI软件创业公司调研仓库。在该仓库具有如下几个特点：
- 持续更新：将持续加入更多的AI创业公司。
- 多层次：覆盖AI的基础设施领域到应用领域。"!"表示该公司的是开源公司。
- 技术角度：从技术的角度来AI软件创业公司进行分类，给AI创业人士启发。
- 多国家：覆盖中国、美国和以色列等。"#"该公司的是开源公司是以色列公司
- 商业价值：给出AI创业公司的最新一轮融资额。举例：Scale.ai :$155M ==》表示 scale.ai公司最新一轮融资155 million dollor。融资额来源于创投数据库,并不一定准确。

## 作者

作者：Warren Wen（[耀途资本](https://www.glory-ventures.com/)，glory-ventures） 

联系方式：warrenwen@glory-ventures.com

## 特别提醒
SSAIS—MLOps是SSAIS中的MLOps部分，对MLOps的相关公司，进行更详细的归纳和总结，[点击进入](./SSAIS_MLOps.md)


## 目录

* [AI基础设施Infrastructure](#AI基础设施Infrastructure) 
  * [异构加速器虚拟化](#异构加速器虚拟化) 
  * [准备](#准备) 
  * [构建](#构建) 
  * [部署和监控](#部署和监控) 
  * [安全与隐私](#安全与隐私) 
  * [NLP](#NLP) 
  * [向量搜索与数据库](#向量搜索与数据库) 
* [文本NLP](#文本NLP) 
  * [NLP](#NLP) 
  * [预训练模型](#预训练模型) 
  * [机器翻译](#机器翻译) 
  * [写作](#写作) 
  * [Chatbot](#Chatbot) 
  * [背景调查](#背景调查) 
  * [OCR](#OCR) 
  * [合同审查](#合同审查) 
  * [会话分析](#会话分析) 
  * [NLQ](#NLQ) 
  * [代码](#代码) 
  * [其他](#其他) 
* [视觉Vision](#视觉Vision) 
  * [图像综合](#图像综合) 
  * [视频](#视频) 
  * [创作工具](#创作工具) 
  * [图像压缩](#图像压缩) 
  * [物体渲染](#物体渲染) 
  * [形象生成](#形象生成) 
  * [无人零售](#无人零售) 
  * [安防](#安防) 
  * [测试](#测试) 
  * [医学影像](#医学影像) 
  * [其他](#其他) 
* [音频Audio](#音频Audio) 
  * [语音](#语音) 
  * [声纹识别](#声纹识别) 
  * [反欺诈](#反欺诈) 
  * [CRM](#CRM) 
  * [医药](#医药) 
  * [音乐](#音乐) 
* [搜索和推荐](#搜索和推荐) 
* [优化Optimization](#优化Optimization) 
  * [强化学习](#强化学习) 
  * [运筹优化](#运筹优化) 
* [场景AI](#场景AI) 
  * [人力](#人力) 
  * [RPA](#RPA) 
  * [工业检测](#工业检测) 
  * [智能运维](#智能运维) 
* [行业AI](#行业AI) 
  * [零售](#零售) 
  * [教育](#教育) 
  * [农业](#农业) 
  * [法律](#法律) 
  * [金融](#金融) 
  * [医疗](#医疗) 
  * [制药](#制药) 
  * [服装](#服装) 
  * [房地产](#房地产) 
  * [物流](#物流) 
  * [工业](#工业) 
* [安全](#安全) 
# AI基础设施Infrastructure
>## 异构加速器虚拟化
>>>* 趋动科技：数亿元人民币
>>>* #RunAI：$30M
>>>* #Deci AI：$9.1M
>## 准备
>>### 数据处理与发现
>>>* Trifacta：$100M
>>>* #explorium：$31M
>>### 数据合成
>>>* Tonic.ai：$35M
>>>* #DataGen Technologies：$18.5M
>>>* Ai.reverie：$5.6M
>>### 数据标注
>>>* Scale AI：$325M，估值$7B 
>>>* Hive.ai：$50M，估值$2B
>>>* ！Snorkel AI：$85M，估值$1B
>>>* LabelBox：$40M
>>>* Kili Technology：$25M
>>>* SuperAnnotate：$14.5M
>>>* Cord：$12.5M
>>>* Super.ai：$12M
>>>* #Dataloop AI：$11M
>>>* 龙猫数据：3300万人民币
>>>* 爱数智慧: 数千万人民币
>>>* 倍赛科技BasicFinder：数千万人民币
>>>* 37度数据：千万级人民币
>>>* 曼孚科技MindFlow：千万级人民币
>>>* 星尘数据stardust：1000万人民币
>>### 数据质量
>>>* Aquarium：$2.6M
>>### 数据版本管理和托管
>>>* !Iterative.ai：$20M
>>>* !Pachyderm：$16M
>>>* 格物钛Graviti：千万级美元
>>>* Superb AI： $9.3M
>>>* Activeloop：$5M
>>### Feature Store
>>>* !Tecton：$35M
>>>* Rasgo：$20M
>>>* !Molecula：$17.6M
>>>* Kaskada：$8M	
>>>* !Logicalclocks：€1.3M
>## 构建
>>### IDE：
>>>* Hex Technologies：$16M
>>>* Observable: $10.5M
>>>* Noteable：$4.1M
>>>* Saturn Cloud：$4M
>>>* Deepnote：$3.8M
>>>* Count：$2.4M
>>>* Curvenote：CA$1.1M
>>### 深度学习框架
>>>* ！一流科技OneFlow：5000万人民币
>>### 训练管理
>>>* !Weights&Biases：$135M，估值$865M
>>>* 模型训练过程中的实验追踪、超参数优化以及模型和数据集版本管理
>>>* !Grid AI：$18.6M
>>>* !#Comet.ml：$13M
>>>* neptune.ai：$3M
>>>* Determined AI：被HPE收购
>>### 建模
>>>* DataRobot：$250M，估值$6B
>>>* Dataiku：$400M，估值$4.2B
>>>* !H2O.ai：$100M，估值$1.6B
>>>* Domino Data Lab：$100M
>>>* abacus.ai：$50M 
>>>* Pecan：$35M
>>>* Deci：$21M
>>>* RapidMiner：$16M  
>>>* Machinify：$10M
>>>* 第四范式：7亿美元，估值30亿美元
>>>* 九章云极DataCanvas：3亿人民币
>>>* 行动贝果：3443万人民币
>>>* 深度赋智：数千万人民币
>>>* 和鲸科技：数百万美元
>>>* 智易科技：数百万美元
>>>* 探智立方DarwinML：数百万美元
>>>* cnvrg.io被intel收购
>## 部署和监控
>>### 部署（狭义MLOps）
>>>* OctoML：$85M
>>>* !#iguazio：$24M
>>>* Spell：$15M
>>>* #Allegro.ai：$11M
>>>* Verta.ai：$10M
>>>* #SuperWise.ai：$4.5M
>>>* !Seldon：£7.1
>>>* #DAGsHub：$3M
>>>* Valohai：$1.8M
>>>* Datatron：$1.4M
>>>* 开放智能Open AI LAB
>>>* BentoML.ai
>>>* #ParallelM：被DataRobot收购
>>>* Algorithmia：被DataRobot收购
>>### 监控与可解释性
>>>* Fiddler AI：$32M
>>>* Arize AI：$19M
>>>* Arthur AI：$15M
>>>* #databand.ai：$14.5M
>>>* Truera：$12.2M
>>>* #Aporia：$5M
>>>* WhyLabs：$4M
>>>* 瑞莱智慧RealAI：数千万人民币
>>### 数据应用构建
>>>* Streamlit：$35M
>## 安全与隐私
>>>* Robust Intelligence：$30M
>>>* 瑞莱智慧RealAI：数千万人民币
>>>* #D-ID：$13.5M
>## NLP
>>>* !Hugging Face：$40M
>>>* !Rasa：$26M
>>>* Explosion AI：$6M
>## 向量搜索与数据库
>>>* !ZilliZ：4300万美元
>>>* ! 极纳科技Jina AI：3000万美元
>>>* Pinecone：$10M
>>>* Relevance AI：$3M
>>### 数据处理框架
>>>* Anyscale：$100M，估值$900M
>>>* Coiled：$21M
>>>* Akridata：$15M
>>>* Monolith AI：850万英镑
>>>* Elementl：$1.8Mi
>>>* ModelOp：$6M
>>>* Taktile: $4.7M
>>>* Akkio：$3M
>>>* 
# 文本NLP
>## NLP
>>>* primer.ai：$110M
>>>* mindee：$14M
>## 预训练模型
>>>* Cohere: $40M
>>>* 澜舟科技
>## 机器翻译
>>>* Unbabel：$60M
>>>* Lilt：$25M
>>>* 推文科技：1000万人民币
>>>* Atman：560万美元
>## 写作
>>>* Grammarly：$200M，估值$12.8B
>## Chatbot
>>### 智能客服
>>>* Ada Support：$130M，估值$1.1B
>>>* yellow.ai：$78.2M
>>>* cognigy：$44M
>>>* 图灵机器人：3.5亿人民币
>>>* 沃丰科技Udesk: 3亿人民币
>>>* 智齿科技：2亿人民币
>>>* 追一科技：数亿人民币，估值48亿人民币
>>>* 晓多科技：超2亿人民币
>>>* 硅基智能：数亿人民币
>>>* 乐言科技：数亿人民币
>>>* 微洱科技：数亿人民币
>>>* 云问科技：亿元级人民币
>>### 员工
>>>* Moveworks：$200M，估值$1.9B
>>>* Aisera：$40M
>>>* Espressive：$35M
>>### 心理健康
>>>* Woebot Labs：$22.8M 
>## 背景调查
>>>* Checkr $160M
>>>* Middesk $4M
>>>* i背调：数千万人民币
>## OCR
>>>* HyperScience：$80M
>>>* Eigen Technologies：$37M
>>>* Cinnamon AI：$13M
>## 合同审查
>>>* Kira systems：CA$65M
>>>* Lexion:$11M
>## 会话分析
>>>* #Gong.io：$250M, 估值$7B
>>>* Clari：$150M，估值$1.5B
>>>* People.ai：$100M，估值$1B
>>>* Cresta：$50M
>>>* #chorus.ai：$5.57B被收购
>>>* Vivun：$35M
>>>* Tact.AI：$27M
>>>* Remesh：$25M
>>>* Troops.ai：$12M
>>>* Polyai：$12M
>>>* 客知音：千万级人民币
>>>* 深维智信：350万美元
>>>* 循环智能
>## NLQ
>>>* ThoughtSpot: $100M，估值$4.1B
>>>* MagicBI：数百万美元
>>>* 北极数据：2000万人民币
>## 代码
>>>* Kite: $17M
>>>* Tabnine：$12M
>## 其他
>>>* 达观数据 2.7亿人民币
>>>* #A21 labs
>>>* Golden $14.5M
>>>* ClearGraph 被TABLEAU收购
>>>* UpCodes $3.4M
# 视觉Vision
>## 图像综合
>>>* 商汤：已上市，IPO估值130亿美元
>>>* 旷世：7.5亿美元
>>>* 依图：2亿美元
>>>* 云从：18亿人民币
>>>* 图普科技：千万美元
>>>* 极视角：
>## 视频
>>### 综合
>>>* Viedeo++
>>>* 影普科技
>>>* Kapwing
>>### 视频异常分析
>>>* 闪马智能 近亿元人民币
>>### 视频广告
>>>* #KERV Interactive $11M
>>### 视频录制
>>>* Loom $28.8M
>>>*  $26M
>## 创作工具
>>>* Canva $60M, $8.7B
>>>* Figma $50M,$2B 
>>>* InVisionApp $115M, $1.9B
>>>* Runway $8.5M
>>>* Beautiful.AI $11M
>>>* GliaCloud
>>>* 来画视频 5000万人民币
>>### 漫画
>## 图像压缩
>>>* 图鸭科技 数千万人民币
>## 物体渲染
>>>* 酷家乐 超1亿美元
>>>* 粒界科技 数千万美元
>>>* 凌迪科技 2亿人民币
>>>* 51world 2.1亿人民币
>>>* 叠境数字 亿元级人民币
>>>* 时谛智能 近亿人民币
>>>* 深尚科技 600万美元
>>>* 商询科技 datamesh
>## 形象生成
>>>* 魔珐科技Xmov 数亿人民币
>>>* 相芯科技 1.2亿人民币
>>>* 诺亦腾 数千万美元
>>>* 迈吉客科技 数千万人民币
>>>* 诗云科技 数百万美金
>>>* ZMO.ai
>>>* 像素偏移
>>>* 慧夜科技
>>>* 我是大咖
>>>* Brud $20M, $125M
>>>* Synthesia：$12.5M
>>>* #D-ID：$13.5M
>>>* Reface.ai：
>>>* Avararify
>>>* FaceRig：$2M
>>>* Rosebud AI：$1.5M
>>>* EmbodyMe
>>>* ROSEBUD.AI $1.5M
>## 无人零售
>>>* Standard Cognition：$150M
>>>* Grabango：$39M
>>>* Accel Robotics：$30M
>>>* Mad Street Den：$17M
>## 安防
>>>* Verkada：$80M
>>>* tractable.ai：$60M
>>>* #AnyVision：$43M
>>>* Intenseye：$25M
>## 测试
>>>* #Applitools $31M
>## 医学影像
>>>* 连心医疗：9000万人民币
>## 其他
>>>* Urbint：$60M
>>>* Akasha Imaging
>>>* 墨奇科技
# 音频Audio
>## 语音
>>>* verbit.ai：$150M，估值$1.9B
>>>* 思必驰：数亿人民币
>>>* 云知声：6亿人民币
>>>* Observe.AI：$54M
>>>* Otter.ai：$50M
>>>* Descript：$30M
>>>* DeepGram：$25M
>>>* Fireflies.ai：$14M
>>>* 魔音助手 
>## 声纹识别
>>>* 声扬科技VoiceAI 近亿人民币
>>>* SpeakIn
>## 反欺诈
>>>* Pindrop $90M
>## CRM
>>### Troops.ai
>## 医药
>>>* Suki $20M
>## 音乐
>>>* Amper Music $4M
>>>* StepBeats 150万人民币
>>>* 时域科技
# 搜索和推荐
>>>* Coveo：CA$227M
>>>* Attentive：$230M
>>>* Outlier：$22.1M
>>>* Lily AI：$12.5M
# 优化Optimization
>## 强化学习
>>### 游戏
>>>* DeepMind
>>>* 超参数科技：3000万美元
>>>* 启元世界：数千万人民币
>>>* rct studio：超千万美元
>>### 调度
>>>* secondmind.ai $24M
>>### 测试
>>>* Mabl：$40M
>>>* Test.ai：$11M
>>>* Testim：$10M
>>### 其他
>>>* 南栖仙策
>## 运筹优化
>>>* 杉树科技 近亿元人民币
>>>* 悠桦林 近亿人民币
>>>* 宾通智能 6000万人民币
>>>* 智因科技 
>>>* nextMV $8M
# 场景AI
>## 人力
>>>* Eightfold：$220M
>>>* Pymetrics：$40m
>>>* Turing.com：$32M
>>>* Truework：$30M
>>>* e成科技：8000万美元
>>>* Bello倍罗：数千万人民币
>>>* 近屿智能：数千万人民币
>>>* 方便面面试
>## RPA
>>>* Uiptah：$750M
>>>* Automation Anywhere：$290M
>>>* FortressIQ：$30M
>>>* skan.ai：$14M
>>>* 来也科技：4200万美元
>>>* 弘玑Cyclone：近4000万美元
>>>* 云扩科技：3000万美元
>>>* 影刀RPA
>## 工业检测
>>>* 深度视觉：数千万人民币
>>>* 深浅优视：数千万人民币
>## 智能运维
>>>* 擎创科技：千万级美元
>>>* 必示科技：1.5亿人民币
>>>* 云兴维智：数千万人民币
# 行业AI
>## 零售
>>>* Tekion：$250M
>>>* ImageDT图匠数据：千万级美元
>## 教育
>>>* 松鼠AI：10亿人民币
>## 农业
>>>* 极飞科技：12亿人民币
>>>* Hypersonix：$11.5M
>>>* 爱科农：
>## 法律
>>>* 幂律智能：6000万人民币
>>>* Ross Intelligence
>>>* Atrium LTS
>>>* DoNotPay：$10M
>>>* 秘塔
>## 金融
>>### 机器学习
>>>* Taktile：€6M
>>>* 山景智能
>>### 智能投顾/投研
>>>* Wealthfront $75M
>>>* Kensho $550M 收购
>>>* 香侬科技：1.1亿人民币
>>>* 虎博科技：3300万美元
>>>* 阿法金融
>>>* eBrain
>>>* 倍漾科技
>>>* 卡方科技
>>>* 弘量研究
>>>* 贝塔数据
>>### 风控
>>>* 同盾科技：1亿美金
>>>* Sift Science $53M
>>>* 慧安金科: 1亿人民币
>>>* DataVisor：4000万美元
>>>* Simility 1.2亿美金被收购
>>>* 新加坡的CashShield, GGV 2000万美元
>>>* #Forter：5000万美元
>>>* 巴黎的Shift Technology，6000万美元，accel
>>>* 英国的Featurespace, 3000万美元
>>>* Signifyd 1亿美元
>>>* SentiLink
>>>* UnifyID
>>>* Tessian $42M
>>>* Tara AI：$10M
>## 医疗
>>>* 连心医疗：9000万人名币
>>>* 麦歌算法
>## 制药
>>>* 晶泰科技：近4亿美元，估值超20亿美元
>>>* Owkin：10亿美元
>>>* 因明生物：5000万美元
>>>* 望石智慧：数千万美元
>>>* 星亢原：3000万美元
>>>* 宇道生物：2000万美元
>>>* 燧坤智能：1.5亿人民币
>>>* METiS：过亿元人民币
>>>* 费米子科技：上亿元
>>>* 智化科技：1500万美元
>>>* 未知君：超千万美元
>>>* 冰洲石AccutarBio：数千万美元
>>>* 星药科技：数千万美元
>>>* 希格生科：近千万美元
>>>* 英飞智药：近4000万人民币
>>>* 亿药科技：数百万人民币
>## 服装
>>>* 智布：1亿美元
>>>* 极睿科技：亿元级人民币
>>>* 时谛智能：近亿人民币
>## 房地产
>>>* Skyline AI
>## 物流
>>>* 快运兔
>## 工业
>>>* Augury：$180M
# 安全
