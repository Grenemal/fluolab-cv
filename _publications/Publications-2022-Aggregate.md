---
title: "ASBase: The universal database for aggregate science"
collection: publications
category: manuscripts
permalink: /publications/Publications-2022-Aggregate
excerpt: "<p style='text-align:justify'> This paper reports the first universal and versatile database on aggregate materials for the field of aggregate science research. At the current stage, the database contains over 1000 entries of organic aggregate material systems (mainly luminescent systems at the current stage) with a unique data structure which is designed particularly for aggregate materials and containing the photophysics and physicochemical properties of the compounds in different statuses of aggregation, including dilute solution form, pristine solid-state, stable crystalline, and nanoaggregates formed in solvents. The web-based interface of the database provided functions to index, search, manipulate, fetch and deposit data entries. In addition, a background calculation service optimizes the chemical structure of new entries on different levels of accuracies. The database also provided background API for interactive developments of prediction or regression models based on machine-learning algorithms.</p><img src='/images/GA/Publications-2022-Aggregate.jpg' style='width: 400px; border-radius: 20px; display: block; margin: 0 auto;'>"
date: 2022-09-01
venue: 'Aggregate'
slidesurl: https://doi.org/10.1002/agt2.263
paperurl: /files/pdf/Publications-2022-Aggregate.pdf
bibtexurl: /files/bib/Publications-2022-Aggregate.bib
citation: 'Gong, J.; <em><strong>Gong, W.</strong></em>; Wu, B.; Wang, H.; He, W.; Dai, Z.; Li, Y.; Liu, Y.; Wang, Z.; Tuo, X.; Lam, J. W. Y.; Qiu, Z.; Zhao, Z.; Tang, B. Z. ASBase: The Universal Database for Aggregate Science. <em>Aggregate</em>, <strong>2023</strong>, <em>4</em> (1), e263. https://doi.org/10.1002/agt2.263.'
---

<img src='/images/GA/Publications-2022-Aggregate.jpg' style='border-radius: 20px; display: block; margin: 0 auto;'>

## 一、研究背景与意义

近年来，聚集体科学作为化学与材料科学领域的一个新兴分支，逐渐引起了科研人员的广泛关注。^[1]^聚集体科学不仅关注分子的化学结构，还强调分子间的组织形式及其对宏观性质的影响。^[2]^其中，聚集诱导发光（Aggregation-Induced Emission, AIE）作为聚集体科学的一个重要子领域，因其独特的光学性能和潜在的应用价值，成为研究热点。^[3]^

然而，与实验室研究的快速发展相比，聚集体科学的研究方法仍停留在经典实验化学阶段，高度依赖经验法则和试错法。^[4]^此外，尽管计算机科学和数据科学取得了显著进展，但聚集体科学领域的数据积累和泛化能力仍然不足，限制了数据驱动的研究范式的发展。^[5]^现有的数据库如剑桥结构数据库（CSD）、SciFinder、Reaxys和Materials Project等，虽然为化学和材料研究提供了数据检索、比较、过滤和追溯功能，但在聚集体科学领域仍存在不适应的问题。^[6]^

因此，开发一个专门针对聚集体科学的通用数据库显得尤为重要。^[7]^本文研究的ASBase数据库正是为了满足这一需求而设计的，旨在为聚集体科学领域的研究人员提供一个全面、灵活且易于使用的数据平台。^[8]^

## 二、ASBase数据库的设计与功能

**1. 数据库结构**

ASBase数据库采用独特的架构设计，以适应聚集体科学研究的特殊需求。^[9]^整个系统分为服务器端和客户端两部分。服务器端基于Django 4.0框架构建，包含数据服务器模块和计算服务器模块。^[10]^数据服务器模块进一步细分为三个子表，分别存储化学结构信息、参考文献信息和光物理性质信息。每个条目包含约40个字段的数据，涵盖化学结构、文献参考、专利、光物理性质（如吸收、发射、量子产率和寿命）、理化性质（如稳定性和溶解度）以及应用信息等。^[11]^

**2. 数据上传与验证**

注册用户可以通过网页的数据提交界面上传条目，上传的条目将存储在临时数据库中进行验证。验证过程包括定期审查临时数据库中的条目，确定其可靠性，并将可靠的条目录入核心数据库，不可靠的条目则返回给上传者进行复查。^[12]^一旦可靠数据被记录在核心数据库中，将生成包括分配系数对数（log P）、拓扑极性表面积（TPSA）、结构标识符（如InChI和InChIKey）、化学式和分子量等信息。^[13]^

**3. 数据检索与搜索**

