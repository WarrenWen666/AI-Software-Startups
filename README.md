Last login: Fri Mar  5 12:12:52 on console
wentingcan@wentingcandeMacBook-Pro ~ % pip install docx
zsh: command not found: pip
wentingcan@wentingcandeMacBook-Pro ~ % pip3 install docx
Collecting docx
  Downloading docx-0.2.4.tar.gz (54 kB)
     |████████████████████████████████| 54 kB 281 kB/s 
Collecting Pillow>=2.0
  Downloading Pillow-8.1.1-cp39-cp39-macosx_10_10_x86_64.whl (2.2 MB)
     |████████████████████████████████| 2.2 MB 50 kB/s 
Collecting lxml
  Downloading lxml-4.6.2-cp39-cp39-macosx_10_9_x86_64.whl (4.6 MB)
     |████████████████████████████████| 4.6 MB 20 kB/s 
Building wheels for collected packages: docx
  Building wheel for docx (setup.py) ... done
  Created wheel for docx: filename=docx-0.2.4-py3-none-any.whl size=53925 sha256=506ce23212eecb274cead9d56eb5913aa05859d0c2fc4674f0f7a38934bc591a
  Stored in directory: /Users/wentingcan/Library/Caches/pip/wheels/0f/8e/9d/7003eed35a84cf960876aae6bdf60d02041ddfcca66eceee94
Successfully built docx
Installing collected packages: Pillow, lxml, docx
ERROR: Could not install packages due to an EnvironmentError: [Errno 13] Permission denied: '/usr/local/docx-template'
Consider using the `--user` option or check the permissions.

WARNING: You are using pip version 20.3.3; however, version 21.0.1 is available.
You should consider upgrading via the '/usr/local/opt/python@3.9/bin/python3.9 -m pip install --upgrade pip' command.
wentingcan@wentingcandeMacBook-Pro ~ % sudo pip3 install docx
Password:
WARNING: The directory '/Users/wentingcan/Library/Caches/pip' or its parent directory is not owned or is not writable by the current user. The cache has been disabled. Check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Requirement already satisfied: docx in /usr/local/lib/python3.9/site-packages (0.2.4)
Requirement already satisfied: Pillow>=2.0 in /usr/local/lib/python3.9/site-packages (from docx) (8.1.1)
Requirement already satisfied: lxml in /usr/local/lib/python3.9/site-packages (from docx) (4.6.2)
WARNING: You are using pip version 20.3.3; however, version 21.0.1 is available.
You should consider upgrading via the '/usr/local/opt/python@3.9/bin/python3.9 -m pip install --upgrade pip' command.
wentingcan@wentingcandeMacBook-Pro ~ % ls   
Applications		Library			Public
Desktop			Movies			WeDrive
Documents		Music			apache-maven-3.6.3
Downloads		Pictures		许可.pdf
IdeaProjects		Postman			耀途资本
wentingcan@wentingcandeMacBook-Pro ~ % cd Desktop 
wentingcan@wentingcandeMacBook-Pro Desktop % cd testCode 
wentingcan@wentingcandeMacBook-Pro testCode % ls
processAIdoc.py		starAnalysis.py		visual.svg
python_repos.svg	starAnalysis2.py
star.py			test.py
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py 
\Traceback (most recent call last):
  File "/Users/wentingcan/Desktop/testCode/processAIdoc.py", line 1, in <module>
    from docx import Document
  File "/usr/local/lib/python3.9/site-packages/docx.py", line 30, in <module>
    from exceptions import PendingDeprecationWarning
ModuleNotFoundError: No module named 'exceptions'
wentingcan@wentingcandeMacBook-Pro testCode % sudo pip3 install docx
WARNING: The directory '/Users/wentingcan/Library/Caches/pip' or its parent directory is not owned or is not writable by the current user. The cache has been disabled. Check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Requirement already satisfied: docx in /usr/local/lib/python3.9/site-packages (0.2.4)
Requirement already satisfied: Pillow>=2.0 in /usr/local/lib/python3.9/site-packages (from docx) (8.1.1)
Requirement already satisfied: lxml in /usr/local/lib/python3.9/site-packages (from docx) (4.6.2)
WARNING: You are using pip version 20.3.3; however, version 21.0.1 is available.
You should consider upgrading via the '/usr/local/opt/python@3.9/bin/python3.9 -m pip install --upgrade pip' command.
wentingcan@wentingcandeMacBook-Pro testCode % sudo pip3 install python-docx
WARNING: The directory '/Users/wentingcan/Library/Caches/pip' or its parent directory is not owned or is not writable by the current user. The cache has been disabled. Check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Collecting python-docx
  Downloading python-docx-0.8.10.tar.gz (5.5 MB)
     |████████████████████████████████| 5.5 MB 721 kB/s 
Requirement already satisfied: lxml>=2.3.2 in /usr/local/lib/python3.9/site-packages (from python-docx) (4.6.2)
Building wheels for collected packages: python-docx
  Building wheel for python-docx (setup.py) ... done
  Created wheel for python-docx: filename=python_docx-0.8.10-py3-none-any.whl size=184489 sha256=a647a106220471f56af4f790e3f57c596ac37915bb65d66b7b80a08882542382
  Stored in directory: /private/tmp/pip-ephem-wheel-cache-b848ap0q/wheels/d0/9f/b0/6c97fe84397519cce28035e638c5f2dac3409ba2df7c62d242
