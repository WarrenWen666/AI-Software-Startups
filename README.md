
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
  * [异构加速和虚拟化](#异构加速和虚拟化) 
  * [准备](#准备) 
  * [构建](#构建) 
  * [部署和监控](#部署和监控) 
  * [NLP](#NLP) 
  * [向量搜索与数据库](#向量搜索与数据库) 
  * [安全与隐私](#安全与隐私) 
* [文本NLP](#文本NLP) 
  * [NLP](#NLP) 
  * [预训练模型](#预训练模型) 
  * [机器翻译](#机器翻译) 
  * [写作](#写作) 
  * [Chatbot](#Chatbot) 
  * [背景调查](#背景调查) 
  * [文档抽取](#文档抽取) 
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
* [图形Graph](#图形Graph) 
* [搜索和推荐](#搜索和推荐) 
* [优化Optimization](#优化Optimization) 
  * [强化学习](#强化学习) 
  * [运筹优化](#运筹优化) 
  * [研究 ](#研究 ) 
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
# AI基础设施Infrastructure
>## 异构加速和虚拟化
>>>* #RunAI：$75M
>>>* Exafunction：$25M
>>>* 趋动科技：数亿元人民币
>## 准备
>>### 数据收集与处理
>>>* #explorium：$75M
>>>* Trifacta：acquired by alteryx at $400M
>>### 数据合成
>>>* #DataGen Technologies：$50M
>>>* Tonic.ai：$35M
>>>* Ai.reverie：$5.6M
>>### 数据标注
>>>* Scale AI：$325M，估值$7B 
>>>* Hive.ai：$50M，估值$2B
>>>* ！Snorkel AI：$85M，估值$1B
>>>* LabelBox：$110M，估值$900M
>>>* Heartex：$25M
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
>>>* Superconductive：$40M
>>>* Aquarium：$2.6M
>>### 数据版本管理和托管
>>>* !Iterative.ai：$20M
>>>* !Pachyderm：$16M
>>>* 格物钛Graviti：千万级美元
>>>* Superb AI： $9.3M
>>>* Activeloop：$5M
>>### Feature Store
>>>* !Tecton：$100M
>>>* Rasgo：$20M
>>>* !Molecula：$17.6M
>>>* Continual：$15.7M
>>>* #Qwak：$15M
>>>* Kaskada：$8M	
>>>* !Logicalclocks：€5M
>## 构建
>>### IDE：
>>>* Hex Technologies：$52M
>>>* Observable：$35.6M
>>>* Noteable：$21M
>>>* Deepnote：$20M
>>>* Saturn Cloud：$4M
>>>* Count：$2.4M
>>>* Curvenote：CA$1.1M
>>>* 白海科技：数千万人民币
>>### 深度学习框架
>>>* ！一流科技OneFlow：5000万人民币
>>### 训练管理
>>>* Weights&Biases：$135M，估值$865M
>>>* #Comet.ml：$50M
>>>* !Lightning AI：$18.6M
>>>* neptune.ai：$8M
>>>* Determined AI：acquired by HPE
>>### 建模
>>>* DataRobot：$250M，估值$6B
>>>* Dataiku：$400M，估值$4.2B
>>>* !H2O.ai：$100M，估值$1.6B
>>>* Domino Data Lab：$100M
>>>* Pecan：$66M
>>>* abacus.ai：$50M 
>>>* RapidMiner：$16M  
>>>* 第四范式：7亿美元，估值30亿美元
>>>* 九章云极DataCanvas：3亿人民币
>>>* 行动贝果：3443万人民币
>>>* 深度赋智：数千万人民币
>>>* 宽邦科技BigQuant：千万级人民币
>>>* 和鲸科技：数百万美元
>>>* 智易科技：数百万美元
>>>* 探智立方DarwinML：acquired by 来也科技
>>>* cnvrg.io：acquired by intel
>## 部署和监控
>>### 部署
>>>* OctoML：$85M
>>>* Neural magic：$30M
>>>* !#iguazio：$24M
>>>* #Deci：$21M
>>>* Datatron：$12.1M
>>>* #Allegro.ai：$11M
>>>* Verta.ai：$10M
>>>* !Seldon：£7.1
>>>* #DAGsHub：$3M
>>>* Valohai：$1.8M
>>>* 开放智能Open AI LAB
>>>* CoCoPIE： 数千万人民币
>>>* BentoML
>>>* #ParallelM：acquired by DataRobot
>>>* Algorithmia：acquired by DataRobot
>>>* Spell：acquired by Reddit 
>>### 监控与可解释性
>>>* Arize AI：$38M
>>>* Fiddler AI：$32M
>>>* Truera：$25M
>>>* #Aporia：$25M
>>>* Arthur AI：$15M
>>>* WhyLabs：$10M
>>>* #SuperWise.ai：$4.5M
>>>* Evidently AI: $125K
>>>* 瑞莱智慧RealAI：数千万人民币
>>### Workflow Orchestration
>>>* Astronomer：$213M
>>>* Prefect：$32M
>>>* Elementl：$14M
>>>* Union.ai：$10M
>>>* Outrebounds:
>>### 数据应用构建
>>>* Streamlit：acquired by snowflake at $800M valuation
>## NLP
>>>* !Hugging Face：$100M,估值$2B
>>>* !Rasa：$26M
>>>* Explosion AI：$6M
>## 向量搜索与数据库
>>>* !ZilliZ：6000万美元
>>>* ! 极纳科技Jina AI：3000万美元
>>>* Pinecone：$28M
>>>* SeMI Technologies：$16M
>>>* Relevance AI：$3M
>>>* Qdrant：€2M
>## 安全与隐私
>>>* Robust Intelligence：$30M
>>>* 瑞莱智慧RealAI：数千万人民币
>>>* #D-ID：$13.5M
# 文本NLP
>## NLP
>>>* primer.ai：$110M
>>>* mindee：$14M
>## 预训练模型
>>>* Cohere：CA$159M
>>>* #AI21 Labs：$64M
>>>* 澜舟科技：近亿人民币
>## 机器翻译
>>>* Unbabel：$60M
>>>* Lilt：$55M
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
>## 文档抽取
>>>* Instabase：$105M，
>>>* HyperScience：$80M
>>>* Eigen Technologies：$37M
>>>* Cinnamon AI：$13M
>## 合同审查
>>>* Kira systems：CA$65M
>>>* Lexion:$11M
>## 会话分析
>>>* #Gong.io：$250M, 估值$7B
>>>* Clari：$225M，估值$2.4B
>>>* Cresta：$80M，估值$1.5B
>>>* People.ai：$100M，估值$1B
>>>* Vivun：$75M
>>>* Tact.AI：$27M
>>>* Remesh：$25M
>>>* Troops.ai：$12M
>>>* Polyai：$12M
>>>* #chorus.ai：acquired by zoominfo
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
>>>* 硅心科技aiXXcoder：数千万人民币
>## 其他
>>>* 达观数据 2.7亿人民币
>>>* Golden $14.5M
>>>* ClearGraph 被TABLEAU收购
>>>* UpCodes $3.4M
# 视觉Vision
>>>* 研究
>## 图像综合
>>>* 商汤：已上市，IPO估值130亿美元
>>>* 旷世：7.5亿美元
>>>* 依图：2亿美元
>>>* 云从：18亿人民币
>>>* 图普科技：千万美元
>>>* 极视角：
>## 视频
>>### 综合
>>>* 极链科技Viiideo++
>>>* 影普科技
>>>* Kapwing
>>### 视频异常分析
>>>* 闪马智能 近亿元人民币
>>### 视频广告
>>>* #KERV Interactive $11M
>>### 视频录制
>>>* Loom $28.8M
>>>*  $26M
>>>* Runwayml: $35M
>## 创作工具
>>>* Canva $60M, $8.7B
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
>>>* Synthesia：$12.5M
>>>* #D-ID：$13.5M
>>>* Reface.ai：$5.5M
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
>>>* 墨奇科技：2.5亿人民币
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
# 图形Graph
>>>* RelationalAI：$122M
>>>* Katana Graph: $28.5M
>>>* Kumo.AI：$18.5M
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
>## 研究 
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
>>>* CognitOps: 1100万美元

## Contributors
<a href="https://github.com/WarrenWen666/AI-Software-Startups/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=WarrenWen666/AI-Software-Startups" />
</a>

Made with [contrib.rocks](https://contrib.rocks).