客户端提供了一个全面的网页界面，供用户交互式利用数据库。^[14]^最重要的功能是数据检索系统，提供三种不同的检索方式：基本搜索允许用户根据作者姓名、不同聚集状态下的光物理性质、报告特征和应用等简单条件进行搜索；高级搜索功能支持用户同时使用多个过滤器进行检索；化学结构搜索提供了化学结构编辑器和SMILES输入框，用于根据输入的化学子结构搜索化合物。^[15]^

**4. 统计报告生成**

ASBase数据库的另一个关键特性是统计报告生成功能。服务器端可以根据核心数据库中的数据条目生成实时统计报告，并在网页上渲染图表。^[16]^当前版本的统计报告包含六个图表，包括溶液中吸收峰波长、固态发射峰波长和固态荧光量子产率的三个直方图，报告特征和报告光致发光机制的两个饼图，以及一个以吸收峰波长为x轴、固态发射峰波长为y轴的相关散点图。^[17]^

**5. 算法与计算方法**

ASBase数据库使用了多种算法和计算方法来处理和分析数据，包括皮尔逊相关系数、斯皮尔曼相关系数和t-分布式随机邻居嵌入（t-SNE）等。^[18]^这些算法帮助揭示数据之间的潜在关系，如光物理性质之间的相关性、化学结构与性质之间的关系等。

## 三、ASBase数据库的应用与优势

**1. 学术研究与工业应用**

ASBase数据库不仅为学术研究人员提供了强大的数据支持，还为工业界的工程师、投资者和政策制定者提供了有价值的参考。研究人员可以利用数据库中的数据进行理论探索、新材料预测和光物理性质预测等。工程师则可以基于数据库中的信息开发具有特定需求的产品。投资者和政策制定者则可以通过数据库了解聚集体科学领域的发展趋势和潜在应用价值。

**2. 数据驱动的研究范式**

ASBase数据库的建立促进了聚集体科学领域的数据驱动研究范式的发展。^[19]^通过积累大量的实验数据，并利用机器学习算法对这些数据进行分析和挖掘，研究人员可以发现新的规律、预测未知化合物的性质，并指导实验设计。这种数据驱动的研究方法不仅提高了研究效率，还降低了研究成本。^[20]^

**3. 数据库的灵活性与可扩展性**

ASBase数据库具有高度的灵活性和可扩展性。研究人员可以根据需要自定义检索条件，获取特定领域或特定性质的数据。^[21]^同时，数据库还提供了数据提交功能，鼓励全球范围内的研究人员共享他们的研究成果。随着研究的不断深入和新数据的不断积累，ASBase数据库将不断扩大其数据规模和应用范围。^[22]^

## 四、ASBase数据库的当前数据与初步分析

**1. 当前数据规模**

截至目前，ASBase数据库已包含超过1100个条目，每个条目对应一个在聚集体科学领域报道的化合物。^[23]^这些化合物涵盖了AIE、聚集诱导猝灭（ACQ）、室温磷光（RTP）、热激活延迟荧光（TADF）和聚集诱导延迟荧光（AIDF）等多种机制。^[24]^此外，数据库还根据化合物的光致发光机制将其分类为分子内电荷转移（ICT）、扭曲分子内电荷转移（TICT）、激发态分子内质子转移（ESIPT）、中性芳香（NA）和簇发光（CL）等系统。^[25]^

**2. 初步数据分析**

通过对数据库中前988个条目的初步分析，研究人员发现了一些有趣的现象和规律。^[26]^例如，发射峰波长的分布表明平均斯托克斯位移约为120纳米；晶体中的发射峰波长均值最低，这可能是由于晶体中的刚性化效应抑制了激发态的弛豫过程。^[27]^此外，量子产率在聚集体、晶体和原始固态粉末中表现出两个显著的密度峰，而在稀溶液中只有一个明显的密度峰。^[28]^这些发现为进一步理解聚集体科学中的光物理现象提供了有力支持。

## 五、结论与展望

ASBase数据库作为聚集体科学领域的首个通用数据库，为研究人员提供了一个全面、灵活且易于使用的数据平台。^[29]^通过独特的数据结构设计、强大的数据检索与搜索功能、灵活的统计报告生成功能以及丰富的算法与计算方法，ASBase数据库不仅满足了聚集体科学研究的需求，还促进了数据驱动的研究范式的发展。^[30]^

未来，ASBase数据库将继续运营和扩展，不断吸收新的数据和功能。^[31]^研究人员可以期待更多的数据条目、更丰富的数据类型以及更强大的数据分析工具。^[32]^同时，ASBase数据库也将成为聚集体科学领域的重要交流平台，促进全球范围内的研究人员共享他们的研究成果和经验。我们相信，在ASBase数据库的支持下，聚集体科学领域将迎来更加繁荣的发展。^[33]^