Successfully built python-docx
Installing collected packages: python-docx
Successfully installed python-docx-0.8.10
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py       
Traceback (most recent call last):
  File "/Users/wentingcan/Desktop/testCode/processAIdoc.py", line 2, in <module>
    doc=Document("./a.docx")
  File "/usr/local/lib/python3.9/site-packages/docx/api.py", line 25, in Document
    document_part = Package.open(docx).main_document_part
  File "/usr/local/lib/python3.9/site-packages/docx/opc/package.py", line 128, in open
    pkg_reader = PackageReader.from_file(pkg_file)
  File "/usr/local/lib/python3.9/site-packages/docx/opc/pkgreader.py", line 32, in from_file
    phys_reader = PhysPkgReader(pkg_file)
  File "/usr/local/lib/python3.9/site-packages/docx/opc/phys_pkg.py", line 30, in __new__
    raise PackageNotFoundError(
docx.opc.exceptions.PackageNotFoundError: Package not found at './a.docx'
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
符号
不包括自动驾驶、芯片、机器人、金融和医药的AI
#代表以色列公司
*代表中国
%表示战略投资

















































数据隐私、合规

BigID $70M
以色列特拉维夫的数据隐私保护公司
BigID成立于2016年，其研发的平台采用机器学习来自动化流程，让企业可以找到保存在其服务器和数据库中的敏感数据，以降低违规风险并确保其符合欧盟刚刚推出的GDPR 数据保护条例。对于那些可能为成千上万的客户提供大量数据的大企业而言，BigID可以更轻松地发现危险的或其他未编目的数据，并将其自动与用户身份关联起来。

OneTrust $300M
Druva $130M
Privitar $80M
Ethyca $13.5M

InCountry $18M
 data-residency-as-a-service platform.
InCountry provides a SaaS platform that securely stores, processes, and regulates profile data in its country of origin allowing multinationals to scale by providing integration.
The introduction of InCountry Border will provide a suite of new features to further secure and streamline the storage and processing of protected data, including:
– Localized encryption,
– High availability in highly-regulated countries,
– Integrates without coding.




Text IQ $12.6M

 $5M
WireWheel $20M
concentric.ai $7.5M
隐私计算
多方安全计算MPC
华控清交
芯片
星云Clustar
#Duality Technologies
联邦学习：
微众银行
蚂蚁金服
平安银行

数据库
向量数据库
ZilliZ milvus
Jina 600万美元
Pinecone

tecton.ai
时间序列
Influxdb $60M

Timescale $15M
涛思TDengine 超1000万美元
Graph
TigerGraph 1.05亿美元
欧若数网 Nebula 近千万美元
DGraph $11.5M
NoSQL
#ScyllaDB
ScyllaDB 是用 C++ 重写的 Cassandra，每节点每秒处理 100 万 TPS。ScyllaDB 完全兼容 Apache Cassandra，拥有比 Cassandra 多 10x 倍的吞吐量，降低了延迟
MongoDB
内存数据库
MemSQL 
Relation
新数科技
巨杉数据库
Pingcap
CockroachDB
Rockset

AI infra
个人总结：

AI有一个有趣的现象，每年大量的paper发出来，很多算法长期难以保持State of the art。显然算法就不能成为一家公司成为壁垒。难么一家公司的壁垒是什么呢？
一数据壁垒：
二工程壁垒：
三产品壁垒：

易用性

很多算法工程师的技术栈都是围绕着技术展开的。
很多算法工程师的现状就是， 赵论文和github对应的代码。
而一篇论文的算法代码，包括了模型训练的代码和数据清洗和处理。
模型的训练代码。

现在看到市面上，看到比较大的AI创业公司，无论是CV四小龙，还是做NLP的公司，都是从应用侧解决问题的。

但是另外一些公司提供了新的思路。
Rasa把chatbot进行了沉淀。
HuggingFace借助了基于transformer的预训练模型的东风，迅速增长
Jina提供了An easier way to build neural search on the cloud
Grid AI的，算法本身的是不断变化的，但是模型的训练和调试代码是相对固定的。

机器学习平台，又从切入的MLops，也有从AutoML切入的。
MLops指的是为了解决算法工程师和软件工程师是两拨人的，AI模型训练和AI的部署的割裂的问题。
AutoML从技术角度来说，是减轻算法工程师的工程量。从商业的角度来说，是降低了AI的标准化。



Rasa $26M
an open source machine learning framework to automate text-and voice-based conversations. With Rasa, you can build contextual assistants

投资人：
由Accel领投的A轮融资中获得了1300万美元的投资，Basis Set Ventures、OpenAI联合创始人兼主席Greg Brockman、UiPath首席执行官Daniel Dines和Hashicorp创始人Mitchell Hashimoto跟投。

客户：包括Circle Medical、T-Mobile、MoneyLion、宝马、瑞士保险公司Helvetia、Allianz、空客、丰田、女性健康机器人初创公司Tia以及美国十大银行中的五家

“自动化是企业的下一个战场，虽然这是一个很难取胜的领域，尤其是对于文本和语音等非结构化信息，但鉴于开发人员对它们的采用给人留下深刻印象，我们相信Rasa能够容纳一切，”Accel合伙人Andrei Brasoveanu说。“现有的解决方案不能让内部开发团队控制自己的自动化命运。Rasa正在为人工智能环境应用商业开源软件解决方案，类似于Cloudera、Mulesoft和Hashicorp等开源领导者所做的事情。”


Weidauer表示：“这里有大量的ML研究，但是开发者没有时间阅读所有的研究资料。但这就是我们公司所做的事情。我们将最新最好的研究录入并发布到一个可以随时运行、没有内存限制的图书馆。”

Grid AI $18.6M
The lightweight PyTorch wrapper for high-performance AI research. Scale your models, not the boilerplate.
Hugging Face $15M
Build, train and deploy state of the art models powered by the reference open source in NLP.





cnvrg.io 被intel收购
软硬件优化
OctoML $15M
TVM 是一个端到端优化堆栈，该端到端优化编译器堆栈可降低和调整深度学习工作负载，以适应多种硬件后端。TVM 的设计目的是分离算法描述、调度和硬件接口。该原则受到 Halide 的计算／调度分离思想的启发，而且通过将调度与目标硬件内部函数分开而进行了扩展。这一额外分离使支持新型专用加速器及其对应新型内部函数成为可能。TVM 具备两个优化层：计算图优化层和新型调度基元的张量优化层。通过结合这两种优化层，TVM 从大部分深度学习框架中获取模型描述，执行高级和低级优化，生成特定硬件的后端优化代码，如树莓派、GPU 和基于 FPGA 的专用加速器。
OctoML 拥有当前最先进的 AI、系统、编程语言、编译器和架构技术，可以让机器学习系统的优化和部署变得更加容易。该公司致力于打造一个可扩展、开放、中立的端到端栈，用于深度学习模型的优化和部署。


Neural magic $15M



CEO Shavit表示：“ Neural Magic证明了深度学习模型的高性能执行是…一个系统工程问题，可以用正确的软件算法解决。”

此版本的Neural Magic产品面向实时推荐和计算机视觉系统，
前者通常在生产中受到少量图形芯片内存的限制。通过运行通常具有更多可用内存的现成处理器来运行模型，数据科学家可以用最少的工作量来实现加速。
对于计算机视觉模型，Shavit声称Neural Magic的解决方案以“图形芯片速度”执行诸如图像分类和对象检测之类的任务，从而可以通过容器化应用在较大的图像和视频流上执行。





Weka.IO $31.7M
Weka.IO是一家AI深度学习及技术问题解决商，旨在解决AI深度学习和技术计算中的性能挑战。WekaIO的旗舰产品Matrix通过以低成本或传统NAS提供最高性能，最低延迟的存储，超越传统存储基础架构。WekaIO的软件在本地数据中心和公共云之间提供无缝混合云解决方案。WekaIO在多个高性能市场拥有客户，包括自动车辆AI培训，基因组学，财务建模，EDA，软件开发，卫星成像以及媒体和娱乐。


GPU虚拟化
趋动科技
#RunAI 
#bitfusion
数据处理与发现
Trifacta $100M
是一种提供数据分析服务的平台，负责分析非结构化数据预处理
# $31M
数据合成
Ai.reverie: $5.6M
#DataGen Technologies $3.5M
creating customized photorealistic synthetic visual data to train neural networks
We create high-quality labeled 2D, 2.5D, 3D and 4D visual datasets, with a perfect detection, segmentation, classification, 3D regression Ground Truth.
人脸生成


数据标注


Scale.ai :$155M 
Labelbox: $40M
#Dataloop AI $11M
Snorkel AI: $12M

向量搜索与数据库
ZilliZ milvus 4300万美元
Jina AI 600万美元
An easier way to build neural search on the cloud      
Jina is a deep learning-powered search framework for building cross-/multi-modal search systems (e.g. text, images, video, audio) on the cloud.
Pinecone $10M

深度学习框架
一流科技：OneFlow 5000万人民币
Skymind:DL4J
Experiment Tracking:
Weights&Biases：4500万美元
模型训练过程中的实验追踪、超参数优化以及模型和数据集版本管理


目的：增加AI训练时候的团队和合作，和透明程度。如果Github是共享代码的平台，那么AI ops 就是共享AI模型训练的代码，参数，实验结果的平台,GPU和内存的使用率等。可以做团队的对比和合作。模型效果可视化。团队之间的transparency

OpenAI的体验https://www.youtube.com/watch?v=0BU58W85KqU


机器学习平台
DataRobot: $270M 
Dataiku：$100M
H2O.ai：$72.5M
domino data：$43M
abacus.ai $22M 

AI as a service
Bias an Explainability 
NAS

产品
 
RapidMiner：$16M
Machinify：$10M
第四范式：7亿美元
和鲸科技 数百万美元
AutoML










星环科技 5亿人民币
行动贝果 3443万人民币

探智立方 DarwinML 数百万美元
江苏鸿程
#Allegro.AI: $11M
深度学习AUTO ML 和ML Ops



大公司
微软NNI
亚马逊AutoGluon
谷歌


MLops


Experiment
Feature Store
Deploy
Scale
Manage the ML life cycle



Saagie €25M
Algorithmia: $25M



#iguazio $24M
https://www.youtube.com/watch?v=MlnMnl1BFBw

Determined AI：$11M




Spell $15M
Verta $10M
Fiddler Labs $10.2M
Pecan $11M
Allegro.ai  $11M
#SuperWise $4.5M
AI Assurance - keeping an eye on your AI; AI performance management; AI monitoring
#Comet.ml $4.5



datatron $1.4M
痛点：模型部署，data scientist 到engineer，different enviroment
客户：很多银行SAS 换成 tensorflow，有了datatron 不用重建，都可以移植到datatron







Seldon £7.1
Open-source platform for rapidly deploying machine learning models on Kubernetes

Open source machine learning deployment
Manage, serve and scale models built in any framework on Kubernetes.
Take your ML projects from POC to production.

Evidently ai
#ParallelM 被DataRobot收购
machine learning model management, deployment and monitoring platform, in a move to give users more control over their AI lifecycles.

H2O.ai


Feature Store:
Tecton：$35M
The Enterprise Feature Store for Machine Learning
Build a library of great features. Serve them in production. Do it at scale
model monitoring
Arthur AI $15M


databand.ai $14.5M


WhyLabs $4M


Feature Discovery
#explorium $31M
Automated Data and Feature Discovery



向量搜索
Zilliz
As an open source vector similarity search engine, Milvus is easy-to-use, highly reliable, scalable, robust, and blazing fast. 
Pinecone
tecton.ai
数据版本和共享社区
Pachyderm $16M
Graviti 千万级美元
# DAGsHub $3M
which is built on top of the open source project .

和鲸科技

安全
Robust Intelligence $11M
RealAI

可解释性
开源项目
Lime
SHARP
Fiddler labs $10.2M





InterpretML
RealAI
当前AI技术对训练数据过分依赖，这导致算法在工业领域等样本和标注不足的场景中极易出错；
其次模型可解释性不强，在医疗、金融决策等敏感领域难以被广泛接受，张钹院士曾举例“比如医学图像识别，计算机识别率能够超过人类，但是医生不敢用，因为机器判断这张图片是有癌症，医生根本不知道它根据什么判断出来的，这是普遍遇到的问题”；
另外模型安全性差，通过对输入样本进行人类无法分辨的简单修改，就可以误导神经网络给出错误结果

 “珠算（ZhuSuan）”概率编程库，大幅降低了开发贝叶斯深度学习算法的技术门槛与成本；
并实现基于贝叶斯深度学习算法的半监督学习与无监督学习，大大减少实际场景中需要的标注数量；
团队在AI安全和可解释等方面也取得了令人瞩目的成果，通过对模型的可解释性进行建模，能够实现对模型决策的解释，让模型更加安全可靠。
#Aporia


隐私
#DID
边缘AI
开放智能
一个算法1.5
#Deci AI $9.1M

NLP
综合
达观数据 2.7亿人民币
机器翻译
Unbabel：众包 $60M
Lilt $25M

*推文科技：网络小说翻译 1000万人民币 联想之星
*Atman：医药文献翻译 560万美元 北极光
文本重写
Grammarly $90M
Chatbot
Automated CX
Ada Support $44M
智能客服
追一科技 4100万美元
智齿科技 2.1亿人民币
晓多科技 超2亿人民币
乐言科技 1.5亿人民币

心理健康
Woebot Labs  $22.8M 心理健康聊天机器人
运维
Moveworks $75M
companies can completely eliminate the need for IT staff to work on tasks such as provisioning applications, resetting passwords, unlocking accounts, managing email lists, and answering questions so they can focus on high-value activities.
The platform is already deployed and endorsed by CIOs at Fortune 500 and leading enterprise companies such as Autodesk, Broadcom, and Nutanix.
Customer including Broadcom, Western Digital, Medallia, Autodesk and Nutanix Align Technology, LinkedIn, Symantec, Belkin, Stitch Fix, AppDynamics and more.
其他
Troops.ai $12M


背景调查
Checkr $160M
Middesk创始人创业
Middesk $4M
i背调：数千万人民币
招聘
Eightfold $125M
Turing.com $32M
e成科技 8000万美元
Bello倍罗 数千万人民币
近屿智能 数千万人民币
方便面面试
Pyxai $150K
合同审查
Kira systems CA$65M
销售
第一，AI赋能Sales，从上图中我们可以清晰的看到AI赋能的效果。AI赋能有一定门槛，一是和底层的平台例如CDP、CRM的集成能力；二是AI的能力，比如对文本语音进行识别和分析、对话机器人、知识图谱等；三是对销售行业的理解。
列举几个典型公司：用人工智能挖掘销售线索的Zoominfo、实现销售流程自动化的People.ai、用人工智能帮助销售分析话术，提高谈判技巧的Gong.io和Chorus.ai、用人工智能帮助销售改善与潜在买家对话方式的Highspot、Seismic和Showpad。


列举几个典型公司：
用人工智能挖掘销售线索的Zoominfo、100亿
实现销售流程自动化的People.ai、
用人工智能帮助销售分析话术，提高谈判技巧的Gong.io和Chorus.ai、
用人工智能帮助销售改善与潜在买家对话方式的Highspot、Seismic和Showpad。

AI赋能Sales，从上图中我们可以清晰的看到AI赋能的效果。AI赋能有一定门槛，一是和底层的平台例如CDP、CRM的集成能力；
AI的能力，比如对文本语音进行识别和分析、对话机器人、知识图谱等；
是对销售行业的理解。
列举几个典型公司：
用人工智能挖掘销售线索的Zoominfo、
实现销售流程自动化的People.ai、
用人工智能帮助销售分析话术，提高谈判技巧的Gong.io和Chorus.ai、
用人工智能帮助销售改善与潜在买家对话方式的Highspot、Seismic和Showpad。
#Gong.io
#chorus.ai
People.ai
Troops.ai
Tact.AI 


Recurrent.ai
客知音
深维智信

Sales enablement
https://www.youtube.com/watch?v=472T-HuIehI

其他
# A21 labs
Israeli AI Research Company Led by Stanford Professor and MobileEye CEO Introduces Model to Solve Text Ambiguity


Golden $14.5M
ClearGraph 被收购
用自然语言替代SQL（结构化查询语言）查询，知识图谱的形式存储语义数据
2017 TABLEAU收购自然语言查询初创技术企业CLEARGRAPH  $33M
UpCodes $3.4M
OCR+搜索，实时更新建筑领域的法律

 consolidates regulations, inserts government commentary, provides a custom search engine, and offers team collaboration tools. According to McKinsey, construction is the second least productive industry in the US. But with access to UpCodes, construction companies will save time, prevent errors and reduce the overall cost of building.
They have grown to over 44,000 monthly active users, which include architects, engineers, building inspectors and homeowners. The founders of UpCodes are brothers Garrett Reynolds and Scott Reynolds. Prior to starting the company, Scott worked in architecture and Garrett worked as an engineer at PlanGrid.            --------YC
在美国，除了通用性建筑法规，各地方可能还会有自己的法规，并且会一直在更新。对于建筑师来说，需要整合不同的法规并紧密跟踪更新法规，即使是最勤奋的建筑师团队也经常犯错。在最坏情况下，一个错误的代价可能是数千甚至数百万美元。据麦肯锡和全美住宅建筑商协会的研究表明，遵守法规的复杂性是造成建筑业生产力下降和房价上涨的主要原因。

“在线法规库”是将建筑规范相关的书籍、PDF和在线资源整合到一个数据库中，用户可以通过电脑、手机等随时查看和搜索法规。UpCodes会实时更新跟踪这些法规的更新，并支持用户团队共同标记和研究。截止到2017年，UpCodes已经处理了超过11万次搜索。




Vision
技术路线
Neural rendering
NPR——non photorealistic render. 即非真实感图形学。
Cel-Shading 或者叫做 ToneBasedShading 即所谓的卡通渲染。

https://blog.csdn.net/wodownload2/article/details/89488347




综合
商汤
旷世
依图
云从
图普科技

动作捕捉
诺亦腾
Xmov




创作工具

Canva $60M, $8.7B
Canva让用户上手即用，设计零门槛时代要来了


adobe设计门槛高
们的愿景是，让设计平民化。




Figma $50M, $2B 
InVisionApp $115M, $1.9B
Runway $8.5M
Beautiful.AI $11M
人工智能驱动幻灯片设计平台
其特点和优势包括：
幻灯片自动设计。了解设计规则的 Beautiful.AI 应用启发式技术来构建实时响应内容的幻灯片。这些幻灯片会根据需要自动调整布局以确保视觉效果和一致性。动画。演示工具中的动画会让演示效果更有效，但因为创建的难度大，很多人不愿意去接触。借助Beautiful.AI，动画会以一种有意义且有影响力的方式自动应用于作品中。少即是多。对于演示来说，少即是多。通过限制每张幻灯片上的内容量，Beautiful.AI 为图像留下空间，以增强信息的影响力并保持观众的参与度。图片。Beautiful.AI 提供丰富的免版权费图像、图标和徽标，可供用户随时查找和搜索。这能让幻灯片在视觉上保持一致性，并帮助用户专注于内容创作而无需打开新标签、搜索网页、调整大小、剪切或粘贴图像。

GliaCloud
台湾
利用人工智能技术进行视频自动生产制作平台。公司研发了一套机器自动生产视频的系统GliaStudio ，目前主要针对新闻资讯，用户只需要输入文字内容或者链接，即可以自动生成剧本、抓取网络素材、生产短视频。

来画视频 5000万人民币
漫画
触漫 6000万人民币



图像压缩
图鸭科技 数千万人民币
TNG 采用了深度学习卷积网络（CNN）的编码方式，与 JPEG 相比，压缩率提升了 122%；与 WebP 相比，压缩率提高了 30%。而且相比 BPG/HEIF 等图片格式，TNG 采用了 CNN 技术而非 HEVC 编解码器，在保证图片质量的同时，避免了高昂的专利费用。


渲染

个人总结：
代码的复用：
业务的复用：业务中台
动作的复用：？？

VR：3D实时渲染

应用场景：
电影
动漫
游戏

人才
国外难找

然而，纵观MR产业链，从上游的设备研发制造，到中间的OS、渲染引擎，再到下游与产业结合的应用，均有环节亟待开发和完善，而这也恰恰是创业公司的机会。
光学成像
光学和OS系统是MR眼镜的两大核心技术，其中光学模组作为MR硬件的重要组成部分，其成本可占到整体眼镜的60%以上。
市面上主流光学模组主要采用棱镜、自由曲面、光波导、光场等方案。而对于人眼来说，具有较大视场角、轻薄体积的光波导技术则是最优方案。目前，光波导分为全息光波导和阵列光波导两种技术方案，其中微软、Waveoptics采用全息光波导；国内的珑景光电、灵犀微光以及以色列Lumus采用阵列光波导；仅有Magic Leap一家采用了多层叠加光波导。
对于光波导技术而言，目前的痛点有生产工艺复杂、量产难度高、良品率低，及成本过高（Lumus光学模组单价可达1000美金）。作为MR眼镜供应链上游的核心环节，光波导技术仍有较大的成长空间。
OS系统
软件层面，操作系统是MR的关键。对MR来说，操作系统要保证虚拟信息能够快速实时刷新，从而满足用户在真实环境中无延迟浏览虚拟信息的需求。目前，不少公司都基于Android开发OS，而由于Android的底层架构是基于手机系统研发的，因而刷新率较低，不能满足人眼诉求。因此，像Magic Leap、微软这类公司都在针对MR重写OS。
对于中国公司来说，市面上的操作系统均基于Android开发，无法满足MR眼镜对于事实性和低延迟性的要求，这一空白市场也尚待填充。
3D渲染引擎
无论是C端还是B端的MR内容开发都离不开3D渲染引擎。现有的3D渲染引擎是基于PC和移动手机端研发的，如果应用在MR眼镜端则无法做到实时，且并发热量高，耗电量大。迎合移动MR技术这一趋势，3D渲染引擎需要弱化现有引擎大而全的特点，做到轻量化、高实时性，强化交互性和渲染效果的真实性。
36氪曾报道过一家公司粒界科技，主攻下一代AR-Ready架构平台的渲染引擎GritGene，可支持实时大规模的场景渲染、交互，也可移植到可穿戴设备中（如未来的移动AR）,目前在影视制作、智慧城市领域均有所涉猎。


AR core：谷歌概念介绍https://developers.google.cn/ar/discover/supported-devices


动漫
总体来看，国内动画的爆发还是3D动画占据主流，主要是因为3D和2D的制作原理不一样。
一般来说，3D是在建模阶段最花时间。在模做好之后，一般就是一集一集用机器往后跑，所以只要分镜能够保证，制作周期不会耽误太久。而且3D动画的优势还在于不容易画风崩坏，同时可以支持较为复杂的材质和造型，比如绚丽的服饰等。
相比来说，2D动画的制作就要困难很多，它需要要一张一张的画，如果中间哪里出了问题，就得重新画一遍，这样制作周期就会拉长。并且，目前国内2D动画的人才非常紧缺，而且培养周期非常久。一般一个成熟的原画师，需要3-5年的培养才可以独当一面。

51world
北京五一视界数字孪生科技股份有限公司（51WORLD）是一家以计算机图形学为核心的数字孪生平台公司。公司以原创的全要素场景（AES）作为核心技术，融合物理模拟、工业仿真、人工智能、云计算及地理信息等技术进行持续的创新，帮助全球政府及企业进行新一轮数字化升级，并引领数字孪生成为新型基础设施。

51WORLD 通过 AES 建立数字孪生平台，实现多源时空数据融合，城市数字底座搭建，多元仿真模型模拟等应用价值。AES已被全球超千家大中型政府及企业广泛应用，辐射近 200 个城市和数十个行业。 公司产品主要赋能智慧城市、汽车及交通、智能制造、智慧水务、房地产等领域，在多行业市场占有率均为第一。其中，标杆项目包括雄安新区智能城市大数据平台、南京市江北新区智慧城市指挥中心、安徽铜陵城市超脑、一带一路中白工业园智慧园区、深圳数字孪生港口、航科院数字孪生机场、云南三湖智慧水务、中科院合肥物质研究院数字孪生工厂、华为深圳坂田总部智慧园区以及南京、重庆、济南、西安、贵州等国家级新区数字孪生平台。

公司在各大细分领域的客户和业务增长率均保持每年超过200%，已服务来自海内外近1000家企业客户，其中泛智慧类业务客户包括中国移动、中国联通、中国电信、华为、腾讯、阿里巴巴、商汤、科大讯飞、Facebook、盛裕控股集团（Surbana Jurong）等；自动驾驶仿真及交通仿真业务客户包括宝马、戴姆勒奔驰、广汽集团、威马汽车、国家智能网联汽车(上海)示范区、重庆车辆检测研究院等；数字地产业务则已触达90%以上全国Top100品牌房企，如万科、碧桂园、招商局集团、华润、中国铁建等。
目前公司超500人，其中研发人员硕博比例超过50%。公司的主要研发方向覆盖计算机图形学、计算力学、计算机视觉、车辆仿真、传感器仿真、交通和车联网仿真、强化学习、深度学习、离散数学、决策规划、分布式系统等十余项高科技类基础研究，研发人才主要来自清华大学、浙江大学、上海交通大学、中国科学院、康奈尔大学、伊利诺伊大学、佐治亚理工学院、微软亚洲研究院等高校和研究机构。

全要素场景（All Element Scene，简称AES）是51WORLD的核心产品。
AES是一种基于真实的地理信息，集合物理世界各种要素，
通过计算机实时渲染而生成的可交互三维仿真场景，可以广泛应用于需要场景数字孪生的全行业领域。
粒界科技
拥有经验丰富的人才是粒界引擎得以加速研发的关键。截至目前，粒界科技的80名员工来自17个国家，分布在德国法兰克福、上海和广州。其中，德国团队以研发为主，上海团队主要负责动漫内容的创作，不久前也成立了研发部，广州团队主要做智慧城市类的业务拓展。
团队构成如此“国际化”，主要是因为既精通游戏引擎研发，又具备非游戏领域经验的人才极度稀缺，吴小毛只能在全球范围内寻觅，终于组成这样一支顶级的“混血战队”。
“光是做游戏引擎研发的人就非常难找，上海研发部门最初的3个人我们找了非常久。” 吴小毛透露，“但我们一开始并没有去打造一款游戏引擎，我们缩减了模块，也无需像游戏引擎那样要兼容很多硬件，因此可以加快研发速度。”


叠境
RestAR
酷家乐
迈吉客科技


商询科技 datamesh
时谛智能


形象生成
从零开始的自制Vtuber

zhihu.com/people/hua-chuan-xie-hui/posts
Brud $20M $125M
a transmedia studio that creates digital character driven story worlds.

FaceRig $2M
EmbodyMe
Youtube

Xmov魔珐科技 数亿人民币
相芯科技 1.2亿人民币
迈吉客科技 数千万人民币
诗云科技 数百万美金
ZMO.ai
https://www.zmo.ai/zh/about-us/
像素偏移
慧夜科技
我是大咖

DID


中科深智


视频录制



演讲者可以更丰富的表达，加强注意力。人脸的表情，肢体语言
素材突出重点
结合两者
演讲者背景虚化


Loom

视频
Viedeo++
影普科技
Kapwing
视频编辑创作平台


视频异常分析
闪马智能
OCR
HyperScience $80M
OCR颠覆庞大且效率极低的数据输入市场
帮助大型公司和政府组织加快文书工作的处理过程
such works as data entry, invoice processing, and data reconciliation


视频广告
#KERV Interactive $11M
Interactive Video 
交互式视频广告平台
技术：语义分割 
客户


无人零售
Grabango
无人零售解决方案提供商

Standard Cognition
作为 Amazon Go 的挑战者，Standard Cognition 是第一家向存量零售商提供基于人工智能与计算机视觉的自动结算解决方案的公司，通过他们的技术，小零售商们能够低门槛实现技术升级，将自己的实体店转型为无人商店。
Amazon Go 的商店内安装了多许摄像头、3D 摄像头和传感器，但 Standard Cognition 表示零售商们只需要对自己的实体店进行轻量级的改造——将摄像头安装在天花板上，他们的系统便能够适配任何商品陈列布局方式。因此，现有的零售商们无需为接入 Standard Cognition 付出高昂的时间与经济成本。


Mad Street Den
产品Vue.ai是一个共服装零售商使用的人工智能和图像识别平台，这款产品既适合大型百货商店，也是用于线上平台。它可以提供数据分类和目录数据管理，包括基于AI的自动数据标记，包括属性，标题和描述，帮助企业改进产品发现和可搜索性

融资1亿美元
时尚
深尚科技
安防
#AnyVision  $43M
tractable.ai
Tractable is a software company that develops artificial intelligence for accident and disaster recovery.

视频异常
闪马智能：近亿元人民币
测试
#Applitools $31M
Intelligent Functional and Visual Testing Through Visual AI





医学影像
连心医疗：9000万人民币

其他
Akasha Imaging
墨奇科技
藏指纹识别解决方案提供商 


Audio/speech
音乐
Amper Music
一款基于AI的音乐作曲家，允许用户为其内容创建和自定义原创音乐，是全球首家人工智能编曲、表演和制作公司，使用户能够即时创作和定制原创音乐。

StepBeats
是一款通过跑步来创作音乐的App。一个运动创作音乐平台，搭建基于大量运动、生理体征和情感参数数据训练下的AI作曲模式，通过传感器实时对用户运动步频、动作、姿势进行智能分析，生成个性化节拍和音效，并且支持协同创作。未来将打造音乐IP，提供音乐版权化服务。

语音
Descript
团购网站 Groupon 前 CEO Andrew Mason

Descript的设计意图不仅仅转录音频。相反，它会将音频转录下来的文字放到Word文档中，然后编辑人员或音频制作人可以像修文档一样剪辑音频。比方说，如果你从文档中删除一个字，那么音频中的那个字也就被删除了；如果你在文档中增加一个字，那么音频中也会出现相应的那个字。

人听语音是慢的，但是阅读文字是很快的。

DeepGram
英伟达和YC投资。

输入文字转音素，以音搜音。Speech Recognition同音词如果错了，文本搜索不到

语音搜索。检索音频和视频文件中的语音信息的搜索引擎,搜索范畴包括通话、会议、播客、视频短片、演讲等。很多公司都有好几百万小时的通话记录，我们的搜索工具一定会有用武之地。

Deepgram的创始人曾在官方博文提到 “ 当处理一个巨大的文档语料库时，文本搜索只能在其中嵌入不同类型的数据，这是一个容易解决的问题，但通过录音进行搜索是非常困难的。按照传统的工作流程，通常将原始音频转录成文本再将其输入搜索工具，如果你使用人工进行转录，这真的是太费时费力了！而如果您尝试使用自动语音转文本，那么搜索的准确性就是问题。Deepgram在这些方面都做了修正和提升！”。

那么既然语音搜索这么难，DeepGram又是如何实现的呢？据了解，Deepgram主要是基于短语的声音搜索而不是文本中的精确拼写，从而产生相关的结果，与其他同类的语音搜索软件最大的不同是它可以通过不同的语境来区别不同的声音含义。因此，即使拼写错误Deepgram也可以找到它们。从使用流程上看，首先用户将音频文件上传到平台，如电话、播客、会议或视频甚至可以使用YouTube URL；然后平台会对语音进行“深度索引”处理，通过语音学来发声而不是尝试将声音翻译成单词；最后当用户输入搜索文字时，Deepgram就可以在索引中找到相关的结果。在这过程中，Deepgram通过深度学习的训练，实现了相比传统方式更快、更便宜及更便捷的突破提升。准确率方面，虽比不了人工的准确率水平，但Deepgram平均80%的准确率，相比更容易出错、20%准确率的语音转文本的搜索方式显然更好；响应速度方面，一旦索引，Deepgram只需要几秒钟就可以在其索引中找到您的搜索字词，并直接跳转到音频中提及的关键字的时间；成本方面，公司能够在不到一半的时间内将音频文件编入索引，相比行业价格每小时1.5美元的服务费，Deepgram每小时75美分的音频成本显然有着明显的优势

创业公司而言，基于语音识别技术大多运用于营销环节，如 Chorus.ai、TalkIQ、Gong.io等通过深度学习数据分析及预测帮助销售人员提高工作效率并提升业绩。而语音搜索方便比较相近的公司则有Voicebase，2010年成立于美国加利福尼亚，是一家提供录音存储服务，用户可以随时随地访问、搜索、查找录音相关内容并允许其他人分享及添加评论的初创公司。






Otter.ai $50M
魔音助手 5000万美元

思必驰：端侧
云知声：云


音频数据和视频数据的频次差别大


声纹识别
VoiceAI 
SpeakIn
反欺诈
Pindrop  $90M
（Google Capital领投）, 9000万美金
防电话欺诈，主要通过对来电的语音和相关数据分析来帮助企业用户辨别诈骗电话。
下一步，是开发客户服务之外的更多用途——目前客服是公司业务的主要来源——让所有具备语音界面的应用都用上Pindrop，包括联网车平台、居家安全设备、智能办公设备和智能音箱等。
Pindrop于2011年创立于亚特兰大，公司当前的主要业务是在客户服务的过程中，帮助预防语音欺诈。Pindrop表示，截止2018年，公司已经帮助避免了3.5亿美元的损失。目前美国规模最大的5家保险公司，以及排名前十的银行中有八家都是Pindrop的客户。

公司预计能于2019年第一季度实现盈利，并保持持续的增长，因为语音欺诈问题已经给相关领域带来了220亿美元的损失（其中140亿美元是欺诈导致的，还有80亿美元是安全问题引发的时间和系统资源浪费所导致的）。Pindrop表示，截止2018年，公司已经帮助避免了3.5亿美元的损失。目前美国规模最大的5家保险公司，以及排名前十的银行中有八家都是Pindrop的客户。

CRM
亚马逊、微软和 Salesforce 三巨头均看好语音交互

语音助手+CRM， 融资27milion

语音人机交互，因为销售人员需要开车四处见客户，要花费大量的时间在路上。
智能语音助手帮助销售人员快速查找信息，下达命令等。不仅能提供下一次会议的基本概要，还能提供交易细节和其他相关信息，为他们准备下一次更高效的会面。该创企一直试图改变销售人员使用语音与CRM系统中的信息进行交互的方式
Tact的创新主要体现在两方面，一方面是结合人工智能，让使用者可以更方便下指令；另一方面是打通了CRM和社交账号之间的数据。
Ganapathi对CRM工具局限性的理解可能比任何人都要好。这是因为在他创办Tact之前的20几年里，他一直在帮助建造这样的系统。他首先与Ernst and Young合作定制系统，然后与Siebel Systems进行了合作，最后与Salesforce使用云进行合作。
CRM的价值主张一直是它为公司提供了存储客户数据的中心位置。这虽然是一种电子格式，但输入和检索数据对繁忙的销售人员来说仍然是一件苦差事。Ganapathi于2012年推出了Tact，希望能够使用语音来帮助更轻松地与这些工具进行交互。战略投资者也认识到了销售人员语音界面的价值。
GGV

销售对话语音转录+CRM。客知音目前服务的客户主要来自教育、金融、企业服务行业。我们和国内的多家呼叫中心系统和CRM厂商开展了不同层面的合作，协力为销售客户提供最完整的解决方案。
目前平台拥有2款产品，一款是用以解放大量人工的语音机器人，一款是“销冠AI教练“，加快30%新人或者新产品的上手时间。
客知音提供云端和私有化部署，现已在互联网、保险、银行等金融领域和互联网教育场景落地。产品客单价在10万~100万之间，已有20多家客户，实现几百万营收。

Troops.ai
智能会话软件
长在slack之上


医药
Suki $20M
医用语音笔记助手研发商 
医生只需要在诊疗患者的时候大声说话，Suki就可以像医生助理一样进行记录，医生则无需将问询病史、记录病历这类工作亲自输入到医疗记录系统，或者完全手写记录。这一变革可以让医生更轻松地诊疗更多的患者，为医生提供了一种更高效的治疗方式，而并不妨碍医生和病人


个性化推荐
Attentive $230M
a personalized mobile messaging platform that helps e-commerce and retail brands connect with customers.
“CRM is changing,” Long said in a statement. “Businesses can’t build a relationship with the modern consumer through email alone. Email performance, as measured by how many subscribers click-through on a message, is down 45% over the last five years. Rather than continuing to shout one-way messages at consumers, smart brands will stay relevant by embracing personalized, real-time, two-way communication channels.”

Outlier $22.1M
Outlier正在试图解决一个存在已久的难题，那就是如何在用户不发问的情况下提供有价值的分析内容。使用传统的BI工具，用户在获得数据后必须提出问题，然后才能查看数据是否可以解决相关问题。而Outlier试图利用智能和自动化技术在不需要用户提出正确问题的情况下便给出准确的分析。

Lily $12.5M
人工智能时尚推荐平台


决策智能
研究 
运筹学
数学规划 (math programming)
优化 (optimization)、
最优化理论、
决策科学(Decision Science)

简单地说：凡是有“最”字，如：利润最大化、成本最小化，基本就和运筹学息息相关。
运筹学、数学规划（Math Programming）问题的数学表达式，由自变量（Variables）、目标函数（Objective Function）和约束条件（Constraints）组成，所有优化问题本质上都可以化简为由它们组成的数学表达式，然后求解满足约束条件下使得目标函数最大/小的变量的值。


分类：
数学规划有三个大类，
线性规划（LP），混合整数规划（MIPS），还有非线性规划（NLP）

约束规划和组合优化


4 Classification of optimization problem
(IP: integer programming,
MINLP: mixed integer non-linear programming,
MILP: mixed integer linear programming,
LP: linear programming,
QP: quadratic programming,
NLP: non-linear programming)




线性规划（Linear Programming）
当自变量是连续的，目标函数和不等式是线性的时候，该问题被称为线性规划问题。

整数规划（Integer Programming）问题
整数规划，或者离散优化（Discrete Optimization），是指数学规划问题中自变量存在整数。与线性规划连续的可行域不同，整数规划的可行域是离散的


另外，除了整数规划，还有混合整数规划（Mixed Integer Programming, MIP），即自变量既包含整数也有连续变量。



总结
决策智能主要分为三种技术路径：
强化学习（计算机流）
运筹优化（数学流）
量子计算（遥远）

运筹优化更适合解决调度问题，航班调度，物流调度，网络调度等
强化学习的本质最终的还是回到运筹学。
强化学习在调度优化问题上不一定比运筹优化的方法好。（待考证）
但是强化学习应该能用于调度优化以外的场景。

启元世界：从侧面看，我看启元世界2019年时候的官网上，还说要解决航班调度，物流调度，网络调度问题。今年都不强调优化调度场景了，而是更强调其他场景。比如AI博弈、AI陪练，虚拟玩家等。
南栖仙策：用在四个场景：制造、营销、物流、军事对抗
RCT：做智能NPC，剧情AI


运筹优化：
杉树核心优势是团队稀缺，线性求解器方面做到世界前列的水平。但是团队意识到只做求解器天花板低(如国外的gurobi)，所以这两年，开始做求解器之上的应用平台。估值较高
智因团队是英国伦敦大学硕士，之前在英国的公司做的事情。短期不做求解器，打采用国外的成熟的求解器，主要是做应用平台，他认为目前是调度优化是蓝海市场，遇到的竞争者都是传统用启发式算法的厂商，拿单容易，号称遇到一单拿一单，还没有达到碰到杉树的程度。天使轮，估值便宜。



强化学习
综合
启元世界

南栖仙策
为什么说“智能决策”将拉开商业变革大幕？ | 甲子光年

游戏
%DeepMind
超参数科技
启元世界

启元世界目前对哪些行业场景的关注比较多？成果如何？未来还计划覆盖哪些行业场景？
袁泉：我们关注的主要是游戏、网络智能和仿真相关的行业。我们的深度强化学习等技术，其实最早也是从游戏中训练而来的，而后基于启元决策智能平台做进一步的拓展和应用。所以我们比较自然的先发掘游戏行业的应用，比如为游戏公司提供 AI 引擎和服务。我们的 AI 智能体不仅可以在游戏中替代传统的 NPC，甚至可以陪人玩得很有乐趣（AI 和人类一起玩星际争霸的视频参见 http://www.inspirai.com/research.html），所以电子竞技行业是我们关注的比较多的。网络智能和仿真也是深度强化学习有优势的领域。
目前启元的决策智能平台已经具备如下竞争优势：
第一，持续学习的能力。持续学习的能力是智能体训练中关键的一环。在训练阶段，智能体需要在学习新技能的过程中保留过去学会的技能，才能达到很高的水平。启元决策智能平台通过智能体群体匹配竞技的方式实现「自然选择」，从而达到持续学习的效果。在竞技过程中，强者留存，弱者被淘汰。在弱者被淘汰之后，空出来的位置被强者的克隆体代替，而强者的克隆体则根据新的超参设定持续进化。在固定计算资源预算的情况下，启元决策智能平台通过这套机制在探索新强者（exploration）和深挖旧强者（exploitation）之间平衡对计算资源的使用情况。
第二，支持复杂场景的多智能体联合训练。在多智能体博弈问题中，不同智能体之间的相互克制较为常见，其收敛可能性极为复杂。以炸弹人竞赛举例，在竞赛中，不同队伍的智能体风格迥异，有的善攻，有的善守。基于「鲶鱼效应」的思想（指透过引入强者，激发弱者变强的效应），启元决策智能平台在训练初期引入基于规则的高阶对手，激发初期较弱的智能体在与强者的对决中学会各种基本技能，迅速提升变强；随着训练阶段的深入，启元决策智能平台同时训练多个智能体，使其在激烈的相互对抗中完善自我。
第三，支持基于私有云集群的大规模、高并发的模拟和大规模训练。启元决策智能平台将多个模块进行组件化，并封装到了容器中（如图）。通过云端自动化的方式管理数百 CPU 以及 GPU 资源并实现容器编排，降低了调度数十个炸弹人训练任务的成本。大规模、高并发的模拟计算以及大规模的训练同时在私有云集群中进行。另外，启元决策智能平台提供分布式存储方案，并配置成共享模型池，为炸弹人智能体模型群体的持久化和共享提供支持。

2018 年我们已经尝试把一些技术商业化，目前也取得了不错的营收。2019年，启元世界计划发布第一版启元决策智能平台型产品，为更多行业客户、终端用户带去高体验的服务。
说回决策智能，它是个比较通用的技术，这种辅助决策的能力可以泛化到很多行业，甚至包括网络智能—— 其实网络中的每一个节点也都是一个可决策的智能体，决策智能有很大的发挥空间。未来可能对于电信电力、网络智能相关的行业我们也会关注。
AI 科技评论：决策智能在现实应用中需要考虑决策的可解释性、决策的公平性、给人类提供辩解的机会等等问题。你们对这些问题是否有所准备？
袁泉：可解释性、公平性这些都很重要。这里面不仅要给人类提供辩解的机会，也需要让 AI 解释自己的决策过程，向人展示可信任的、具备可解释性的决策，以及辅助决策的结果。比如其中一种方式是，可以把决策结果以很好的可视化呈现出来，我们过去在电商中做过的推荐系统，在生成推荐结果的时候可以同时给出几条可解释性的推荐理由。目前我们也从技术上，包括深度学习可解释性相关的技术上做更多的技术积累。
Rct
调度
%secondmind.ai $24M
帮助企业进行决策，包括再平衡金融投资组合、管理供应链和物流。

Prowler的AI决策平台名叫VUCU，一些北欧资产管理公司已经用它来进行风险建模和投资组合优化，西班牙运输初创公司Paack还将它用于为司机规划最优路线。
监督学习技术需要依赖于大量的数据，但无监督学习技术则基于应用数学领域来讨论概率，不需要大量数据集。市面上的很多AI公司采用的都是前者，而Prowler采用的是后者。Prowler的决策软件还依赖于强化学习技术（软件从经验而非数据中学习）和博弈论。
以巴塞罗那的快递初创企业Paack为例，该公司利用Prowler的工具为骑手计划了优化路线。

测试
Test.ai $11M
Testim $10M
Mabl $20M
机器人
Osaro $37M
研究机器人深度强化学习的机器学习研发商，其开发的机器智能软件结合了感官知觉和判定能力，帮助计算机和机器人系统能够更加有快速有效地进行试错学习。
物流和仓储机器人

RPA
FortressIQ $30M
a new kind of artificial intelligence to process automation called imitation learning, 
raised $12 million.
It’s a bit like Robotics Process Automation (RPA), but instead of simply recording what’s happening on the desktop, and reproducing that digitally, it takes it a step further in a process called “imitation learning.”





运筹优化
赛道：为什么国外美国对标的公司？
技术路线？
求解器的区别导致应用的区别？

定制项目到产品化能力？
估值？
杉树科技 近亿元人民币
线性优化、混合整数优化、非线性优化
悠桦林 近亿人民币
智因科技 
组合优化、约束优化
宾通智能
nextMV $8M


Next generation AI 
Gamalon $20M
Bayesian Program Synthesis（BPS）实现了让机器自主完成概率编程，而不再需要人工编写。技术公布后，甚至有媒体宣称机器学习的速度将可能提升百倍。


场景AI
工业检测
深度视觉

智能运维
擎创科技 千万级美元
必示科技 1.5亿人民币
云兴维智 数千万人民币
RPA
Uiptah $750M
Automation Anywhere $290M
来也科技 4200万美元
弘玑Cyclone 近4000万美元
云扩科技 3000万美元
影刀RPA

行业AI
零售
ImageDT图匠数据：千万级美元
教育
在线教育：猿辅导、作业帮（工具切入）
AI教育：松鼠AI、暗物智能、流利说不行

猿辅导市值达到新东方的一半,原来是极度分散的行业

教育是一个非常分散的行业，俞敏洪：新东方+好未来，都不够
其实是在线教育的渗透率不够。
现在猿辅导的估值达到新东方的一半。
松鼠AI：10亿人民币
农业
Hypersonix $11.5M
爱科农：
极飞科技：12亿人民币
法律
Ross Intelligence
Atrium LTS
A16z, 60m
DoNotPays
可以帮助用户处理停车罚单或其他有争议的指控，截至2016年，该应用程序已成功帮助伦敦和纽约的用户避免了16万张罚单。
幂律智能
秘塔

金融
智能投顾/投研
Wealthfront $75M
Kensho $550M 收购


香侬科技：1.1亿人民币
虎博科技：3300万美元
阿法金融
eBrain
倍漾科技
卡方科技
弘量研究
贝塔数据



风控
同盾科技：1亿美金
Datavisor: 4000万美元
慧安金科: 1亿人民币
反欺诈
据估计，到2023年，反欺诈领域将拥有430亿美元的市场规模
Sift Science $53M
电商、网络支付以及Airbnb和Uber等交易类平台都是Sift Science的目标客户，目前，它已经拥有了Twitter，Airbnb，Twilio，Instacart，Zillow和Yelp等一系列知名客户。

具体来说，电商公司可以先把Sift Science的API嵌入自己网站，并提供一些这个网站上典型欺诈账号的数据样本供Sift Science参考。Sift Science会监测该账号在网站上的行为模式，把它和其他大量的欺诈行为对比，以此来计算这一账号的欺诈可疑性。监测的行为模式有很多维度，比如用户在这个网上浏览的页面数，所用设备和浏览器，是哪个地区的IP等等。
DataVisor，4000万美元
无监督机器学学习

DataVisor的一站式AI反欺诈平台，以独创的无监督反欺诈机器学习为核心，并融合了有监督机器学习和全球智能信誉库，为线上企业和金融公司提供一站式智能反欺诈检测服务。DataVisor独有的无监督反欺诈技术，无需历史标签和训练数据，有效检测未知欺诈和团伙欺诈，减少欺诈损失，降低人力成本，助力智能化反欺诈风控体系搭建，提升客户风控能力。

Simility 1.2亿美金被收购
新加坡的CashShield, GGV 2000万美元
特拉维夫的Forter,  5000万美元
巴黎的Shift Technology，6000万美元，accel
英国的Featurespace, 3000万美元

Signifyd 1亿美元
欺诈预防服务平台 

SentiLink
检测和阻止合成身份。他们提供实时API和风险分析师识别这些假人和其他连接的欺诈性应用程序，这样他们就不会损害您的底线。

UnifyID
所以该公司的目标是简化用户认证，提供一种基于传感器设备收集的数据进行生物学测量的用户认证技术。本地设备上安装的软件持续收集本地设备的数据，并与云服务进行通信，处理这些数据。收集的数据包括移动设备上的GPS、重力传感器数据；PC或笔记本上的键盘击键间隔、鼠标移动轨迹等等。这家公司声称有100多种属性的数据，检出准确率高达99.999%。
通过用户平常使用手机、电脑和可穿戴设备产生的数据，UnifyID可辨识用户的特征，例如走路的步态、速度等，形成用户的独特的档案。然后，再与登录账户时传来的数据比对，判断是不是用户本人。Unify ID会采集你生活中各种行为数据，形成你独有的标识。
Unify ID获得了TechCrunch创业大赛的亚军


Tessian $42M
自动解决企业邮件的安全问题，通过机器学习来发现和修复地址错误的邮件.如果它发现某封即将被寄出的邮件存在什么异常，那么它就会向用户发出警告，让他去仔细审查内容。

之前这家公司的名字叫CheckRecipient，它通过机器学习来发现和修复地址错误的邮件，这看似是个小问题，实际上会给大公司带来巨大的安全隐患，因为某些敏感的信息可能就会因此寄到错误的人手中。

Tessian指出，英国的信息委员会收到的安全事故报告中，有关邮件地址写错的，远远多于其他种类的安全问题。而欧洲最新的隐私法律会给这样的失误开出巨额的罚款。

“根据最近ICO的报告，邮件误寄已经成为了数据安全事故的头号问题，如今《通用数据保护条例》也已经实施，公司们应该将这个安全问题放在首位。人类的本能会惧怕黑客入侵或恶意软件这类事情，但我们很少会在寄邮件这些熟悉而又日常的事情前，三思而后行。实际上，这是一个巨大的隐患。”Tessian的首席执行官Tim Sadler说道。

Tessian的机器智能技术能将企业的邮件网络集中在一起，去分析和识别正常和异常的现象。如果它发现某封即将被寄出的邮件存在什么异常，那么它就会向用户发出警告，让他去仔细审查内容。

Tara AI $10M
AI 构建并管理产品开发生命周期，利用AI实现产品范围的自动化和软件开发人才的分配。

Tara AI利用机器学习来预测新软件项目所需的技术任务、工程资源和时间表。Tara AI正在改造缓慢、陈旧、完全手工的产品开发过程，这种过程导致企业每年因项目范围的低效而平均损失660亿美元。
如今，企业在他们的项目管理系统、git版本控制和员工目录中保存着有价值的数据。Tara AI连接到这些数据并使用机器学习模型，预测如何最好地构建软件(技术任务)、项目应该花费多长时间(时间轴)以及谁应该执行(资源)。

Tara AI的企业客户包括思科(Cisco)、Orange Silicon Valley和Mower Digital。到目前为止，它的人工智能技术已经从公开可用的数据中吸收了数百万个数据对象，并且正以20%的速度增长，导致每个项目的算法结果越来越精确。
医疗
总结



连心医疗：9000万人名币
麦歌算法

制药
全球融资金额超45亿美元，AI助力药企掀起创新热潮｜2020年盘点

https://36kr.com/p/1055494298325634

晶泰科技：3.188亿美元 全球最高的AI药研公司
望石智慧
First-in-class、Fast-follow、Me-better

费米子科技：上亿元
Recursion Pharmaceuticals
运用计算机视觉技术来处理细胞图像，通过分析细胞特征来评估疾病细胞药后反应结果的公司。他们使用先进的成像技术和人工智能技术进行高通量的细胞模型实验，致力于在上百种疾病的细胞模型中进行上千种候选药物的检测，最终找出对应不同疾病的新药。Recursion Pharmaceuticals的独特之处是结合机器自动化和人工智能技术，大规模地并行多个实验。现在，Recursion的实验室每周可以进行3万个实验。，在不久的将来他们可以每周进行几十万个实验。


服装

智布：1亿美元
极睿科技：亿元级人民币
时谛智能：近亿人民币
房地产
Skyline AI
物流
快运兔
工业
Augury $55M

工业物联网系统，利用手机应用、特殊装置和传感器来记录机器发动机和工作泵工作时发出的声音，然后将这些声音与正常运行的机器声音进行比较，然后辨别判断出当前运行的设备是否在正常工作，一旦发现声音不对或出现异常，就会跟进探索问题原因并寻求解决方案。

实际上，为了更好地检测、收集机器设备的声音，Augury公司需要将一种专业超声波传感器安装在设备上，比如工作泵、风扇、中央空调等，这些传感器会把收集到的数据发送到该公司开发的一款名为“Auguscope”的工具上进行分析，所有分析结果还能被发送到手机上，让管理人员及时了解设备状况、维修记录等信息。

值得一提的是，根据麦肯锡全球研究院（McKinsey Global Institute）最近发布的一项研究报告显示，预计到2025年全球企业设备维护行业的市场规模将会增长到12-37亿美元，这也给Augury公司创造了一个巨大的市场发展空间




个人思考
从论文挖人，重人力的活，不如机器之心、新智元、量子位。
从行业的理解角度，不如甲子光年。


VC思考
内部创业，内部创新
内心的小火苗：VC行业的创新
再次唤醒内心的小火苗

AI替代VC：创始人
AI替代FA

AI的根本逻辑是用数据编写部分功能
gravity
hugging face




做什么？
Deal sourcing innovation

为什么？
内心早已经有小火苗，却没有实践。
VC行业需要创新，耀途内部需要创新
心态上：要以创始人的心态和视角。

定位：VC行业的创新者。
变量是什么？
在线化
智能化

在变量
在线化：异步视频版的BP。提升沟通的效率
智能化：
语言识别，会议记录。提升认知的效率
创始人AI打分模型：提升对人理解的效率。（适合阅人无数的场景）
流动性（退出方式）：SPAC，加密货币，提升资金的效率。

创新者：
VC行业的创新者：

个人反思；
比较junior，不敢坚持推项目。
把自己定位成实习生，总是做研究，辅助参与项目，没有主动接触项目，从而没有认知闭环。

Cassie带宽有限，兴趣点不同。

AI+游戏：超参数、启元世界
AI文娱：虚拟形象
AR/VR







怎么做？
目的：
通过输出干货的方式，建立AI领域的影响力，触达创业者。（在于质量，不在于数量）
Founder sourcing strategy：
梳理AI领域的公司，并开源在github上
投资策略开源，以文章输出的方式

提供创业思路，提供全局视角。调研所有的公司。


创业者画像： 
事实：
不同领域的导师：
AI领域的导师：由于方法的范式变化，跳出了之前统计学习的框架。不在一线科研的导师hold不住学生。
非AI领域的导师：导师带领学生，学生的创新难以跳出老师现有的跳出现有框架。

NLP+行业的创业：一个复杂的流程，之中，小部分的


自由而无用，之前量子计算毕业找不到工作。学术界出来就是巨大的创新。

产学研
偏向于底层创新：一线。AI颠覆式创新：年轻的博士。Snorkel，旷视、商汤
偏向于应用侧面：行业+AI：一线的NLP工程师+领域资深人士。
基础软件的创业： 是一个巨大的工程，所以需要资深的软件工程师。snowflake
就像是堆积木。不断的改造，然后。

BERT、GPT3用海量的数据和算力。背后是钱的堆积

给定的基础任务，就算做到了SOTA，也很难去创业。比如文本分类，文本匹配。
没有壁垒，下个月就被超越。
算法的分类效果，不如数据的积累提升来的快。
所以创业者一定是比较颠覆的任务。
大公司的垃圾邮件过滤，换上新的算饭就好。

结论：一定要不要去通用基础的任务，比如文本分类。只能做到从90到91。
生成任务是从0到1的。Snorkel也是非常创新的角度。


事实：幂律智能，举办法律智能比赛。法律智能领域的论文是18级硕士做的。幂律智能创始人挂个三作。

社区
未来形态可能是工具，
工具的发展路径
Saas：adobe
社区：创意社区


小影科技不行，背靠大树好乘凉，剪辑工具难独活
2019年小影科技仅海外营收就超过亿级人民币且近三年复合增长率超50%，2020年VivaVideo在SensorTower发布的《2020上半年中国短视频/直播AP收入Top20》榜单中位列第四。

投资主题
深度学习
VR/AR
区块链
云原生
属于NLU
会话智能：
业务数据信息化并分析->语言数据信息化分析。
结构化数据vs非结构化数据

视频的创作与分析
可控的生成任务
内容生成：文本生产（故事线和知识），语意图像生产和检索（多模态）

极大的丰富设计资源：生成模型
版权保护：版权的界定？
品牌视觉管理难

AI infrastruce：MLOps

向量数据库
Deal sourcing方式
自媒体文章输出
GitHub
论文
专利：google patents
投资策略
医药机器人是机器人组看还是医药组看？

基金的发展的路径
多领域：人工智能+行业，人工智能+职能
多阶段：人工智能药物

人工智能金融
人工智能医疗
医疗影像：
药物
人工智能金融
智能投顾：
风控：图算法、图数据挖掘、异常检测

从人的mapping：
AI领域：将门创投


医疗信息化 VS 医疗AI

流程信息化，需要业务的知识
数据的特性，需要

数据共享：联邦学习、区块链
医疗
金融

Sourcing
学术界：论文、产学研
投资机构：将门创投、中科创星、真格、创新工场
科研机构：中科院、清华、北大、中科大、上海交大、复旦、微软亚研院、达摩院
人群：教授、博士
适合领域：适合前沿科技（量子计算、脑机接口），不适合应用软件，对市场敏感度较低
案例：spark、snorkel、CV四小龙
产业界：公司、展会
投资机构：XXX
公司：
人群：段位高的人、程序员社区（陈昱）
适合领域：工程量大、对市场敏感高
案例：各种数据库

云原生是一个代码工程量很大的领域：pingcap、snowflake

AI是一个数据算力要求比好高的领域
成熟的任务没有机会，机会新的任务（如生产任务）
人脸识别、文本分类
GPT3、GAN
成熟的任务就是产品化。
差异化：定义好产品


预训练模型改变了什么？
降低了对fi-tune阶段的数据量的和标注依赖，提高了pre-train阶段的算力需求
从商业的角度来说，降低了定制阶段的时间，提高了研发成本。成本从实施转移到研发。提高了研发成本，降低了边际成本（包括数据的获取成本和标注成本），提升毛利率。

AutoML改变了什么？
降低了对算法工程师的经验依赖，减少了调参时间
从商业的角度降低了算法工程师的人力成本


生成任务（如GAN）可能改变了什么？
极大的降低了创作的门槛
未来的机会可能在数字创意领域（所以Adobe做了非常多的研究和研发）




从人的角度

调研AI
研究思路
视觉端：关注unity和adobe的收购新闻

小结
传统方式用代码编写功能，
机器学习用数据编写功能。

用数据编写核心功能：CV四小龙，客服机器人，convesationAI
用数据编写核心功能：


看AI提升的效率：
AI+行业？学术的单点巨大突破带动的。风控、医学影像、药物研发、调度
AI+场景？看国外：RPA、招聘、法律、运维

技术突破：
行业的变化：政策

预训练模型带来了什么？
GPT3


Transformer
安全


二级市场的价格说相对连续的，一级市场的价格是相对离散的。
需要事件驱动、造成风口（比如RPA、海外的融资进展、二级市场的增长等）
吸引优秀的员工出来创业
吸引资金的投入

从技术的产品形态看来，发展趋势来看是文娱、游戏、创作的机会。
金融

区块链
基础软件
开源
退出周期短：择时有更高的要求，什么时候买入，什么时候卖出

物流
好像还是可以看一看，车的调度，saas
NLP学术团队创业
幂律智能
Recurrent.AI

政策的影响是很多的
疫情影响的是政策
税改
GDPR

技术的突破
DeepMind AlphaFold2 解决蛋白质折叠
原来是结构生物学，迎来了一个「革命性」的突破。
11月30日，DeepMind宣布：AlphaFold 2，这个AI已经成功解决蛋白质折叠的问题，生物学50年的难题被DeepMind解决了，
AlphaFold的“准确性”均分，直接从原本的60+/100，提升至了92.4/100。
而过去十几年，其他方法只能在40分左右徘徊。
OpenAI预训练模型GPT3
GPT3
快手万亿参数


NLP目前能做什么，不能做什么
把非结构化的本文，通过分类，换成结构化的标签+加上规则系统。
跟自动驾驶比较像，把传感器把数据结构化，然后用规则系统。
外呼机器人，意图识别之后是coding system。本质上是做分类。

被替代的场景：
低社交、高重复。卡车司机

差的销售容易替代，但是创造的价值少，替代没有意义。
好的销售难替代，但是创造的价值大，所以说辅助，提升效率。

壁垒
多维度
落地时复杂的问题
优化效率
好的产品、技术和交付能力

灾难性遗忘、持续学习
NLP落地在什么行业？
看精细化程度要求的高低：
金融、保险
房地产、教育

NLP的发展阶段












大数据
大模型

自监督学习同分布数据泛化能力好
预训练模型任务泛化能力好








AI VC
国内
创新工场
GGV
线性资本
明势资本
靖亚资本
初心资本
国外
Index Ventures
Mike Volpi
Fireside Chat: Mike Volpi, General Partner, Index Ventures (FirstMark's Data Driven NYC)

Fireside Chat with Mike Volpi (Index Ventures)


creativity

Confluent、elastic、cockroach

​ - Looking Forward: 2021 and Beyond (Part I AI)

人其实就是由文字和声音组成的。替代人写文章。
从预测到生成

疫情加速了视频数据的产生
AI从预测到生成。
艺术，音乐和电影创作

关于GPT3
创作
AI的摩尔定律去预测
GPT3的差异化产品形态
带来了多样性
Bryan offut


类别于电力，冰箱

The Evolution and Future of Open Source



如何做开源的早期投资A轮和A轮之前
核心社区开发者：从Hortonworks学到社区的核心开发者，应该尽可能的招到公司。
大的市场：大多数self-host用户不付钱。不到10%的用户会付钱。采用Freemium的模式，所以市场要大。每个节点100～1000美元。
包含很多数据的开源项目更容易商业化，因为客户乎算有多少数据在这里面。数据库、kafaka（隐形数据库），越多的数据，就越多的节点，就会付越多的钱。

Hotonworks和cloudera由于竞争，价格战。就尽可能的把商业化feature做的越来越薄，导致最后没有利润

后期的简单，就看数据，早期就看一些线索。

A16Z
Martin Casado
Accel

FirstMark Capital

Basis Set Ventures
媒体







AI软件的创业机会在哪里？
AI时代的巨头可能会在哪里？

具体答案是我也不知道。如果连我拍都能能想出来的，但是那些冲在一些的人，和巨头的战略部门更应该知道，互联网巨头或者AI巨头早就去做了。那就是不是机会了。
应该是巨头一开始没看到，或者不起眼，或者做不起来的方向。

AI软件的创业机会不外乎3点
AI创业分类
AI+基础设施
AI+场景
AI+行业
AI+基础设施：
数据标注：scale
AutoML：datarobot
MLops：
Model monitoring：Arthur
Obervility：abcus
向量数据库：pingcone
向量搜索：milvus, Jina, 
Rasa, hugging face, Pytorch lightening
AI+场景：
从流程信息化 -> 会话文本化 ：
otter.ai、 魔音智能
Going.io 、chorus.ai. 
从理解到生成 -> AI内容生成：
输出比输入难很多：作文必阅读更费时间、看懂单词和会拼写单词是两种能力
艺术和AI的结合
Video native：
需求增加


AI+行业
行业语言模型
金融：投研、投顾、反欺诈
医疗：医疗影像、医学文本
药研：
教育：自适应教育

趋势总结与思考
趋势一：论文的state of the art层出不穷，不管多牛的模型，用不多久就被超越，所以模型本身没有壁垒。

科研部门与工程部门的割裂，缺乏沟通。把科研的成果模型工程化。
开源

创业公司的机会在哪里？
Hugging face 的开源项目transformer保持着NLP模型的各种sota，强调易用性。

趋势二：诸如GPT和BERT这类预训练模型越来越大。

对于分布式的需求越来越高
深度学习框架：一流科技
异构虚拟化：趋动科技

趋势三：代码共享—>数据共享
Github for data

趋势四：AI时代的搜索，搜索的是向量（embedding）：
Zilliz项目Miluvs
Jina

趋势四：AI科研走向工程：
模型部署到监测

趋势五：生成任务越来越成熟。
视觉端：GAN、
文本端：GPT3

趋势六：AI的开发的生命周期被重塑。MLops

模型的管理

从商业的角度来说：
AutoML降低了算法工程师的工作量降低了部分人力成本
预训练语言模型降低了对数据的依赖。降低了部分数据成本提升了交付能力
算力的成本：
Weight bais

AI低毛利，SaaS成本


AI基础设施
AI生成
互联网：Google、Microsoft、Amazon
移互联网：Facebook、Apple、微信
AI时代：更智能？提升效率？

我不这么认为
什么是AI？我认为是创作。

AI分为专家系统、机器学习。。。。
专家系统：基于规则
机器学习：基于概率



信息输入VS信息输出
阅读VS作文
听英语VS说英语
听别人唱歌VS自己唱歌

AI分为理解和生成
NLP：NLU VS NLG
视觉：CV VS CG（neural rendering）
听觉：ASR VS Text2Speech

从技术演变的角度来说，生成的技术难度更大。
从用户体验的角度来说，生成的体验更具有颠覆性。

文本分类，从80%，提升到90%，体验不大。
但是以前的技术在生成，可能是从0到1点。

不管是像素偏移、ZMO、还是诗云科技都看到了这个大方向，
但是具体来说创作或者创意的机会在哪？我不知道。巨头也不知道。
如果巨头知道，早就去干了。就不是创业公司的机会了。
巨头的战略部或者产品部肯定比我更懂。他们都不知道，那我就更不知道了。


AI赋能软件：
本质
阿姆达尔定律的关键在于，你能够获取的最大速度提升受限于优化的工作所占的比例。
用商业的说法就是：关键是看解决的是痛点还是痒点
在某个环节能有巨大的提升，或者说在打通了某个小的环节，但是释放的势能是巨大的。

该定律的数学公式为：
假设这部分工作占用了90%的时间，即p = 0.90，在优化的过程中，如果将这部分的时间降至0，则整体的工作速度将提高1/(1 – 0.90) = 10倍。
假设这部分工作占用了10%的时间，即p = 0.10，在优化的过程中，如果将这部分的时间降至0，则整体的工作速度将提高1/(1 – 0.10) = 1。1倍。



这一波AI的热潮来源于2012的ImageNet上的突破，本质上是深度神经网络带来的。

深度神经网络最大的提升是在于对于非结构化数据：文本、图像、视频和音频的处理能力。更具体的来说，是通过神经网络把这些非结构化的数据转化为稠密的向量。然后对这些向量做各种操作。

我们现在在讨论的都AI本质的本质上都是



文章总结

AutoML:
Auto Feature engineering： Feature Labs，Explorium
AUTOML：H2O.ai，DataRobot，4paradigm, iguazio, Cnvrg.io, AutoML, Firefly.ai
NAS：google，

MLOps：
1: Experiment
MLops will become a big market?  
Eg: Comet.ML，
2: Deploy
Competion from big data science/machine learning platform ?
Eg: Spell，ParrellelM(acquire), Rasa
总结
Data sharing?
Federal learning
Blockchain ?


数据
数据发现：Explorium.ai 
数据标注：监督学习。Dataloop，LightTAG
数据生成：降低对数据和数据标注的依赖 Eg: Datagen, AI.reverie

NLP: rasa

实验和部署
DL框架
MLOps：Missinglink, Allegro, cnvrg.io and Comet
Kubernetes :, , 

加速
硬件：HAILO, HABANA
软件：虚拟化Eg: RUNAI, Bitfusion
可解释性：Fiddler labs，aporia(高盛)



耀途分享
人或者技术的mapping
5倍估值，但是风险没有下降5倍。

2C：15亿人抓到几亿人，就是几百亿美金
2B：天花板取决于供应链，就30倍的回报

2C是覆盖式的打法，中国理解
2B是阻击式的打法，全球理解

2C不依赖产业资源，依赖流量
2B依赖产业资源和供应链，比如小米很强势

聚焦和专注
产业资源：抢项目

系统性的研究

来一项目看一个项目：推荐
主动梳理：推荐

主动去挖水面下的项目

很多的新技术增量市场，都在以色列。
AWS是新技术风向标。


Anapa
Mellanox

炎融对标weka.io

以色列都是做颠覆式创新，然后被收购



复盘
L4一定要投资，
特别大的赛道，估值贵一点也没关系，主流美元基金都很积极。
万亿级美金的市场。

大的方向的第一轮没有看到

清华

Cassie
软件投资年轻人

因为大龄的人，单一资源依赖，如果资源

系统集成
服务业和制造业的区别。

归纳用于的需求
归纳

机器人

2C：面向最终客户
2B：
2G：

供应链和终端
模块化，项目制作
面向终端的，反而能定义出一些模块。

2C软件，2C消费电子，本质是一样。
2C和2小B，需要产品定义的能力
学习能力强，

产品定义的能力，

人不一定是老鸟，但是到底什么样的人能成功？

应用怎么在早期判断，下决心。

机器人

AI infra的人什么才是适合的？

符号
数据隐私、合规
隐私计算
数据库
AI infra
MLops
NLP
Vision
Audio/speech
个性化推荐
决策智能
Next generation AI 
场景AI
行业AI
个人思考
调研AI
AI VC
AI软件的创业机会在哪里？
文章总结
wentingcan@wentingcandeMacBook-Pro testCode % clear

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
符号
数据隐私、合规
隐私计算
数据库
AI infra
MLops
NLP
Vision
Audio/speech
个性化推荐
决策智能
Next generation AI 
场景AI
行业AI
个人思考
调研AI
AI VC
AI软件的创业机会在哪里？
文章总结
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
Traceback (most recent call last):
  File "/Users/wentingcan/Desktop/testCode/processAIdoc.py", line 12, in <module>
    content += "#" + p.text + "\n"
NameError: name 'content' is not defined
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号

#符号
#数据隐私、合规

#符号
#数据隐私、合规
#隐私计算

#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库

#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra

#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
#隐私计算
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
##时间序列
##Graph
##NoSQL
##内存数据库
##Relation
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
###BigID $70M
###OneTrust $300M
###Druva $130M
###Privitar $80M
###Ethyca $13.5M
###InCountry $18M
###Text IQ $12.6M
### $5M
###WireWheel $20M
###concentric.ai $7.5M
#隐私计算
###多方安全计算MPC
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
###ZilliZ milvus
###Jina 600万美元
###Pinecone
###tecton.ai
##时间序列
###Influxdb $60M
###Timescale $15M
###涛思TDengine 超1000万美元
##Graph
###TigerGraph 1.05亿美元
###欧若数网 Nebula 近千万美元
###DGraph $11.5M
##NoSQL
####ScyllaDB
###MongoDB
##内存数据库
##Relation
###新数科技
###巨杉数据库
###Pingcap
###CockroachDB
###Rockset
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
###OctoML $15M
###Neural magic $15M
###Weka.IO $31.7M
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
###微软NNI
###亚马逊AutoGluon
###谷歌
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
###databand.ai $14.5M
###WhyLabs $4M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
###Fiddler labs $10.2M
###InterpretML
###RealAI
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
###达观数据 2.7亿人民币
##机器翻译
###Unbabel：众包 $60M
###Lilt $25M
###*推文科技：网络小说翻译 1000万人民币 联想之星
###*Atman：医药文献翻译 560万美元 北极光
##文本重写
###Grammarly $90M
##Chatbot
###Automated CX
###Ada Support $44M
###智能客服
###追一科技 4100万美元
###智齿科技 2.1亿人民币
###晓多科技 超2亿人民币
###乐言科技 1.5亿人民币
###心理健康
###Woebot Labs  $22.8M 心理健康聊天机器人
###运维
###Moveworks $75M
###其他
###Troops.ai $12M
##背景调查
###Checkr $160M
###Middesk $4M
###i背调：数千万人民币
##招聘
###Eightfold $125M
###Turing.com $32M
###e成科技 8000万美元
###Bello倍罗 数千万人民币
###近屿智能 数千万人民币
###方便面面试
###Pyxai $150K
##合同审查
###Kira systems CA$65M
##销售
####Gong.io
####chorus.ai
###People.ai
###Troops.ai
###Tact.AI 
###Recurrent.ai
###客知音
###深维智信
###Sales enablement
##其他
#### A21 labs
###Golden $14.5M
###ClearGraph 被收购
###UpCodes $3.4M
#Vision
###技术路线
##综合
###商汤
###旷世
###依图
###云从
###图普科技
##动作捕捉
###诺亦腾
###Xmov
###

##创作工具
###Canva $60M, $8.7B
###Figma $50M, $2B 
###InVisionApp $115M, $1.9B
###Runway $8.5M
###Beautiful.AI $11M
###GliaCloud
###来画视频 5000万人民币
###漫画
##图像压缩
###图鸭科技 数千万人民币
##渲染
###个人总结：
###51world
###粒界科技
###叠境
###RestAR
###酷家乐
###迈吉客科技
###商询科技 datamesh
###时谛智能
##形象生成
###Brud $20M $125M
###FaceRig $2M
###EmbodyMe
###Xmov魔珐科技 数亿人民币
###相芯科技 1.2亿人民币
###迈吉客科技 数千万人民币
###诗云科技 数百万美金
###ZMO.ai
###像素偏移
###慧夜科技
###我是大咖
###
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
###闪马智能
##OCR
###HyperScience $80M
##视频广告
####KERV Interactive $11M
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
###深尚科技
##安防
####AnyVision  $43M
###tractable.ai
##视频异常
###闪马智能：近亿元人民币
##测试
####Applitools $31M
##医学影像
###连心医疗：9000万人民币
##其他
###Akasha Imaging
###墨奇科技
#Audio/speech
##音乐
###Amper Music
###StepBeats
##语音
###Descript
###DeepGram
###Otter.ai $50M
###魔音助手 5000万美元
###思必驰：端侧
###云知声：云
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
###Pindrop  $90M
##CRM
###Troops.ai
##医药
###Suki $20M
#个性化推荐
###Attentive $230M
###Outlier $22.1M
###Lily $12.5M
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###启元世界
###南栖仙策
###游戏
###%DeepMind
###超参数科技
###启元世界
###Rct
###调度
###%secondmind.ai $24M
###测试
###Test.ai $11M
###Testim $10M
###Mabl $20M
###机器人
###Osaro $37M
###RPA
###FortressIQ $30M
##运筹优化
###杉树科技 近亿元人民币
###悠桦林 近亿人民币
###智因科技 
###宾通智能
###nextMV $8M
#Next generation AI 
###Gamalon $20M
#场景AI
##工业检测
###深度视觉
##智能运维
###擎创科技 千万级美元
###必示科技 1.5亿人民币
###云兴维智 数千万人民币
##RPA
###Uiptah $750M
###Automation Anywhere $290M
###来也科技 4200万美元
###弘玑Cyclone 近4000万美元
###云扩科技 3000万美元
###影刀RPA
#行业AI
###零售
###ImageDT图匠数据：千万级美元
##教育
###松鼠AI：10亿人民币
##农业
###Hypersonix $11.5M
###爱科农：
###极飞科技：12亿人民币
##法律
###Ross Intelligence
###Atrium LTS
###DoNotPays
###幂律智能
###秘塔
##金融
###智能投顾/投研
###Wealthfront $75M
###Kensho $550M 收购
###
###香侬科技：1.1亿人民币
###虎博科技：3300万美元
###阿法金融
###eBrain
###倍漾科技
###卡方科技
###弘量研究
###贝塔数据
###风控
###同盾科技：1亿美金
###Datavisor: 4000万美元
###慧安金科: 1亿人民币
###反欺诈
###Sift Science $53M
###DataVisor，4000万美元
###Simility 1.2亿美金被收购
###新加坡的CashShield, GGV 2000万美元
###特拉维夫的Forter,  5000万美元
###巴黎的Shift Technology，6000万美元，accel
###英国的Featurespace, 3000万美元
###Signifyd 1亿美元
###SentiLink
###UnifyID
###Tessian $42M
###Tara AI $10M
##医疗
###总结
###连心医疗：9000万人名币
###麦歌算法
##制药
###晶泰科技：3.188亿美元 全球最高的AI药研公司
###望石智慧
###费米子科技：上亿元
###Recursion Pharmaceuticals
##服装
##
###智布：1亿美元
###极睿科技：亿元级人民币
###时谛智能：近亿人民币
##房地产
###Skyline AI
##物流
###快运兔
##工业
###Augury $55M
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
###DeepMind AlphaFold2 解决蛋白质折叠
###OpenAI预训练模型GPT3
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
###Index Ventures
###A16Z
###Accel
###FirstMark Capital
###Basis Set Ventures
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % clear

wentingcan@wentingcandeMacBook-Pro testCode % clear























































wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
###BigID $70M
###OneTrust $300M
###Druva $130M
###Privitar $80M
###Ethyca $13.5M
###InCountry $18M
###Text IQ $12.6M
### $5M
###WireWheel $20M
###concentric.ai $7.5M
#隐私计算
###多方安全计算MPC
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
###ZilliZ milvus
###Jina 600万美元
###Pinecone
###tecton.ai
##时间序列
###Influxdb $60M
###Timescale $15M
###涛思TDengine 超1000万美元
##Graph
###TigerGraph 1.05亿美元
###欧若数网 Nebula 近千万美元
###DGraph $11.5M
##NoSQL
####ScyllaDB
###MongoDB
##内存数据库
##Relation
###新数科技
###巨杉数据库
###Pingcap
###CockroachDB
###Rockset
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
###OctoML $15M
###Neural magic $15M
###Weka.IO $31.7M
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
###微软NNI
###亚马逊AutoGluon
###谷歌
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
###databand.ai $14.5M
###WhyLabs $4M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
###Fiddler labs $10.2M
###InterpretML
###RealAI
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
###达观数据 2.7亿人民币
##机器翻译
###Unbabel：众包 $60M
###Lilt $25M
###*推文科技：网络小说翻译 1000万人民币 联想之星
###*Atman：医药文献翻译 560万美元 北极光
##文本重写
###Grammarly $90M
##Chatbot
###Automated CX
###Ada Support $44M
###智能客服
###追一科技 4100万美元
###智齿科技 2.1亿人民币
###晓多科技 超2亿人民币
###乐言科技 1.5亿人民币
###心理健康
###Woebot Labs  $22.8M 心理健康聊天机器人
###运维
###Moveworks $75M
###其他
###Troops.ai $12M
##背景调查
###Checkr $160M
###Middesk $4M
###i背调：数千万人民币
##招聘
###Eightfold $125M
###Turing.com $32M
###e成科技 8000万美元
###Bello倍罗 数千万人民币
###近屿智能 数千万人民币
###方便面面试
###Pyxai $150K
##合同审查
###Kira systems CA$65M
##销售
####Gong.io
####chorus.ai
###People.ai
###Troops.ai
###Tact.AI 
###Recurrent.ai
###客知音
###深维智信
###Sales enablement
##其他
#### A21 labs
###Golden $14.5M
###ClearGraph 被收购
###UpCodes $3.4M
#Vision
###技术路线
##综合
###商汤
###旷世
###依图
###云从
###图普科技
##动作捕捉
###诺亦腾
###Xmov
###

##创作工具
###Canva $60M, $8.7B
###Figma $50M, $2B 
###InVisionApp $115M, $1.9B
###Runway $8.5M
###Beautiful.AI $11M
###GliaCloud
###来画视频 5000万人民币
###漫画
##图像压缩
###图鸭科技 数千万人民币
##渲染
###个人总结：
###51world
###粒界科技
###叠境
###RestAR
###酷家乐
###迈吉客科技
###商询科技 datamesh
###时谛智能
##形象生成
###Brud $20M $125M
###FaceRig $2M
###EmbodyMe
###Xmov魔珐科技 数亿人民币
###相芯科技 1.2亿人民币
###迈吉客科技 数千万人民币
###诗云科技 数百万美金
###ZMO.ai
###像素偏移
###慧夜科技
###我是大咖
###
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
###闪马智能
##OCR
###HyperScience $80M
##视频广告
####KERV Interactive $11M
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
###深尚科技
##安防
####AnyVision  $43M
###tractable.ai
##视频异常
###闪马智能：近亿元人民币
##测试
####Applitools $31M
##医学影像
###连心医疗：9000万人民币
##其他
###Akasha Imaging
###墨奇科技
#Audio/speech
##音乐
###Amper Music
###StepBeats
##语音
###Descript
###DeepGram
###Otter.ai $50M
###魔音助手 5000万美元
###思必驰：端侧
###云知声：云
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
###Pindrop  $90M
##CRM
###Troops.ai
##医药
###Suki $20M
#个性化推荐
###Attentive $230M
###Outlier $22.1M
###Lily $12.5M
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###启元世界
###南栖仙策
###游戏
###%DeepMind
###超参数科技
###启元世界
###Rct
###调度
###%secondmind.ai $24M
###测试
###Test.ai $11M
###Testim $10M
###Mabl $20M
###机器人
###Osaro $37M
###RPA
###FortressIQ $30M
##运筹优化
###杉树科技 近亿元人民币
###悠桦林 近亿人民币
###智因科技 
###宾通智能
###nextMV $8M
#Next generation AI 
###Gamalon $20M
#场景AI
##工业检测
###深度视觉
##智能运维
###擎创科技 千万级美元
###必示科技 1.5亿人民币
###云兴维智 数千万人民币
##RPA
###Uiptah $750M
###Automation Anywhere $290M
###来也科技 4200万美元
###弘玑Cyclone 近4000万美元
###云扩科技 3000万美元
###影刀RPA
#行业AI
###零售
###ImageDT图匠数据：千万级美元
##教育
###松鼠AI：10亿人民币
##农业
###Hypersonix $11.5M
###爱科农：
###极飞科技：12亿人民币
##法律
###Ross Intelligence
###Atrium LTS
###DoNotPays
###幂律智能
###秘塔
##金融
###智能投顾/投研
###Wealthfront $75M
###Kensho $550M 收购
###
###香侬科技：1.1亿人民币
###虎博科技：3300万美元
###阿法金融
###eBrain
###倍漾科技
###卡方科技
###弘量研究
###贝塔数据
###风控
###同盾科技：1亿美金
###Datavisor: 4000万美元
###慧安金科: 1亿人民币
###反欺诈
###Sift Science $53M
###DataVisor，4000万美元
###Simility 1.2亿美金被收购
###新加坡的CashShield, GGV 2000万美元
###特拉维夫的Forter,  5000万美元
###巴黎的Shift Technology，6000万美元，accel
###英国的Featurespace, 3000万美元
###Signifyd 1亿美元
###SentiLink
###UnifyID
###Tessian $42M
###Tara AI $10M
##医疗
###总结
###连心医疗：9000万人名币
###麦歌算法
##制药
###晶泰科技：3.188亿美元 全球最高的AI药研公司
###望石智慧
###费米子科技：上亿元
###Recursion Pharmaceuticals
##服装
##
###智布：1亿美元
###极睿科技：亿元级人民币
###时谛智能：近亿人民币
##房地产
###Skyline AI
##物流
###快运兔
##工业
###Augury $55M
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
###DeepMind AlphaFold2 解决蛋白质折叠
###OpenAI预训练模型GPT3
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
###Index Ventures
###A16Z
###Accel
###FirstMark Capital
###Basis Set Ventures
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % clear

wentingcan@wentingcandeMacBook-Pro testCode % clear























































wentingcan@wentingcandeMacBook-Pro testCode % clear























































wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#符号
#数据隐私、合规
###BigID $70M
###OneTrust $300M
###Druva $130M
###Privitar $80M
###Ethyca $13.5M
###InCountry $18M
###Text IQ $12.6M
### $5M
###WireWheel $20M
###concentric.ai $7.5M
#隐私计算
###多方安全计算MPC
###华控清交
##芯片
###星云Clustar
####Duality Technologies
##联邦学习：
###微众银行
###蚂蚁金服
###平安银行
#数据库
##向量数据库
###ZilliZ milvus
###Jina 600万美元
###Pinecone
###tecton.ai
##时间序列
###Influxdb $60M
###Timescale $15M
###涛思TDengine 超1000万美元
##Graph
###TigerGraph 1.05亿美元
###欧若数网 Nebula 近千万美元
###DGraph $11.5M
##NoSQL
####ScyllaDB
###MongoDB
##内存数据库
##Relation
###新数科技
###巨杉数据库
###Pingcap
###CockroachDB
###Rockset
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
###OctoML $15M
###Neural magic $15M
###Weka.IO $31.7M
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
###微软NNI
###亚马逊AutoGluon
###谷歌
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
###databand.ai $14.5M
###WhyLabs $4M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
###Fiddler labs $10.2M
###InterpretML
###RealAI
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
###达观数据 2.7亿人民币
##机器翻译
###Unbabel：众包 $60M
###Lilt $25M
###*推文科技：网络小说翻译 1000万人民币 联想之星
###*Atman：医药文献翻译 560万美元 北极光
##文本重写
###Grammarly $90M
##Chatbot
###Automated CX
###Ada Support $44M
###智能客服
###追一科技 4100万美元
###智齿科技 2.1亿人民币
###晓多科技 超2亿人民币
###乐言科技 1.5亿人民币
###心理健康
###Woebot Labs  $22.8M 心理健康聊天机器人
###运维
###Moveworks $75M
###其他
###Troops.ai $12M
##背景调查
###Checkr $160M
###Middesk $4M
###i背调：数千万人民币
##招聘
###Eightfold $125M
###Turing.com $32M
###e成科技 8000万美元
###Bello倍罗 数千万人民币
###近屿智能 数千万人民币
###方便面面试
###Pyxai $150K
##合同审查
###Kira systems CA$65M
##销售
####Gong.io
####chorus.ai
###People.ai
###Troops.ai
###Tact.AI 
###Recurrent.ai
###客知音
###深维智信
###Sales enablement
##其他
#### A21 labs
###Golden $14.5M
###ClearGraph 被收购
###UpCodes $3.4M
#Vision
###技术路线
##综合
###商汤
###旷世
###依图
###云从
###图普科技
##动作捕捉
###诺亦腾
###Xmov
###

##创作工具
###Canva $60M, $8.7B
###Figma $50M, $2B 
###InVisionApp $115M, $1.9B
###Runway $8.5M
###Beautiful.AI $11M
###GliaCloud
###来画视频 5000万人民币
###漫画
##图像压缩
###图鸭科技 数千万人民币
##渲染
###个人总结：
###51world
###粒界科技
###叠境
###RestAR
###酷家乐
###迈吉客科技
###商询科技 datamesh
###时谛智能
##形象生成
###Brud $20M $125M
###FaceRig $2M
###EmbodyMe
###Xmov魔珐科技 数亿人民币
###相芯科技 1.2亿人民币
###迈吉客科技 数千万人民币
###诗云科技 数百万美金
###ZMO.ai
###像素偏移
###慧夜科技
###我是大咖
###
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
###闪马智能
##OCR
###HyperScience $80M
##视频广告
####KERV Interactive $11M
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
###深尚科技
##安防
####AnyVision  $43M
###tractable.ai
##视频异常
###闪马智能：近亿元人民币
##测试
####Applitools $31M
##医学影像
###连心医疗：9000万人民币
##其他
###Akasha Imaging
###墨奇科技
#Audio/speech
##音乐
###Amper Music
###StepBeats
##语音
###Descript
###DeepGram
###Otter.ai $50M
###魔音助手 5000万美元
###思必驰：端侧
###云知声：云
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
###Pindrop  $90M
##CRM
###Troops.ai
##医药
###Suki $20M
#个性化推荐
###Attentive $230M
###Outlier $22.1M
###Lily $12.5M
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###启元世界
###南栖仙策
###游戏
###%DeepMind
###超参数科技
###启元世界
###Rct
###调度
###%secondmind.ai $24M
###测试
###Test.ai $11M
###Testim $10M
###Mabl $20M
###机器人
###Osaro $37M
###RPA
###FortressIQ $30M
##运筹优化
###杉树科技 近亿元人民币
###悠桦林 近亿人民币
###智因科技 
###宾通智能
###nextMV $8M
#Next generation AI 
###Gamalon $20M
#场景AI
##工业检测
###深度视觉
##智能运维
###擎创科技 千万级美元
###必示科技 1.5亿人民币
###云兴维智 数千万人民币
##RPA
###Uiptah $750M
###Automation Anywhere $290M
###来也科技 4200万美元
###弘玑Cyclone 近4000万美元
###云扩科技 3000万美元
###影刀RPA
#行业AI
###零售
###ImageDT图匠数据：千万级美元
##教育
###松鼠AI：10亿人民币
##农业
###Hypersonix $11.5M
###爱科农：
###极飞科技：12亿人民币
##法律
###Ross Intelligence
###Atrium LTS
###DoNotPays
###幂律智能
###秘塔
##金融
###智能投顾/投研
###Wealthfront $75M
###Kensho $550M 收购
###
###香侬科技：1.1亿人民币
###虎博科技：3300万美元
###阿法金融
###eBrain
###倍漾科技
###卡方科技
###弘量研究
###贝塔数据
###风控
###同盾科技：1亿美金
###Datavisor: 4000万美元
###慧安金科: 1亿人民币
###反欺诈
###Sift Science $53M
###DataVisor，4000万美元
###Simility 1.2亿美金被收购
###新加坡的CashShield, GGV 2000万美元
###特拉维夫的Forter,  5000万美元
###巴黎的Shift Technology，6000万美元，accel
###英国的Featurespace, 3000万美元
###Signifyd 1亿美元
###SentiLink
###UnifyID
###Tessian $42M
###Tara AI $10M
##医疗
###总结
###连心医疗：9000万人名币
###麦歌算法
##制药
###晶泰科技：3.188亿美元 全球最高的AI药研公司
###望石智慧
###费米子科技：上亿元
###Recursion Pharmaceuticals
##服装
##
###智布：1亿美元
###极睿科技：亿元级人民币
###时谛智能：近亿人民币
##房地产
###Skyline AI
##物流
###快运兔
##工业
###Augury $55M
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
###DeepMind AlphaFold2 解决蛋白质折叠
###OpenAI预训练模型GPT3
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
###Index Ventures
###A16Z
###Accel
###FirstMark Capital
###Basis Set Ventures
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % clear

wentingcan@wentingcandeMacBook-Pro testCode % clear























































wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
Traceback (most recent call last):
  File "/Users/wentingcan/Desktop/testCode/processAIdoc.py", line 39, in <module>
    print(content)
NameError: name 'content' is not defined
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
Traceback (most recent call last):
  File "/Users/wentingcan/Desktop/testCode/processAIdoc.py", line 39, in <module>
    print(content)
NameError: name 'content' is not defined
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % clear

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % clear                 

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % clear                 

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
unactive
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
active
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP
##综合
##机器翻译
##文本重写
##Chatbot
###Automated CX
###智能客服
###心理健康
###运维
###其他
##背景调查
##招聘
##合同审查
##销售
##其他
#Vision
###技术路线
##综合
##动作捕捉
###诺亦腾
###Xmov
##创作工具
###漫画
##图像压缩
##渲染
##形象生成
###DID
##视频录制
###
###Loom
##视频
###Viedeo++
###影普科技
###Kapwing
###视频异常分析
##OCR
##视频广告
##无人零售
###Grabango
###Standard Cognition
###Mad Street Den
##时尚
##安防
###tractable.ai
##视频异常
##测试
##医学影像
##其他
#Audio/speech
##音乐
##语音
##声纹识别
###VoiceAI 
###SpeakIn
##反欺诈
##CRM
###Troops.ai
##医药
#个性化推荐
#决策智能
##研究 
###运筹学
###分类：
###线性规划（Linear Programming）
###整数规划（Integer Programming）问题
###总结
##强化学习
###综合
###游戏
###调度
###测试
###机器人
###RPA
##运筹优化
#Next generation AI 
#场景AI
##工业检测
##智能运维
##RPA
#行业AI
###零售
##教育
##农业
##法律
##金融
###智能投顾/投研
###风控
###反欺诈
##医疗
##制药
##服装
##
##房地产
##物流
##工业
#个人思考
###VC思考
##创业者画像： 
##社区
##投资主题
###会话智能：
###视频的创作与分析
###可控的生成任务
###向量数据库
##Deal sourcing方式
##投资策略
#调研AI
###研究思路
###小结
##金融
##NLP学术团队创业
##政策的影响是很多的
##技术的突破
##NLP目前能做什么，不能做什么
##NLP落地在什么行业？
##NLP的发展阶段
#AI VC
##国内
##国外
#AI软件的创业机会在哪里？
###AI创业分类
###趋势总结与思考
##AI基础设施
##AI生成
#文章总结
##总结
###耀途分享

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M
#NLP

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
#AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
##软硬件优化
##GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
##数据处理与发现
###Trifacta $100M
#### $31M
##数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
##数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
##向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
##深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
##机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
##AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
#MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
##Feature Store:
###Tecton：$35M
##model monitoring
###Arthur AI $15M
##Feature Discovery
####explorium $31M
##向量搜索
###Zilliz
###Pinecone
###tecton.ai
##数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
##安全
###Robust Intelligence $11M
###RealAI
##可解释性
####Aporia
##隐私
####DID
##边缘AI
###开放智能
####Deci AI $9.1M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infra
### Rasa $26M
### Grid AI $18.6M
### Hugging Face $15M
### cnvrg.io 被intel收购
## 软硬件优化
## GPU虚拟化
### 趋动科技
### #RunAI 
### #bitfusion
## 数据处理与发现
### Trifacta $100M
### # $31M
## 数据合成
### Ai.reverie: $5.6M
### #DataGen Technologies $3.5M
## 数据标注
### Scale.ai :$155M 
### Labelbox: $40M
### #Dataloop AI $11M
### Snorkel AI: $12M
## 向量搜索与数据库
### ZilliZ milvus 4300万美元
### Jina AI 600万美元
### Pinecone $10M
## 深度学习框架
### 一流科技：OneFlow 5000万人民币
### Skymind:DL4J
### Weights&Biases：4500万美元
## 机器学习平台
### DataRobot: $270M 
### Dataiku：$100M
### H2O.ai：$72.5M
### domino data：$43M
### abacus.ai $22M 
### RapidMiner：$16M
### Machinify：$10M
### 第四范式：7亿美元
### 和鲸科技 数百万美元
## AutoML
### 星环科技 5亿人民币
### 行动贝果 3443万人民币
### 探智立方 DarwinML 数百万美元
### 江苏鸿程
### #Allegro.AI: $11M
### 大公司
# MLops
### Saagie €25M
### Algorithmia: $25M
### #iguazio $24M
### Determined AI：$11M
### Spell $15M
### Verta $10M
### Fiddler Labs $10.2M
### Pecan $11M
### Allegro.ai  $11M
### #SuperWise $4.5M
### #Comet.ml $4.5
### datatron $1.4M
### Seldon £7.1
### Evidently ai
### #ParallelM 被DataRobot收购
### H2O.ai
## Feature Store:
### Tecton：$35M
## model monitoring
### Arthur AI $15M
## Feature Discovery
### #explorium $31M
## 向量搜索
### Zilliz
### Pinecone
### tecton.ai
## 数据版本和共享社区
### Pachyderm $16M
### Graviti 千万级美元
### # DAGsHub $3M
### 和鲸科技
## 安全
### Robust Intelligence $11M
### RealAI
## 可解释性
### #Aporia
## 隐私
### #DID
## 边缘AI
### 开放智能
### #Deci AI $9.1M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infra
###Rasa $26M
###Grid AI $18.6M
###Hugging Face $15M
###cnvrg.io 被intel收购
## 软硬件优化
###OctoML $15M
###Neural magic $15M
###Weka.IO $31.7M
## GPU虚拟化
###趋动科技
####RunAI 
####bitfusion
## 数据处理与发现
###Trifacta $100M
#### $31M
## 数据合成
###Ai.reverie: $5.6M
####DataGen Technologies $3.5M
## 数据标注
###Scale.ai :$155M 
###Labelbox: $40M
####Dataloop AI $11M
###Snorkel AI: $12M
## 向量搜索与数据库
###ZilliZ milvus 4300万美元
###Jina AI 600万美元
###Pinecone $10M
## 深度学习框架
###一流科技：OneFlow 5000万人民币
###Skymind:DL4J
###Weights&Biases：4500万美元
## 机器学习平台
###DataRobot: $270M 
###Dataiku：$100M
###H2O.ai：$72.5M
###domino data：$43M
###abacus.ai $22M 
###RapidMiner：$16M
###Machinify：$10M
###第四范式：7亿美元
###和鲸科技 数百万美元
## AutoML
###星环科技 5亿人民币
###行动贝果 3443万人民币
###探智立方 DarwinML 数百万美元
###江苏鸿程
####Allegro.AI: $11M
###大公司
###微软NNI
###亚马逊AutoGluon
###谷歌
# MLops
###Saagie €25M
###Algorithmia: $25M
####iguazio $24M
###Determined AI：$11M
###Spell $15M
###Verta $10M
###Fiddler Labs $10.2M
###Pecan $11M
###Allegro.ai  $11M
####SuperWise $4.5M
####Comet.ml $4.5
###datatron $1.4M
###Seldon £7.1
###Evidently ai
####ParallelM 被DataRobot收购
###H2O.ai
## Feature Store:
###Tecton：$35M
## model monitoring
###Arthur AI $15M
###databand.ai $14.5M
###WhyLabs $4M
## Feature Discovery
####explorium $31M
## 向量搜索
###Zilliz
###Pinecone
###tecton.ai
## 数据版本和共享社区
###Pachyderm $16M
###Graviti 千万级美元
#### DAGsHub $3M
###和鲸科技
## 安全
###Robust Intelligence $11M
###RealAI
## 可解释性
###Fiddler labs $10.2M
###InterpretML
###RealAI
####Aporia
## 隐私
####DID
## 边缘AI
###开放智能
####Deci AI $9.1M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infrastructure
####Rasa $26M
####Grid AI $18.6M
####Hugging Face $15M
####cnvrg.io 被intel收购
### 软硬件优化
####OctoML $15M
####Neural magic $15M
####Weka.IO $31.7M
### GPU虚拟化
####趋动科技
#####RunAI 
#####bitfusion
### 数据处理与发现
####Trifacta $100M
##### $31M
### 数据合成
####Ai.reverie: $5.6M
#####DataGen Technologies $3.5M
### 数据标注
####Scale.ai :$155M 
####Labelbox: $40M
#####Dataloop AI $11M
####Snorkel AI: $12M
### 向量搜索与数据库
####ZilliZ milvus 4300万美元
####Jina AI 600万美元
####Pinecone $10M
### 深度学习框架
####一流科技：OneFlow 5000万人民币
####Skymind:DL4J
####Weights&Biases：4500万美元
### 机器学习平台
####DataRobot: $270M 
####Dataiku：$100M
####H2O.ai：$72.5M
####domino data：$43M
####abacus.ai $22M 
####RapidMiner：$16M
####Machinify：$10M
####第四范式：7亿美元
### AutoML
####星环科技 5亿人民币
####行动贝果 3443万人民币
####探智立方 DarwinML 数百万美元
####江苏鸿程
#####Allegro.AI: $11M
####大公司
####微软NNI
####亚马逊AutoGluon
####谷歌
### MLops
####Saagie €25M
####Algorithmia: $25M
#####iguazio $24M
####Determined AI：$11M
####Spell $15M
####Verta $10M
####Pecan $11M
####Allegro.ai  $11M
#####SuperWise $4.5M
#####Comet.ml $4.5
####datatron $1.4M
####Seldon £7.1
####Evidently ai
#####ParallelM 被DataRobot收购
####H2O.ai
### Feature Store:
####Tecton：$35M
### model monitoring
####Arthur AI $15M
####databand.ai $14.5M
####WhyLabs $4M
### Feature Discovery
#####explorium $31M
### 边缘MLops
####开放智能Open AI LAB
#####Deci AI $9.1M
### 向量搜索
####Zilliz
####Pinecone
####tecton.ai
### 数据版本和共享社区
####Pachyderm $16M
####Graviti 千万级美元
##### DAGsHub $3M
####和鲸科技 数百万美元
### 可解释性
####Fiddler labs $10.2M
####InterpretML
####RealAI
#####Aporia
### 安全与隐私
####Robust Intelligence $11M
####RealAI
#####DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infrastructure
#### Rasa $26M
#### Grid AI $18.6M
#### Hugging Face $15M
#### cnvrg.io 被intel收购
### 软硬件优化
#### OctoML $15M
#### Neural magic $15M
#### Weka.IO $31.7M
### GPU虚拟化
#### 趋动科技
#### #RunAI 
#### #bitfusion
### 数据处理与发现
#### Trifacta $100M
#### # $31M
### 数据合成
#### Ai.reverie: $5.6M
#### #DataGen Technologies $3.5M
### 数据标注
#### Scale.ai :$155M 
#### Labelbox: $40M
#### #Dataloop AI $11M
#### Snorkel AI: $12M
### 向量搜索与数据库
#### ZilliZ milvus 4300万美元
#### Jina AI 600万美元
#### Pinecone $10M
### 深度学习框架
#### 一流科技：OneFlow 5000万人民币
#### Skymind:DL4J
#### Weights&Biases：4500万美元
### 机器学习平台
#### DataRobot: $270M 
#### Dataiku：$100M
#### H2O.ai：$72.5M
#### domino data：$43M
#### abacus.ai $22M 
#### RapidMiner：$16M
#### Machinify：$10M
#### 第四范式：7亿美元
### AutoML
#### 星环科技 5亿人民币
#### 行动贝果 3443万人民币
#### 探智立方 DarwinML 数百万美元
#### 江苏鸿程
#### #Allegro.AI: $11M
#### 大公司
#### 微软NNI
#### 亚马逊AutoGluon
#### 谷歌
### MLops
#### Saagie €25M
#### Algorithmia: $25M
#### #iguazio $24M
#### Determined AI：$11M
#### Spell $15M
#### Verta $10M
#### Pecan $11M
#### Allegro.ai  $11M
#### #SuperWise $4.5M
#### #Comet.ml $4.5
#### datatron $1.4M
#### Seldon £7.1
#### Evidently ai
#### #ParallelM 被DataRobot收购
#### H2O.ai
### Feature Store:
#### Tecton：$35M
### model monitoring
#### Arthur AI $15M
#### databand.ai $14.5M
#### WhyLabs $4M
### Feature Discovery
#### #explorium $31M
### 边缘MLops
#### 开放智能Open AI LAB
#### #Deci AI $9.1M
### 向量搜索
#### Zilliz
#### Pinecone
#### tecton.ai
### 数据版本和共享社区
#### Pachyderm $16M
#### Graviti 千万级美元
#### # DAGsHub $3M
#### 和鲸科技 数百万美元
### 可解释性
#### Fiddler labs $10.2M
#### InterpretML
#### RealAI
#### #Aporia
### 安全与隐私
#### Robust Intelligence $11M
#### RealAI
#### #DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infrastructure
##### Rasa $26M
##### Grid AI $18.6M
##### Hugging Face $15M
##### cnvrg.io 被intel收购
### 软硬件优化
##### OctoML $15M
##### Neural magic $15M
##### Weka.IO $31.7M
### GPU虚拟化
##### 趋动科技
##### #RunAI 
##### #bitfusion
### 数据处理与发现
##### Trifacta $100M
##### # $31M
### 数据合成
#### Ai.reverie: $5.6M
#### #DataGen Technologies $3.5M
### 数据标注
##### Scale.ai :$155M 
##### Labelbox: $40M
##### #Dataloop AI $11M
##### Snorkel AI: $12M
### 向量搜索与数据库
##### ZilliZ milvus 4300万美元
##### Jina AI 600万美元
##### Pinecone $10M
### 深度学习框架
##### 一流科技：OneFlow 5000万人民币
##### Skymind:DL4J
##### Weights&Biases：4500万美元
### 机器学习平台
##### DataRobot: $270M 
##### Dataiku：$100M
##### H2O.ai：$72.5M
##### domino data：$43M
##### abacus.ai $22M 
##### RapidMiner：$16M
##### Machinify：$10M
##### 第四范式：7亿美元
### AutoML
##### 星环科技 5亿人民币
##### 行动贝果 3443万人民币
##### 探智立方 DarwinML 数百万美元
##### 江苏鸿程
##### #Allegro.AI: $11M
#### 大公司
##### 微软NNI
##### 亚马逊AutoGluon
##### 谷歌
### MLops
##### Saagie €25M
##### Algorithmia: $25M
##### #iguazio $24M
##### Determined AI：$11M
##### Spell $15M
##### Verta $10M
##### Pecan $11M
##### Allegro.ai  $11M
##### #SuperWise $4.5M
#### #Comet.ml $4.5
#### datatron $1.4M
#### Seldon £7.1
#### Evidently ai
#### #ParallelM 被DataRobot收购
#### H2O.ai
### Feature Store:
#### Tecton：$35M
### model monitoring
##### Arthur AI $15M
##### databand.ai $14.5M
##### WhyLabs $4M
### Feature Discovery
##### #explorium $31M
### 边缘MLops
##### 开放智能Open AI LAB
##### #Deci AI $9.1M
### 向量搜索
##### Zilliz
##### Pinecone
##### tecton.ai
### 数据版本和共享社区
##### Pachyderm $16M
##### Graviti 千万级美元
##### # DAGsHub $3M
##### 和鲸科技 数百万美元
### 可解释性
##### Fiddler labs $10.2M
##### InterpretML
##### RealAI
#### #Aporia
### 安全与隐私
##### Robust Intelligence $11M
##### RealAI
##### #DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infrastructure
*Rasa $26M
*Grid AI $18.6M
*Hugging Face $15M
*cnvrg.io 被intel收购
### 软硬件优化
*OctoML $15M
*Neural magic $15M
*Weka.IO $31.7M
### GPU虚拟化
*趋动科技
*#RunAI 
*#bitfusion
### 数据处理与发现
*Trifacta $100M
*# $31M
### 数据合成
#### Ai.reverie: $5.6M
#### #DataGen Technologies $3.5M
### 数据标注
*Scale.ai :$155M 
*Labelbox: $40M
*#Dataloop AI $11M
*Snorkel AI: $12M
### 向量搜索与数据库
*ZilliZ milvus 4300万美元
*Jina AI 600万美元
*Pinecone $10M
### 深度学习框架
*一流科技：OneFlow 5000万人民币
*Skymind:DL4J
*Weights&Biases：4500万美元
### 机器学习平台
*DataRobot: $270M 
*Dataiku：$100M
*H2O.ai：$72.5M
*domino data：$43M
*abacus.ai $22M 
*RapidMiner：$16M
*Machinify：$10M
*第四范式：7亿美元
### AutoML
*星环科技 5亿人民币
*行动贝果 3443万人民币
*探智立方 DarwinML 数百万美元
*江苏鸿程
*#Allegro.AI: $11M
#### 大公司
*微软NNI
*亚马逊AutoGluon
*谷歌
### MLops
*Saagie €25M
*Algorithmia: $25M
*#iguazio $24M
*Determined AI：$11M
*Spell $15M
*Verta $10M
*Pecan $11M
*Allegro.ai  $11M
*#SuperWise $4.5M
#### #Comet.ml $4.5
#### datatron $1.4M
#### Seldon £7.1
#### Evidently ai
#### #ParallelM 被DataRobot收购
#### H2O.ai
### Feature Store:
#### Tecton：$35M
### model monitoring
*Arthur AI $15M
*databand.ai $14.5M
*WhyLabs $4M
### Feature Discovery
*#explorium $31M
### 边缘MLops
*开放智能Open AI LAB
*#Deci AI $9.1M
### 向量搜索
*Zilliz
*Pinecone
*tecton.ai
### 数据版本和共享社区
*Pachyderm $16M
*Graviti 千万级美元
*# DAGsHub $3M
*和鲸科技 数百万美元
### 可解释性
*Fiddler labs $10.2M
*InterpretML
*RealAI
#### #Aporia
### 安全与隐私
*Robust Intelligence $11M
*RealAI
*#DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# AI infrastructure
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### GPU虚拟化
* 趋动科技
* #RunAI 
* #bitfusion
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
#### Ai.reverie: $5.6M
#### #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
#### 大公司
* 微软NNI
* 亚马逊AutoGluon
* 谷歌
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
#### #Comet.ml $4.5
#### datatron $1.4M
#### Seldon £7.1
#### Evidently ai
#### #ParallelM 被DataRobot收购
#### H2O.ai
### Feature Store:
#### Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* # DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
# Contributed by Warren Wen
# AI infrastructure
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### GPU虚拟化
* 趋动科技
* #RunAI 
* #bitfusion
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
#### Ai.reverie: $5.6M
#### #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
#### 大公司
* 微软NNI
* 亚马逊AutoGluon
* 谷歌
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
#### #Comet.ml $4.5
#### datatron $1.4M
#### Seldon £7.1
#### Evidently ai
#### #ParallelM 被DataRobot收购
#### H2O.ai
### Feature Store:
#### Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* # DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen
# AI infrastructure
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### GPU虚拟化
* 趋动科技
* #RunAI 
* #bitfusion
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
#### 大公司
* 微软NNI
* 亚马逊AutoGluon
* 谷歌
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
#### #Comet.ml $4.5
#### datatron $1.4M
#### Seldon £7.1
#### Evidently ai
#### #ParallelM 被DataRobot收购
#### H2O.ai
### Feature Store:
#### Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* # DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen
#表示以色列公司
# AI infrastructure
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### GPU虚拟化
* 趋动科技
* #RunAI 
* #bitfusion
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
#### 大公司
* 微软NNI
* 亚马逊AutoGluon
* 谷歌
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen
#表示以色列公司
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### GPU虚拟化
* 趋动科技
* #RunAI 
* #bitfusion
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py

# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen
#表示以色列公司
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % 
wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen
#表示以色列公司
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
#### #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % clear                 

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* # $31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* #Explorium.ai$31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 向量搜索
* Zilliz
* Pinecone
* tecton.ai
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* #Explorium.ai$31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* #Explorium.ai$31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
### Experiment Tracking:
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
* 大公司
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* #Explorium.ai$31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
### Experiment Tracking:
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* RealAI
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* RealAI
* #DID
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence
# 人工智能创业公司调研
Contributed by Warren Wen

#表示以色列公司
举例：Scale.ai :$155M
表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
### 软硬件优化
* OctoML $15M
* Neural magic $15M
* Weka.IO $31.7M
### 异构加速器虚拟化
* 趋动科技 数亿元人民币
* #RunAI $30M
* #bitfusion 被三星收购
### 数据处理与发现
* Trifacta $100M
* #Explorium.ai$31M
### 数据合成
* Ai.reverie: $5.6M
* #DataGen Technologies $3.5M
### 数据标注
* Scale.ai :$155M 
* Labelbox: $40M
* #Dataloop AI $11M
* Snorkel AI: $12M
### 向量搜索与数据库
* ZilliZ milvus 4300万美元
* Jina AI 600万美元
* Pinecone $10M
### 深度学习框架
* 一流科技：OneFlow 5000万人民币
* Skymind:DL4J
### Experiment Tracking:
* Weights&Biases：4500万美元
### 机器学习平台
* DataRobot: $270M 
* Dataiku：$100M
* H2O.ai：$72.5M
* domino data：$43M
* abacus.ai $22M 
* RapidMiner：$16M
* Machinify：$10M
* 第四范式：7亿美元
### AutoML
* 星环科技 5亿人民币
* 行动贝果 3443万人民币
* 探智立方 DarwinML 数百万美元
* 江苏鸿程
* #Allegro.AI: $11M
### MLops
* Saagie €25M
* Algorithmia: $25M
* #iguazio $24M
* Determined AI：$11M
* Spell $15M
* Verta $10M
* Pecan $11M
* Allegro.ai  $11M
* #SuperWise $4.5M
* #Comet.ml $4.5
* Seldon £7.1
* Evidently ai
* #ParallelM 被DataRobot收购
* H2O.ai
### Feature Store:
* Tecton：$35M
### model monitoring
* Arthur AI $15M
* databand.ai $14.5M
* WhyLabs $4M
### Feature Discovery
* #explorium $31M
### 边缘MLops
* 开放智能Open AI LAB
* #Deci AI $9.1M
### 数据版本和共享社区
* Pachyderm $16M
* Graviti 千万级美元
* #DAGsHub $3M
* 和鲸科技 数百万美元
### 可解释性
* Fiddler labs $10.2M
* InterpretML
* 瑞莱智慧RealAI 数千万人民币
* #Aporia
### 安全与隐私
* Robust Intelligence $11M
* 瑞莱智慧RealAI 数千万人民币
* #D-ID $13.5M
### other
* Rasa $26M
* Grid AI $18.6M
* Hugging Face $15M
* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研
Contributed by Warren Wen

该repo从技术的角度来AI软件创业公司进行分类

#表示以色列公司

举例：Scale.ai :$155M

表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
>### 软硬件优化
>>>* OctoML $15M
>>>* Neural magic $15M
>>>* Weka.IO $31.7M
>### 异构加速器虚拟化
>>>* 趋动科技 数亿元人民币
>>>* #RunAI $30M
>>>* #bitfusion 被三星收购
>### 数据处理与发现
>>>* Trifacta $100M
>>>* #Explorium.ai$31M
>### 数据合成
>>>* Ai.reverie: $5.6M
>>>* #DataGen Technologies $3.5M
>### 数据标注
>>>* Scale.ai :$155M 
>>>* Labelbox: $40M
>>>* #Dataloop AI $11M
>>>* Snorkel AI: $12M
>### 向量搜索与数据库
>>>* ZilliZ milvus 4300万美元
>>>* Jina AI 600万美元
>>>* Pinecone $10M
>### 深度学习框架
>>>* 一流科技：OneFlow 5000万人民币
>>>* Skymind:DL4J
>### Experiment Tracking:
>>>* Weights&Biases：4500万美元
>### 机器学习平台
>>>* DataRobot: $270M 
>>>* Dataiku：$100M
>>>* H2O.ai：$72.5M
>>>* domino data：$43M
>>>* abacus.ai $22M 
>>>* RapidMiner：$16M
>>>* Machinify：$10M
>>>* 第四范式：7亿美元
>### AutoML
>>>* 星环科技 5亿人民币
>>>* 行动贝果 3443万人民币
>>>* 探智立方 DarwinML 数百万美元
>>>* 江苏鸿程
>>>* #Allegro.AI: $11M
>### MLops
>>>* Saagie €25M
>>>* Algorithmia: $25M
>>>* #iguazio $24M
>>>* Determined AI：$11M
>>>* Spell $15M
>>>* Verta $10M
>>>* Pecan $11M
>>>* Allegro.ai  $11M
>>>* #SuperWise $4.5M
>>>* #Comet.ml $4.5
>>>* Seldon £7.1
>>>* Evidently ai
>>>* #ParallelM 被DataRobot收购
>>>* H2O.ai
>### Feature Store:
>>>* Tecton：$35M
>### model monitoring
>>>* Arthur AI $15M
>>>* databand.ai $14.5M
>>>* WhyLabs $4M
>### Feature Discovery
>>>* #explorium $31M
>### 边缘MLops
>>>* 开放智能Open AI LAB
>>>* #Deci AI $9.1M
>### 数据版本和共享社区
>>>* Pachyderm $16M
>>>* Graviti 千万级美元
>>>* #DAGsHub $3M
>>>* 和鲸科技 数百万美元
>### 可解释性
>>>* Fiddler labs $10.2M
>>>* InterpretML
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #Aporia
>### 安全与隐私
>>>* Robust Intelligence $11M
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #D-ID $13.5M
>### other
>>>* Rasa $26M
>>>* Grid AI $18.6M
>>>* Hugging Face $15M
>>>* cnvrg.io 被intel收购

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研
Contributed by Warren Wen

该repo从技术的角度来AI软件创业公司进行分类

#表示以色列公司

举例：Scale.ai :$155M

表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
>### 软硬件优化
>>>* OctoML $15M
>>>* Neural magic $15M
>>>* Weka.IO $31.7M
>### 异构加速器虚拟化
>>>* 趋动科技 数亿元人民币
>>>* #RunAI $30M
>>>* #bitfusion 被三星收购
>### 数据处理与发现
>>>* Trifacta $100M
>>>* #Explorium.ai$31M
>### 数据合成
>>>* Ai.reverie: $5.6M
>>>* #DataGen Technologies $3.5M
>### 数据标注
>>>* Scale.ai :$155M 
>>>* Labelbox: $40M
>>>* #Dataloop AI $11M
>>>* Snorkel AI: $12M
>### 向量搜索与数据库
>>>* ZilliZ milvus 4300万美元
>>>* Jina AI 600万美元
>>>* Pinecone $10M
>### 深度学习框架
>>>* 一流科技：OneFlow 5000万人民币
>>>* Skymind:DL4J
>### Experiment Tracking:
>>>* Weights&Biases：4500万美元
>### 机器学习平台
>>>* DataRobot: $270M 
>>>* Dataiku：$100M
>>>* H2O.ai：$72.5M
>>>* domino data：$43M
>>>* abacus.ai $22M 
>>>* RapidMiner：$16M
>>>* Machinify：$10M
>>>* 第四范式：7亿美元
>### AutoML
>>>* 星环科技 5亿人民币
>>>* 行动贝果 3443万人民币
>>>* 探智立方 DarwinML 数百万美元
>>>* 江苏鸿程
>>>* #Allegro.AI: $11M
>### MLops
>>>* Saagie €25M
>>>* Algorithmia: $25M
>>>* #iguazio $24M
>>>* Determined AI：$11M
>>>* Spell $15M
>>>* Verta $10M
>>>* Pecan $11M
>>>* Allegro.ai  $11M
>>>* #SuperWise $4.5M
>>>* #Comet.ml $4.5
>>>* Seldon £7.1
>>>* Evidently ai
>>>* #ParallelM 被DataRobot收购
>>>* H2O.ai
>### Feature Store:
>>>* Tecton：$35M
>### model monitoring
>>>* Arthur AI $15M
>>>* databand.ai $14.5M
>>>* WhyLabs $4M
>### Feature Discovery
>>>* #explorium $31M
>### 边缘MLops
>>>* 开放智能Open AI LAB
>>>* #Deci AI $9.1M
>### 数据版本和共享社区
>>>* Pachyderm $16M
>>>* Graviti 千万级美元
>>>* #DAGsHub $3M
>>>* 和鲸科技 数百万美元
>### 可解释性
>>>* Fiddler labs $10.2M
>>>* InterpretML
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #Aporia
>### 安全与隐私
>>>* Robust Intelligence $11M
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #D-ID $13.5M
>### other
>>>* Rasa $26M
>>>* Grid AI $18.6M
>>>* Hugging Face $15M
>>>* cnvrg.io 被intel收购
## NLP
>### 综合
>>>* 达观数据 2.7亿人民币
>### 机器翻译
>>>* Unbabel：众包 $60M
>>>* Lilt $25M
>>>* *推文科技：网络小说翻译 1000万人民币 联想之星
>>>* *Atman：医药文献翻译 560万美元 北极光
>### 文本重写
>>>* Grammarly $90M
>### Chatbot
>>#### Automated CX
>>>* Ada Support $44M
>>#### 智能客服
>>>* 追一科技 4100万美元
>>>* 智齿科技 2.1亿人民币
>>>* 晓多科技 超2亿人民币
>>>* 乐言科技 1.5亿人民币
>>#### 心理健康
>>>* Woebot Labs  $22.8M 心理健康聊天机器人
>>#### 运维
>>>* Moveworks $75M
>>#### 其他
>>>* Troops.ai $12M
>### 背景调查
>>>* Checkr $160M
>>>* Middesk $4M
>>>* i背调：数千万人民币
>### 招聘
>>>* Eightfold $125M
>>>* Turing.com $32M
>>>* e成科技 8000万美元
>>>* Bello倍罗 数千万人民币
>>>* 近屿智能 数千万人民币
>>>* 方便面面试
>>>* Pyxai $150K
>### 合同审查
>>>* Kira systems CA$65M
>### 销售
>>>* #Gong.io
>>>* #chorus.ai
>>>* People.ai
>>>* Troops.ai
>>>* Tact.AI 
>>>* Recurrent.ai
>>>* 客知音
>>>* 深维智信
>>>* Sales enablement
>### 其他
>>>* # A21 labs
>>>* Golden $14.5M
>>>* ClearGraph 被收购
>>>* UpCodes $3.4M
## Vision
>>#### 技术路线
>### 综合
>>>* 商汤
>>>* 旷世
>>>* 依图
>>>* 云从
>>>* 图普科技
>### 动作捕捉
>>#### 诺亦腾
>>#### Xmov
>>>* 

>### 创作工具
>>>* Canva $60M, $8.7B
>>>* Figma $50M, $2B 
>>>* InVisionApp $115M, $1.9B
>>>* Runway $8.5M
>>>* Beautiful.AI $11M
>>>* GliaCloud
>>>* 来画视频 5000万人民币
>>#### 漫画
>### 图像压缩
>>>* 图鸭科技 数千万人民币
>### 渲染
>>>* 个人总结：
>>>* 51world
>>>* 粒界科技
>>>* 叠境
>>>* RestAR
>>>* 酷家乐
>>>* 迈吉客科技
>>>* 商询科技 datamesh
>>>* 时谛智能
>### 形象生成
>>>* Brud $20M $125M
>>>* FaceRig $2M
>>>* EmbodyMe
>>>* Xmov魔珐科技 数亿人民币
>>>* 相芯科技 1.2亿人民币
>>>* 迈吉客科技 数千万人民币
>>>* 诗云科技 数百万美金
>>>* ZMO.ai
>>>* 像素偏移
>>>* 慧夜科技
>>>* 我是大咖
>>>* 
>>>* #D-ID $13.5M
>### 视频录制
>>#### 
>>#### Loom
>### 视频
>>#### Viedeo++
>>#### 影普科技
>>#### Kapwing
>>#### 视频异常分析
>>>* 闪马智能
>### OCR
>>>* HyperScience $80M
>### 视频广告
>>>* #KERV Interactive $11M
>### 无人零售
>>#### Grabango
>>#### Standard Cognition
>>#### Mad Street Den
>### 时尚
>>>* 深尚科技
>### 安防
>>>* #AnyVision  $43M
>>#### tractable.ai
>### 视频异常
>>>* 闪马智能：近亿元人民币
>### 测试
>>>* #Applitools $31M
>### 医学影像
>>>* 连心医疗：9000万人民币
>### 其他
>>>* Akasha Imaging
>>>* 墨奇科技
## Audio/speech
>### 音乐
>>>* Amper Music
>>>* StepBeats
>### 语音
>>>* Descript
>>>* DeepGram
>>>* Otter.ai $50M
>>>* 魔音助手 5000万美元
>>>* 思必驰：端侧
>>>* 云知声：云
>### 声纹识别
>>#### VoiceAI 
>>#### SpeakIn
>### 反欺诈
>>>* Pindrop  $90M
>### CRM
>>#### Troops.ai
>### 医药
>>>* Suki $20M
## 个性化推荐
>>>* Attentive $230M
>>>* Outlier $22.1M
>>>* Lily $12.5M
## 决策智能
>### 研究 
>>#### 运筹学
>>#### 分类：
>>#### 线性规划（Linear Programming）
>>#### 整数规划（Integer Programming）问题
>>#### 总结
>### 强化学习
>>#### 综合
>>>* 启元世界
>>>* 南栖仙策
>>#### 游戏
>>>* %DeepMind
>>>* 超参数科技
>>>* 启元世界
>>>* Rct
>>#### 调度
>>>* %secondmind.ai $24M
>>#### 测试
>>>* Test.ai $11M
>>>* Testim $10M
>>>* Mabl $20M
>>#### 机器人
>>>* Osaro $37M
>>#### RPA
>>>* FortressIQ $30M
>### 运筹优化
>>>* 杉树科技 近亿元人民币
>>>* 悠桦林 近亿人民币
>>>* 智因科技 
>>>* 宾通智能
>>>* nextMV $8M
## Next generation AI 
>>>* Gamalon $20M
## 场景AI
>### 工业检测
>>>* 深度视觉
>### 智能运维
>>>* 擎创科技 千万级美元
>>>* 必示科技 1.5亿人民币
>>>* 云兴维智 数千万人民币
>### RPA
>>>* Uiptah $750M
>>>* Automation Anywhere $290M
>>>* 来也科技 4200万美元
>>>* 弘玑Cyclone 近4000万美元
>>>* 云扩科技 3000万美元
>>>* 影刀RPA
## 行业AI
>>#### 零售
>>>* ImageDT图匠数据：千万级美元
>### 教育
>>>* 松鼠AI：10亿人民币
>### 农业
>>>* Hypersonix $11.5M
>>>* 爱科农：
>>>* 极飞科技：12亿人民币
>### 法律
>>>* Ross Intelligence
>>>* Atrium LTS
>>>* DoNotPays
>>>* 幂律智能
>>>* 秘塔
>### 金融
>>#### 智能投顾/投研
>>>* Wealthfront $75M
>>>* Kensho $550M 收购
>>>* 
>>>* 香侬科技：1.1亿人民币
>>>* 虎博科技：3300万美元
>>>* 阿法金融
>>>* eBrain
>>>* 倍漾科技
>>>* 卡方科技
>>>* 弘量研究
>>>* 贝塔数据
>>#### 风控
>>>* 同盾科技：1亿美金
>>>* Datavisor: 4000万美元
>>>* 慧安金科: 1亿人民币
>>#### 反欺诈
>>>* Sift Science $53M
>>>* DataVisor，4000万美元
>>>* Simility 1.2亿美金被收购
>>>* 新加坡的CashShield, GGV 2000万美元
>>>* 特拉维夫的Forter,  5000万美元
>>>* 巴黎的Shift Technology，6000万美元，accel
>>>* 英国的Featurespace, 3000万美元
>>>* Signifyd 1亿美元
>>>* SentiLink
>>>* UnifyID
>>>* Tessian $42M
>>>* Tara AI $10M
>### 医疗
>>>* 总结
>>>* 连心医疗：9000万人名币
>>>* 麦歌算法
>### 制药
>>>* 晶泰科技：3.188亿美元 全球最高的AI药研公司
>>>* 望石智慧
>>>* 费米子科技：上亿元
>>>* Recursion Pharmaceuticals
>### 服装
>### 
>>>* 智布：1亿美元
>>>* 极睿科技：亿元级人民币
>>>* 时谛智能：近亿人民币
>### 房地产
>>>* Skyline AI
>### 物流
>>>* 快运兔
>### 工业
>>>* Augury $55M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研
Contributed by Warren Wen

该repo从技术的角度来AI软件创业公司进行分类

#表示以色列公司

举例：Scale.ai :$155M

表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
>### 软硬件优化
>>>* OctoML $15M
>>>* Neural magic $15M
>>>* Weka.IO $31.7M
>### 异构加速器虚拟化
>>>* 趋动科技 数亿元人民币
>>>* #RunAI $30M
>>>* #bitfusion 被三星收购
>### 数据处理与发现
>>>* Trifacta $100M
>>>* #Explorium.ai$31M
>### 数据合成
>>>* Ai.reverie: $5.6M
>>>* #DataGen Technologies $3.5M
>### 数据标注
>>>* Scale.ai :$155M 
>>>* Labelbox: $40M
>>>* #Dataloop AI $11M
>>>* Snorkel AI: $12M
>### 向量搜索与数据库
>>>* ZilliZ milvus 4300万美元
>>>* Jina AI 600万美元
>>>* Pinecone $10M
>### 深度学习框架
>>>* 一流科技：OneFlow 5000万人民币
>>>* Skymind:DL4J
>### Experiment Tracking:
>>>* Weights&Biases：4500万美元
>### 机器学习平台
>>>* DataRobot: $270M 
>>>* Dataiku：$100M
>>>* H2O.ai：$72.5M
>>>* domino data：$43M
>>>* abacus.ai $22M 
>>>* RapidMiner：$16M
>>>* Machinify：$10M
>>>* 第四范式：7亿美元
>### AutoML
>>>* 星环科技 5亿人民币
>>>* 行动贝果 3443万人民币
>>>* 探智立方 DarwinML 数百万美元
>>>* 江苏鸿程
>>>* #Allegro.AI: $11M
>### MLops
>>>* Saagie €25M
>>>* Algorithmia: $25M
>>>* #iguazio $24M
>>>* Determined AI：$11M
>>>* Spell $15M
>>>* Verta $10M
>>>* Pecan $11M
>>>* Allegro.ai  $11M
>>>* #SuperWise $4.5M
>>>* #Comet.ml $4.5
>>>* Seldon £7.1
>>>* Evidently ai
>>>* #ParallelM 被DataRobot收购
>>>* H2O.ai
>### Feature Store:
>>>* Tecton：$35M
>### model monitoring
>>>* Arthur AI $15M
>>>* databand.ai $14.5M
>>>* WhyLabs $4M
>### Feature Discovery
>>>* #explorium $31M
>### 边缘MLops
>>>* 开放智能Open AI LAB
>>>* #Deci AI $9.1M
>### 数据版本和共享社区
>>>* Pachyderm $16M
>>>* Graviti 千万级美元
>>>* #DAGsHub $3M
>>>* 和鲸科技 数百万美元
>### 可解释性
>>>* Fiddler labs $10.2M
>>>* InterpretML
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #Aporia
>### 安全与隐私
>>>* Robust Intelligence $11M
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #D-ID $13.5M
>### other
>>>* Rasa $26M
>>>* Grid AI $18.6M
>>>* Hugging Face $15M
>>>* cnvrg.io 被intel收购
## 文本NLP
>### 综合
>>>* 达观数据 2.7亿人民币
>### 机器翻译
>>>* Unbabel：众包 $60M
>>>* Lilt $25M
>>>* *推文科技：网络小说翻译 1000万人民币 联想之星
>>>* *Atman：医药文献翻译 560万美元 北极光
>### 文本重写
>>>* Grammarly $90M
>### Chatbot
>>#### Automated CX
>>>* Ada Support $44M
>>#### 智能客服
>>>* 追一科技 4100万美元
>>>* 智齿科技 2.1亿人民币
>>>* 晓多科技 超2亿人民币
>>>* 乐言科技 1.5亿人民币
>>#### 心理健康
>>>* Woebot Labs  $22.8M 心理健康聊天机器人
>>#### 运维
>>>* Moveworks $75M
>>#### 其他
>>>* Troops.ai $12M
>### 背景调查
>>>* Checkr $160M
>>>* Middesk $4M
>>>* i背调：数千万人民币
>### 招聘
>>>* Eightfold $125M
>>>* Turing.com $32M
>>>* e成科技 8000万美元
>>>* Bello倍罗 数千万人民币
>>>* 近屿智能 数千万人民币
>>>* 方便面面试
>>>* Pyxai $150K
>### 合同审查
>>>* Kira systems CA$65M
>### 销售
>>>* #Gong.io $200M
>>>* #chorus.ai $45M
>>>* People.ai $60M
>>>* Tact.AI  $27M
>>>* Troops.ai $12M
>>>* Recurrent.ai
>### 水下
>>>* 客知音
>>>* 深维智信
>>>* Sales enablement
>### 其他
>>>* # A21 labs
>>>* Golden $14.5M
>>>* ClearGraph 被收购
>>>* UpCodes $3.4M
## 视觉Vision
>>#### 研究
>### 综合
>>>* 商汤 10亿美元
>>>* 旷世 7.5亿美元
>>>* 依图 2亿美元
>>>* 云从 18亿人民币
>>>* 图普科技 千万美元
>### 动作捕捉
>>#### 诺亦腾
>>#### Xmov
>>>* 

>### 创作工具
>>>* Canva $60M, $8.7B
>>>* Figma $50M, $2B 
>>>* InVisionApp $115M, $1.9B
>>>* Runway $8.5M
>>>* Beautiful.AI $11M
>>>* GliaCloud
>>>* 来画视频 5000万人民币
>>#### 漫画
>### 图像压缩
>>>* 图鸭科技 数千万人民币
>### 渲染
>>>* 个人总结：
>>>* 51world
>>>* 粒界科技
>>>* 叠境
>>>* RestAR
>>>* 酷家乐
>>>* 迈吉客科技
>>>* 商询科技 datamesh
>>>* 时谛智能
>### 形象生成
>>>* Brud $20M $125M
>>>* FaceRig $2M
>>>* EmbodyMe
>>>* Xmov魔珐科技 数亿人民币
>>>* 相芯科技 1.2亿人民币
>>>* 迈吉客科技 数千万人民币
>>>* 诗云科技 数百万美金
>>>* ZMO.ai
>>>* 像素偏移
>>>* 慧夜科技
>>>* 我是大咖
>>>* 
>>>* #D-ID $13.5M
>### 视频录制
>>#### 
>>#### Loom
>### 视频
>>#### Viedeo++
>>#### 影普科技
>>#### Kapwing
>>#### 视频异常分析
>>>* 闪马智能
>### OCR
>>>* HyperScience $80M
>### 视频广告
>>>* #KERV Interactive $11M
>### 无人零售
>>#### Grabango
>>#### Standard Cognition
>>#### Mad Street Den
>### 时尚
>>>* 深尚科技
>### 安防
>>>* #AnyVision  $43M
>>#### tractable.ai
>### 视频异常
>>>* 闪马智能：近亿元人民币
>### 测试
>>>* #Applitools $31M
>### 医学影像
>>>* 连心医疗：9000万人民币
>### 其他
>>>* Akasha Imaging
>>>* 墨奇科技
## 音频Audio/
>### 语音
>>>* 思必驰：数亿人民币
>>>* 云知声：6亿人民币
>>>* Otter.ai $50M
>>>* Descript $30M
>>>* DeepGram $25M
>>>* 魔音助手 
>### 声纹识别
>>>* 声扬科技VoiceAI 近亿人民币
>>>* SpeakIn
>### 反欺诈
>>>* Pindrop $90M
>### CRM
>>#### Troops.ai
>### 医药
>>>* Suki $20M
>### 音乐
>>>* Amper Music $4M
>>>* StepBeats 150万人民币
## 决策
>### 强化学习
>>#### 游戏
>>>* DeepMind
>>>* 超参数科技 3000万美元
>>>* 启元世界 数千万人民币
>>>* rct studio $10M
>>#### 调度
>>>* %secondmind.ai $24M
>>#### 测试
>>>* Mabl $20M
>>>* Test.ai $11M
>>>* Testim $10M
>>#### RPA
>>>* FortressIQ $30M
>>#### 其他
>>>* 南栖仙策
>### 运筹优化
>>>* 杉树科技 近亿元人民币
>>>* 悠桦林 近亿人民币
>>>* 宾通智能 6000万人民币
>>>* 智因科技 
>>>* nextMV $8M
## 场景AI
>### 工业检测
>>>* 深度视觉
>### 智能运维
>>>* 擎创科技 千万级美元
>>>* 必示科技 1.5亿人民币
>>>* 云兴维智 数千万人民币
>### RPA
>>>* Uiptah $750M
>>>* Automation Anywhere $290M
>>>* 来也科技 4200万美元
>>>* 弘玑Cyclone 近4000万美元
>>>* 云扩科技 3000万美元
>>>* 影刀RPA
## 行业AI
>>#### 零售
>>>* ImageDT图匠数据：千万级美元
>### 教育
>>>* 松鼠AI：10亿人民币
>### 农业
>>>* Hypersonix $11.5M
>>>* 爱科农：
>>>* 极飞科技：12亿人民币
>### 法律
>>>* Ross Intelligence
>>>* Atrium LTS
>>>* DoNotPays
>>>* 幂律智能
>>>* 秘塔
>### 金融
>>#### 智能投顾/投研
>>>* Wealthfront $75M
>>>* Kensho $550M 收购
>>>* 
>>>* 香侬科技：1.1亿人民币
>>>* 虎博科技：3300万美元
>>>* 阿法金融
>>>* eBrain
>>>* 倍漾科技
>>>* 卡方科技
>>>* 弘量研究
>>>* 贝塔数据
>>#### 风控
>>>* 同盾科技：1亿美金
>>>* Datavisor: 4000万美元
>>>* 慧安金科: 1亿人民币
>>#### 反欺诈
>>>* Sift Science $53M
>>>* DataVisor，4000万美元
>>>* Simility 1.2亿美金被收购
>>>* 新加坡的CashShield, GGV 2000万美元
>>>* 特拉维夫的Forter,  5000万美元
>>>* 巴黎的Shift Technology，6000万美元，accel
>>>* 英国的Featurespace, 3000万美元
>>>* Signifyd 1亿美元
>>>* SentiLink
>>>* UnifyID
>>>* Tessian $42M
>>>* Tara AI $10M
>### 医疗
>>>* 总结
>>>* 连心医疗：9000万人名币
>>>* 麦歌算法
>### 制药
>>>* 晶泰科技：3.188亿美元 全球最高的AI药研公司
>>>* 望石智慧
>>>* 费米子科技：上亿元
>>>* Recursion Pharmaceuticals
>### 服装
>>>* 智布：1亿美元
>>>* 极睿科技：亿元级人民币
>>>* 时谛智能：近亿人民币
>### 房地产
>>>* Skyline AI
>### 物流
>>>* 快运兔
>### 工业
>>>* Augury $55M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研
Contributed by Warren Wen

该repo从技术的角度来AI软件创业公司进行分类

#表示以色列公司

举例：Scale.ai :$155M

表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
>### 软硬件优化
>>>* OctoML $15M
>>>* Neural magic $15M
>>>* Weka.IO $31.7M
>### 异构加速器虚拟化
>>>* 趋动科技 数亿元人民币
>>>* #RunAI $30M
>>>* #bitfusion 被三星收购
>### 数据处理与发现
>>>* Trifacta $100M
>>>* #Explorium.ai$31M
>### 数据合成
>>>* Ai.reverie: $5.6M
>>>* #DataGen Technologies $3.5M
>### 数据标注
>>>* Scale.ai :$155M 
>>>* Labelbox: $40M
>>>* #Dataloop AI $11M
>>>* Snorkel AI: $12M
>### 向量搜索与数据库
>>>* ZilliZ milvus 4300万美元
>>>* Jina AI 600万美元
>>>* Pinecone $10M
>### 深度学习框架
>>>* 一流科技：OneFlow 5000万人民币
>>>* Skymind:DL4J
>### Experiment Tracking:
>>>* Weights&Biases：4500万美元
>### 机器学习平台
>>>* DataRobot: $270M 
>>>* Dataiku：$100M
>>>* H2O.ai：$72.5M
>>>* domino data：$43M
>>>* abacus.ai $22M 
>>>* RapidMiner：$16M
>>>* Machinify：$10M
>>>* 第四范式：7亿美元
>### AutoML
>>>* 星环科技 5亿人民币
>>>* 行动贝果 3443万人民币
>>>* 探智立方 DarwinML 数百万美元
>>>* 江苏鸿程
>>>* #Allegro.AI: $11M
>### MLops
>>>* Saagie €25M
>>>* Algorithmia: $25M
>>>* #iguazio $24M
>>>* Determined AI：$11M
>>>* Spell $15M
>>>* Verta $10M
>>>* Pecan $11M
>>>* Allegro.ai  $11M
>>>* #SuperWise $4.5M
>>>* #Comet.ml $4.5
>>>* Seldon £7.1
>>>* Evidently ai
>>>* #ParallelM 被DataRobot收购
>>>* H2O.ai
>### Feature Store:
>>>* Tecton：$35M
>### model monitoring
>>>* Arthur AI $15M
>>>* databand.ai $14.5M
>>>* WhyLabs $4M
>### Feature Discovery
>>>* #explorium $31M
>### 边缘MLops
>>>* 开放智能Open AI LAB
>>>* #Deci AI $9.1M
>### 数据版本和共享社区
>>>* Pachyderm $16M
>>>* Graviti 千万级美元
>>>* #DAGsHub $3M
>>>* 和鲸科技 数百万美元
>### 可解释性
>>>* Fiddler labs $10.2M
>>>* InterpretML
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #Aporia
>### 安全与隐私
>>>* Robust Intelligence $11M
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #D-ID $13.5M
>### other
>>>* Rasa $26M
>>>* Grid AI $18.6M
>>>* Hugging Face $15M
>>>* cnvrg.io 被intel收购
## 文本NLP
>### 机器翻译
>>>* Unbabel：$60M
>>>* Lilt：$25M
>>>* 推文科技：1000万人民币
>>>* Atman：560万美元
>### 文本重写
>>>* Grammarly $90M
>### Chatbot
>>#### Automated CX
>>>* Ada Support $44M
>>#### 智能客服
>>>* 追一科技：4100万美元
>>>* 智齿科技：2.1亿人民币
>>>* 晓多科技：超2亿人民币
>>>* 乐言科技：1.5亿人民币
>>#### 心理健康
>>>* Woebot Labs：$22.8M 
>>#### 运维
>>>* Moveworks：$75M
>### 背景调查
>>>* Checkr $160M
>>>* Middesk $4M
>>>* i背调：数千万人民币
>### 招聘
>>>* Eightfold $125M
>>>* Turing.com $32M
>>>* e成科技 8000万美元
>>>* Bello倍罗 数千万人民币
>>>* 近屿智能 数千万人民币
>>>* 方便面面试
>### 合同审查
>>>* Kira systems CA$65M
>### 销售
>>>* #Gong.io $200M
>>>* #chorus.ai $45M
>>>* People.ai $60M
>>>* Tact.AI  $27M
>>>* Troops.ai $12M
>>>* Recurrent.ai
>>>* 客知音 千万级人民币
>>#### 水下
>>>* 深维智信
>### 其他
>>>* 达观数据 2.7亿人民币
>>>* # A21 labs
>>>* Golden $14.5M
>>>* ClearGraph 被收购
>>>* UpCodes $3.4M
## 视觉Vision
>>#### 研究
>### 综合
>>>* 商汤 10亿美元
>>>* 旷世 7.5亿美元
>>>* 依图 2亿美元
>>>* 云从 18亿人民币
>>>* 图普科技 千万美元
>### 动作捕捉
>>#### 诺亦腾
>>#### Xmov
>>>* 

>### 创作工具
>>>* Canva $60M, $8.7B
>>>* Figma $50M, $2B 
>>>* InVisionApp $115M, $1.9B
>>>* Runway $8.5M
>>>* Beautiful.AI $11M
>>>* GliaCloud
>>>* 来画视频 5000万人民币
>>#### 漫画
>### 图像压缩
>>>* 图鸭科技 数千万人民币
>### 渲染
>>>* 个人总结：
>>>* 51world
>>>* 粒界科技
>>>* 叠境
>>>* RestAR
>>>* 酷家乐
>>>* 迈吉客科技
>>>* 商询科技 datamesh
>>>* 时谛智能
>### 形象生成
>>>* Brud $20M $125M
>>>* FaceRig $2M
>>>* EmbodyMe
>>>* Xmov魔珐科技 数亿人民币
>>>* 相芯科技 1.2亿人民币
>>>* 迈吉客科技 数千万人民币
>>>* 诗云科技 数百万美金
>>>* ZMO.ai
>>>* 像素偏移
>>>* 慧夜科技
>>>* 我是大咖
>>>* 
>>>* #D-ID $13.5M
>### 视频录制
>>#### 
>>#### Loom
>### 视频
>>#### Viedeo++
>>#### 影普科技
>>#### Kapwing
>>#### 视频异常分析
>>>* 闪马智能
>### OCR
>>>* HyperScience $80M
>### 视频广告
>>>* #KERV Interactive $11M
>### 无人零售
>>#### Grabango
>>#### Standard Cognition
>>#### Mad Street Den
>### 时尚
>>>* 深尚科技
>### 安防
>>>* #AnyVision  $43M
>>#### tractable.ai
>### 视频异常
>>>* 闪马智能：近亿元人民币
>### 测试
>>>* #Applitools $31M
>### 医学影像
>>>* 连心医疗：9000万人民币
>### 其他
>>>* Akasha Imaging
>>>* 墨奇科技
## 音频Audio/
>### 语音
>>>* 思必驰：数亿人民币
>>>* 云知声：6亿人民币
>>>* Otter.ai $50M
>>>* Descript $30M
>>>* DeepGram $25M
>>>* 魔音助手 
>### 声纹识别
>>>* 声扬科技VoiceAI 近亿人民币
>>>* SpeakIn
>### 反欺诈
>>>* Pindrop $90M
>### CRM
>>#### Troops.ai
>### 医药
>>>* Suki $20M
>### 音乐
>>>* Amper Music $4M
>>>* StepBeats 150万人民币
## 决策
>### 强化学习
>>#### 游戏
>>>* DeepMind
>>>* 超参数科技 3000万美元
>>>* 启元世界 数千万人民币
>>>* rct studio $10M
>>#### 调度
>>>* %secondmind.ai $24M
>>#### 测试
>>>* Mabl $20M
>>>* Test.ai $11M
>>>* Testim $10M
>>#### RPA
>>>* FortressIQ $30M
>>#### 其他
>>>* 南栖仙策
>### 运筹优化
>>>* 杉树科技 近亿元人民币
>>>* 悠桦林 近亿人民币
>>>* 宾通智能 6000万人民币
>>>* 智因科技 
>>>* nextMV $8M
## 场景AI
>### 工业检测
>>>* 深度视觉
>### 智能运维
>>>* 擎创科技 千万级美元
>>>* 必示科技 1.5亿人民币
>>>* 云兴维智 数千万人民币
>### RPA
>>>* Uiptah $750M
>>>* Automation Anywhere $290M
>>>* 来也科技 4200万美元
>>>* 弘玑Cyclone 近4000万美元
>>>* 云扩科技 3000万美元
>>>* 影刀RPA
## 行业AI
>>#### 零售
>>>* ImageDT图匠数据：千万级美元
>### 教育
>>>* 松鼠AI：10亿人民币
>### 农业
>>>* Hypersonix $11.5M
>>>* 爱科农：
>>>* 极飞科技：12亿人民币
>### 法律
>>>* Ross Intelligence
>>>* Atrium LTS
>>>* DoNotPays
>>>* 幂律智能
>>>* 秘塔
>### 金融
>>#### 智能投顾/投研
>>>* Wealthfront $75M
>>>* Kensho $550M 收购
>>>* 
>>>* 香侬科技：1.1亿人民币
>>>* 虎博科技：3300万美元
>>>* 阿法金融
>>>* eBrain
>>>* 倍漾科技
>>>* 卡方科技
>>>* 弘量研究
>>>* 贝塔数据
>>#### 风控
>>>* 同盾科技：1亿美金
>>>* Datavisor: 4000万美元
>>>* 慧安金科: 1亿人民币
>>#### 反欺诈
>>>* Sift Science $53M
>>>* DataVisor，4000万美元
>>>* Simility 1.2亿美金被收购
>>>* 新加坡的CashShield, GGV 2000万美元
>>>* 特拉维夫的Forter,  5000万美元
>>>* 巴黎的Shift Technology，6000万美元，accel
>>>* 英国的Featurespace, 3000万美元
>>>* Signifyd 1亿美元
>>>* SentiLink
>>>* UnifyID
>>>* Tessian $42M
>>>* Tara AI $10M
>### 医疗
>>>* 总结
>>>* 连心医疗：9000万人名币
>>>* 麦歌算法
>### 制药
>>>* 晶泰科技：3.188亿美元 全球最高的AI药研公司
>>>* 望石智慧
>>>* 费米子科技：上亿元
>>>* Recursion Pharmaceuticals
>### 服装
>>>* 智布：1亿美元
>>>* 极睿科技：亿元级人民币
>>>* 时谛智能：近亿人民币
>### 房地产
>>>* Skyline AI
>### 物流
>>>* 快运兔
>### 工业
>>>* Augury $55M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研
Contributed by Warren Wen

该repo从技术的角度来AI软件创业公司进行分类

#表示以色列公司

举例：Scale.ai :$155M

表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
>### 软硬件优化
>>>* OctoML $15M
>>>* Neural magic $15M
>>>* Weka.IO $31.7M
>### 异构加速器虚拟化
>>>* 趋动科技 数亿元人民币
>>>* #RunAI $30M
>>>* #bitfusion 被三星收购
>### 数据处理与发现
>>>* Trifacta $100M
>>>* #Explorium.ai$31M
>### 数据合成
>>>* Ai.reverie: $5.6M
>>>* #DataGen Technologies $3.5M
>### 数据标注
>>>* Scale.ai :$155M 
>>>* Labelbox: $40M
>>>* #Dataloop AI $11M
>>>* Snorkel AI: $12M
>### 向量搜索与数据库
>>>* ZilliZ milvus 4300万美元
>>>* Jina AI 600万美元
>>>* Pinecone $10M
>### 深度学习框架
>>>* 一流科技：OneFlow 5000万人民币
>>>* Skymind:DL4J
>### Experiment Tracking:
>>>* Weights&Biases：4500万美元
>### 机器学习平台
>>>* DataRobot: $270M 
>>>* Dataiku：$100M
>>>* H2O.ai：$72.5M
>>>* domino data：$43M
>>>* abacus.ai $22M 
>>>* RapidMiner：$16M
>>>* Machinify：$10M
>>>* 第四范式：7亿美元
>### AutoML
>>>* 星环科技 5亿人民币
>>>* 行动贝果 3443万人民币
>>>* 探智立方 DarwinML 数百万美元
>>>* 江苏鸿程
>>>* #Allegro.AI: $11M
>### MLops
>>>* Saagie €25M
>>>* Algorithmia: $25M
>>>* #iguazio $24M
>>>* Determined AI：$11M
>>>* Spell $15M
>>>* Verta $10M
>>>* Pecan $11M
>>>* Allegro.ai  $11M
>>>* #SuperWise $4.5M
>>>* #Comet.ml $4.5
>>>* Seldon £7.1
>>>* Evidently ai
>>>* #ParallelM 被DataRobot收购
>>>* H2O.ai
>### Feature Store:
>>>* Tecton：$35M
>### model monitoring
>>>* Arthur AI $15M
>>>* databand.ai $14.5M
>>>* WhyLabs $4M
>### Feature Discovery
>>>* #explorium $31M
>### 边缘MLops
>>>* 开放智能Open AI LAB
>>>* #Deci AI $9.1M
>### 数据版本和共享社区
>>>* Pachyderm $16M
>>>* Graviti 千万级美元
>>>* #DAGsHub $3M
>>>* 和鲸科技 数百万美元
>### 可解释性
>>>* Fiddler labs $10.2M
>>>* InterpretML
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #Aporia
>### 安全与隐私
>>>* Robust Intelligence $11M
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #D-ID $13.5M
>### other
>>>* Rasa $26M
>>>* Grid AI $18.6M
>>>* Hugging Face $15M
>>>* cnvrg.io 被intel收购
## 文本NLP
>### 机器翻译
>>>* Unbabel：$60M
>>>* Lilt：$25M
>>>* 推文科技：1000万人民币
>>>* Atman：560万美元
>### 文本重写
>>>* Grammarly $90M
>### Chatbot
>>#### Automated CX
>>>* Ada Support $44M
>>#### 智能客服
>>>* 追一科技：4100万美元
>>>* 智齿科技：2.1亿人民币
>>>* 晓多科技：超2亿人民币
>>>* 乐言科技：1.5亿人民币
>>#### 心理健康
>>>* Woebot Labs：$22.8M 
>>#### 运维
>>>* Moveworks：$75M
>### 背景调查
>>>* Checkr $160M
>>>* Middesk $4M
>>>* i背调：数千万人民币
>### 招聘
>>>* Eightfold $125M
>>>* Turing.com $32M
>>>* e成科技 8000万美元
>>>* Bello倍罗 数千万人民币
>>>* 近屿智能 数千万人民币
>>>* 方便面面试
>### 合同审查
>>>* Kira systems CA$65M
>### 销售
>>>* #Gong.io $200M
>>>* #chorus.ai $45M
>>>* People.ai $60M
>>>* Tact.AI  $27M
>>>* Troops.ai $12M
>>>* Recurrent.ai
>>>* 客知音 千万级人民币
>>#### 水下
>>>* 深维智信
>### 其他
>>>* 达观数据 2.7亿人民币
>>>* # A21 labs
>>>* Golden $14.5M
>>>* ClearGraph 被收购
>>>* UpCodes $3.4M
## 视觉Vision
>>#### 研究
>### 综合
>>>* 商汤 10亿美元
>>>* 旷世 7.5亿美元
>>>* 依图 2亿美元
>>>* 云从 18亿人民币
>>>* 图普科技 千万美元
>### 动作捕捉
>>#### 诺亦腾
>>#### Xmov
>>>* 

>### 创作工具
>>>* Canva $60M, $8.7B
>>>* Figma $50M, $2B 
>>>* InVisionApp $115M, $1.9B
>>>* Runway $8.5M
>>>* Beautiful.AI $11M
>>>* GliaCloud
>>>* 来画视频 5000万人民币
>>#### 漫画
>### 图像压缩
>>>* 图鸭科技 数千万人民币
>### 渲染
>>>* 个人总结：
>>>* 51world
>>>* 粒界科技
>>>* 叠境
>>>* RestAR
>>>* 酷家乐
>>>* 迈吉客科技
>>>* 商询科技 datamesh
>>>* 时谛智能
>### 形象生成
>>>* Brud $20M $125M
>>>* FaceRig $2M
>>>* EmbodyMe
>>>* Xmov魔珐科技 数亿人民币
>>>* 相芯科技 1.2亿人民币
>>>* 迈吉客科技 数千万人民币
>>>* 诗云科技 数百万美金
>>>* ZMO.ai
>>>* 像素偏移
>>>* 慧夜科技
>>>* 我是大咖
>>>* 
>>>* #D-ID $13.5M
>### 视频录制
>>#### 
>>#### Loom
>### 视频
>>#### Viedeo++
>>#### 影普科技
>>#### Kapwing
>>#### 视频异常分析
>>>* 闪马智能
>### OCR
>>>* HyperScience $80M
>### 视频广告
>>>* #KERV Interactive $11M
>### 无人零售
>>#### Grabango
>>#### Standard Cognition
>>#### Mad Street Den
>### 时尚
>>>* 深尚科技
>### 安防
>>>* #AnyVision  $43M
>>#### tractable.ai
>### 视频异常
>>>* 闪马智能：近亿元人民币
>### 测试
>>>* #Applitools $31M
>### 医学影像
>>>* 连心医疗：9000万人民币
>### 其他
>>>* Akasha Imaging
>>>* 墨奇科技
## 音频Audio
>### 语音
>>>* 思必驰：数亿人民币
>>>* 云知声：6亿人民币
>>>* Otter.ai $50M
>>>* Descript $30M
>>>* DeepGram $25M
>>>* 魔音助手 
>### 声纹识别
>>>* 声扬科技VoiceAI 近亿人民币
>>>* SpeakIn
>### 反欺诈
>>>* Pindrop $90M
>### CRM
>>#### Troops.ai
>### 医药
>>>* Suki $20M
>### 音乐
>>>* Amper Music $4M
>>>* StepBeats 150万人民币
## 决策
>### 强化学习
>>#### 游戏
>>>* DeepMind
>>>* 超参数科技 3000万美元
>>>* 启元世界 数千万人民币
>>>* rct studio $10M
>>#### 调度
>>>* %secondmind.ai $24M
>>#### 测试
>>>* Mabl $20M
>>>* Test.ai $11M
>>>* Testim $10M
>>#### RPA
>>>* FortressIQ $30M
>>#### 其他
>>>* 南栖仙策
>### 运筹优化
>>>* 杉树科技 近亿元人民币
>>>* 悠桦林 近亿人民币
>>>* 宾通智能 6000万人民币
>>>* 智因科技 
>>>* nextMV $8M
## 场景AI
>### RPA
>>>* Uiptah $750M
>>>* Automation Anywhere $290M
>>>* 来也科技 4200万美元
>>>* 弘玑Cyclone 近4000万美元
>>>* 云扩科技 3000万美元
>>>* 影刀RPA
>### 工业检测
>>>* 深度视觉
>### 智能运维
>>>* 擎创科技 千万级美元
>>>* 必示科技 1.5亿人民币
>>>* 云兴维智 数千万人民币
## 行业AI
>### 零售
>>>* ImageDT图匠数据：千万级美元
>### 教育
>>>* 松鼠AI：10亿人民币
>### 农业
>>>* 极飞科技：12亿人民币
>>>* Hypersonix $11.5M
>>>* 爱科农：
>### 法律
>>>* Ross Intelligence
>>>* Atrium LTS
>>>* DoNotPays
>>>* 幂律智能
>>>* 秘塔
>### 金融
>>#### 智能投顾/投研
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
>>#### 风控
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
>>>* Tara AI $10M
>### 医疗
>>>* 连心医疗：9000万人名币
>>>* 麦歌算法
>### 制药
>>>* 晶泰科技：3.188亿美元 全球最高的AI药研公司
>>>* 费米子科技：上亿元
>>>* 望石智慧
>>>* Recursion Pharmaceuticals
>### 服装
>>>* 智布：1亿美元
>>>* 极睿科技：亿元级人民币
>>>* 时谛智能：近亿人民币
>### 房地产
>>>* Skyline AI
>### 物流
>>>* 快运兔
>### 工业
>>>* Augury $55M

wentingcan@wentingcandeMacBook-Pro testCode % python processAIdoc.py
# Survey of Startups on Artificial Intelligence Software
# 人工智能软件创业公司调研
Contributed by Warren Wen

该repo从技术的角度来AI软件创业公司进行分类

#表示以色列公司

举例：Scale.ai :$155M

表示 scale.ai公司最新一轮融资155 million dollor
# AI infrastructure
>## 软硬件优化
>>>* OctoML $15M
>>>* Neural magic $15M
>>>* Weka.IO $31.7M
>## 异构加速器虚拟化
>>>* 趋动科技 数亿元人民币
>>>* #RunAI $30M
>>>* #bitfusion 被三星收购
>## 数据处理与发现
>>>* Trifacta $100M
>>>* #Explorium.ai$31M
>## 数据合成
>>>* Ai.reverie: $5.6M
>>>* #DataGen Technologies $3.5M
>## 数据标注
>>>* Scale.ai :$155M 
>>>* Labelbox: $40M
>>>* #Dataloop AI $11M
>>>* Snorkel AI: $12M
>## 向量搜索与数据库
>>>* ZilliZ milvus 4300万美元
>>>* Jina AI 600万美元
>>>* Pinecone $10M
>## 深度学习框架
>>>* 一流科技：OneFlow 5000万人民币
>>>* Skymind:DL4J
>## Experiment Tracking:
>>>* Weights&Biases：4500万美元
>## 机器学习平台
>>>* DataRobot: $270M 
>>>* Dataiku：$100M
>>>* H2O.ai：$72.5M
>>>* domino data：$43M
>>>* abacus.ai $22M 
>>>* RapidMiner：$16M
>>>* Machinify：$10M
>>>* 第四范式：7亿美元
>## AutoML
>>>* 星环科技 5亿人民币
>>>* 行动贝果 3443万人民币
>>>* 探智立方 DarwinML 数百万美元
>>>* 江苏鸿程
>>>* #Allegro.AI: $11M
>## MLops
>>>* Saagie €25M
>>>* Algorithmia: $25M
>>>* #iguazio $24M
>>>* Determined AI：$11M
>>>* Spell $15M
>>>* Verta $10M
>>>* Pecan $11M
>>>* Allegro.ai  $11M
>>>* #SuperWise $4.5M
>>>* #Comet.ml $4.5
>>>* Seldon £7.1
>>>* Evidently ai
>>>* #ParallelM 被DataRobot收购
>>>* H2O.ai
>## Feature Store:
>>>* Tecton：$35M
>## model monitoring
>>>* Arthur AI $15M
>>>* databand.ai $14.5M
>>>* WhyLabs $4M
>## Feature Discovery
>>>* #explorium $31M
>## 边缘MLops
>>>* 开放智能Open AI LAB
>>>* #Deci AI $9.1M
>## 数据版本和共享社区
>>>* Pachyderm $16M
>>>* Graviti 千万级美元
>>>* #DAGsHub $3M
>>>* 和鲸科技 数百万美元
>## 可解释性
>>>* Fiddler labs $10.2M
>>>* InterpretML
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #Aporia
>## 安全与隐私
>>>* Robust Intelligence $11M
>>>* 瑞莱智慧RealAI 数千万人民币
>>>* #D-ID $13.5M
>## other
>>>* Rasa $26M
>>>* Grid AI $18.6M
>>>* Hugging Face $15M
>>>* cnvrg.io 被intel收购
# 文本NLP
>## 机器翻译
>>>* Unbabel：$60M
>>>* Lilt：$25M
>>>* 推文科技：1000万人民币
>>>* Atman：560万美元
>## 文本重写
>>>* Grammarly $90M
>## Chatbot
>>### Automated CX
>>>* Ada Support $44M
>>### 智能客服
>>>* 追一科技：4100万美元
>>>* 智齿科技：2.1亿人民币
>>>* 晓多科技：超2亿人民币
>>>* 乐言科技：1.5亿人民币
>>### 心理健康
>>>* Woebot Labs：$22.8M 
>>### 运维
>>>* Moveworks：$75M
>## 背景调查
>>>* Checkr $160M
>>>* Middesk $4M
>>>* i背调：数千万人民币
>## 招聘
>>>* Eightfold $125M
>>>* Turing.com $32M
>>>* e成科技 8000万美元
>>>* Bello倍罗 数千万人民币
>>>* 近屿智能 数千万人民币
>>>* 方便面面试
>## 合同审查
>>>* Kira systems CA$65M
>## 销售
>>>* #Gong.io $200M
>>>* #chorus.ai $45M
>>>* People.ai $60M
>>>* Tact.AI  $27M
>>>* Troops.ai $12M
>>>* Recurrent.ai
>>>* 客知音 千万级人民币
>>### 水下
>>>* 深维智信
>## 其他
>>>* 达观数据 2.7亿人民币
>>>* # A21 labs
>>>* Golden $14.5M
>>>* ClearGraph 被收购
>>>* UpCodes $3.4M
# 视觉Vision
>>### 研究
>## 综合
>>>* 商汤 10亿美元
>>>* 旷世 7.5亿美元
>>>* 依图 2亿美元
>>>* 云从 18亿人民币
>>>* 图普科技 千万美元
>## 动作捕捉
>>### 诺亦腾
>>### Xmov
>>>* 

>## 创作工具
>>>* Canva $60M, $8.7B
>>>* Figma $50M, $2B 
>>>* InVisionApp $115M, $1.9B
>>>* Runway $8.5M
>>>* Beautiful.AI $11M
>>>* GliaCloud
>>>* 来画视频 5000万人民币
>>### 漫画
>## 图像压缩
>>>* 图鸭科技 数千万人民币
>## 渲染
>>>* 个人总结：
>>>* 51world
>>>* 粒界科技
>>>* 叠境
>>>* RestAR
>>>* 酷家乐
>>>* 迈吉客科技
>>>* 商询科技 datamesh
>>>* 时谛智能
>## 形象生成
>>>* Brud $20M $125M
>>>* FaceRig $2M
>>>* EmbodyMe
>>>* Xmov魔珐科技 数亿人民币
>>>* 相芯科技 1.2亿人民币
>>>* 迈吉客科技 数千万人民币
>>>* 诗云科技 数百万美金
>>>* ZMO.ai
>>>* 像素偏移
>>>* 慧夜科技
>>>* 我是大咖
>>>* 
>>>* #D-ID $13.5M
>## 视频录制
>>### 
>>### Loom
>## 视频
>>### Viedeo++
>>### 影普科技
>>### Kapwing
>>### 视频异常分析
>>>* 闪马智能
>## OCR
>>>* HyperScience $80M
>## 视频广告
>>>* #KERV Interactive $11M
>## 无人零售
>>### Grabango
>>### Standard Cognition
>>### Mad Street Den
>## 时尚
>>>* 深尚科技
>## 安防
>>>* #AnyVision  $43M
>>### tractable.ai
>## 视频异常
>>>* 闪马智能：近亿元人民币
>## 测试
>>>* #Applitools $31M
>## 医学影像
>>>* 连心医疗：9000万人民币
>## 其他
>>>* Akasha Imaging
>>>* 墨奇科技
# 音频Audio
>## 语音
>>>* 思必驰：数亿人民币
>>>* 云知声：6亿人民币
>>>* Otter.ai $50M
>>>* Descript $30M
>>>* DeepGram $25M
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
# 决策
>## 强化学习
>>### 游戏
>>>* DeepMind
>>>* 超参数科技 3000万美元
>>>* 启元世界 数千万人民币
>>>* rct studio $10M
>>### 调度
>>>* %secondmind.ai $24M
>>### 测试
>>>* Mabl $20M
>>>* Test.ai $11M
>>>* Testim $10M
>>### RPA
>>>* FortressIQ $30M
>>### 其他
>>>* 南栖仙策
>## 运筹优化
>>>* 杉树科技 近亿元人民币
>>>* 悠桦林 近亿人民币
>>>* 宾通智能 6000万人民币
>>>* 智因科技 
>>>* nextMV $8M
# 场景AI
>## RPA
>>>* Uiptah $750M
>>>* Automation Anywhere $290M
>>>* 来也科技 4200万美元
>>>* 弘玑Cyclone 近4000万美元
>>>* 云扩科技 3000万美元
>>>* 影刀RPA
>## 工业检测
>>>* 深度视觉
>## 智能运维
>>>* 擎创科技 千万级美元
>>>* 必示科技 1.5亿人民币
>>>* 云兴维智 数千万人民币
# 行业AI
>## 零售
>>>* ImageDT图匠数据：千万级美元
>## 教育
>>>* 松鼠AI：10亿人民币
>## 农业
>>>* 极飞科技：12亿人民币
>>>* Hypersonix $11.5M
>>>* 爱科农：
>## 法律
>>>* Ross Intelligence
>>>* Atrium LTS
>>>* DoNotPays
>>>* 幂律智能
>>>* 秘塔
>## 金融
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
>>>* Tara AI $10M
>## 医疗
>>>* 连心医疗：9000万人名币
>>>* 麦歌算法
>## 制药
>>>* 晶泰科技：3.188亿美元 全球最高的AI药研公司
>>>* 费米子科技：上亿元
>>>* 望石智慧
>>>* Recursion Pharmaceuticals
>## 服装
>>>* 智布：1亿美元
>>>* 极睿科技：亿元级人民币
>>>* 时谛智能：近亿人民币
>## 房地产
>>>* Skyline AI
>## 物流
>>>* 快运兔
>## 工业
>>>* Augury $55M

wentingcan@wentingcandeMacBook-Pro testCode % 
