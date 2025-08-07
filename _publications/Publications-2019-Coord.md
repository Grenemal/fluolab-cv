---
title: "Organic fluorescent probes for stochastic optical reconstruction microscopy (STORM): Recent highlights and future possibilities"
collection: publications
category: manuscripts
permalink: /publications/Publications-2019-Coord
excerpt: "<p style='text-align:justify'>Super-resolution fluorescence imaging by single-molecule localization microscopy (SMLM) offers the possibility of microscopic images with sub-diffraction spatial resolution. Stochastic optical reconstruction microscopy (STORM) is one of the emerging SMLM techniques that has contributed new insights into both the structures and functions of sub-cellular organelles in the cellular context with a spatial resolution virtually at the molecular level. Photo-switching of single fluorophores and position determination are the most common features of this SMLM technique, which allows molecule-resolved information as well as super-resolved images. However, achieving successful STORM-based images relies on the suitable choice of a fluorophore. In particular, the use of ideal organic fluorescent probes has great potential to circumvent common difficulties that arise during the construction of STORM images. However, there is hardly any comprehensive review that critically assesses the criteria for choosing ideal fluorescent probes for STORM and designing new efficient organic fluorescent probes to date. Therefore, this review has particularly focused on the choice of organic fluorescent probes, the essential features for designing new probes and the future prospects for resolving persistent issues in STORM imaging. The utility of organic fluorescent probes in multicolor STORM, 3D STORM and live cell STORM imaging are also discussed to provide a perspective concerning the true application potential of commonly used fluorescent dyes. In this review, we not only describe how organic fluorescent dyes have contributed to the growth of STORM-based super-resolution imaging in eukaryotic biology, but we also attempt to provide a basis on which advanced organic fluorescent probes can be designed and developed in the near future.</p><img src='/images/GA/Publications-2019-Coord.jpg' style='width: 400px; border-radius: 20px; display: block; margin: 0 auto;'>"
date: 2018-11-11
venue: 'Coordination Chemistry Reviews'
slidesurl: https://doi.org/10.1016/j.ccr.2018.08.006
paperurl: /files/pdf/Publications-2019-Coord.pdf
bibtexurl: /files/bib/Publications-2019-Coord.bib
citation: 'Samanta, S<em><strong><sup>#</sup></strong></em>.; <em><strong>Gong, W. <sup>#</sup></strong></em>; Li, W.; Sharma, A.; Shim, I.; Zhang, W.; Das, P.; Pan, W.; Liu, L.; Yang, Z.; Qu, J.; Kim, J. S. Organic Fluorescent Probes for Stochastic Optical Reconstruction Microscopy (STORM): Recent Highlights and Future Possibilities. <em>Coordination Chemistry Reviews</em> <strong>2019</strong>, <em>380</em>, 17&ndash;34. https://doi.org/10.1016/j.ccr.2018.08.006.'
---


<img src='/images/GA/Publications-2019-Coord.jpg' style='border-radius: 20px; display: block; margin: 0 auto;'>


光学显微镜技术，特别是荧光显微镜，因其非侵入性和活细胞成像能力，在过去一个世纪的生物医学研究中发挥了不可或估量的作用 [cite: 16]。然而，传统光学显微镜的分辨率受到阿贝衍射极限的制约，对于可见光，其横向分辨率通常在180纳米左右，轴向分辨率约为500纳米 [cite: 17]。这一限制使得观察亚细胞器等精细结构的细节变得非常困难。为了突破衍射极限，科学家们在近几十年中发展了多种超高分辨率显微成像技术（Super-resolution microscopy, SRM） [cite: 18]。这些技术大致可分为两大类：单分子定位显微技术（Single-Molecule Localization Microscopy, SMLM）和可逆饱和光学荧光跃迁（Reversible Saturable Optical Fluorescence Transitions, RESOLFT）显微技术 [cite: 26]。随机光学重建显微镜（Stochastic Optical Reconstruction Microscopy, STORM）作为SMLM家族中的一员，近年来受到了广泛关注，它使得研究人员能够在近乎分子水平的空间分辨率下，深入洞察细胞内亚细胞器的结构和功能 [cite: 5, 28]。

## STORM技术的基本原理

STORM技术的核心思想是通过时间换空间的方式绕过衍射极限 [cite: 39, 40]。在传统的荧光显微镜中，如果两个荧光分子的距离小于衍射极限，它们发出的光斑会发生重叠，无法区分。STORM技术通过控制荧光探针的光物理行为，使得在任何一个时间点，只有稀疏分布的、远小于衍射极限密度的荧光分子被激活并发射荧光 [cite: 49]。这样，每个探测到的光斑都对应于一个单独的荧光分子。通过高精度定位算法（如高斯拟合）确定这些单个分子的精确位置，然后使这些分子失活，再激活另一组稀疏分布的分子进行成像和定位 [cite: 40, 48]。重复这一过程数千至数万次，采集足够多的单分子定位信息后，将所有定位点叠加重建，最终得到一幅远超衍射极限的高分辨率图像 [cite: 52]。STORM图像的分辨率主要取决于单个荧光分子定位的精度和总的定位密度（即标记密度）[cite: 54, 55]。最初的STORM技术通常采用“染料对”策略，即一个“激活剂”分子随机激活邻近的“报告剂”分子发光，报告剂分子随后在成像缓冲液的作用下回到非荧光状态 [cite: 56, 57, 59]。

## 用于STORM的理想有机荧光探针的设计标准

成功的STORM成像在很大程度上依赖于所选用荧光探针的性能 [cite: 7]。尽管荧光蛋白和量子点也被用于STORM成像，但有机小分子荧光探针因其体积小、光子产率高、光物理性质可调等优点而备受青睐 [cite: 8, 64]。设计或选择理想的有机荧光探针需要满足以下关键标准：

1.  **亮度 (Brightness)**：荧光探针在“开启”状态下的亮度直接影响定位精度 [cite: 80]。亮度取决于探针的摩尔消光系数和荧光量子产率 [cite: 91]。高消光系数意味着探针能有效吸收激发光，高量子产率则意味着吸收的光能更有效地转化为荧光光子 [cite: 92, 93, 94]。因此，高亮度的探针能产生更多的可探测光子，从而提高定位的准确性 [cite: 90]。

2.  **占空比 (Duty Cycle) 和对比度 (Contrast Ratio)**：占空比定义为荧光分子处于荧光“开启”状态的时间与总时间的比值（或与处于“关闭”状态时间的比值） [cite: 105]。在STORM成像中，为了确保在同一衍射受限区域内同时发光的分子数量最少，需要探针具有非常低的占空比，即大部分时间处于“关闭”状态，仅在短时间内“开启”并发射荧光 [cite: 106, 107, 110]。对比度是指探针在“开启”状态和“关闭”状态下的光子输出比率 [cite: 81, 102]。理想情况下，“关闭”状态应完全不发光，以获得高对比度，从而降低背景噪声，提高定位精度 [cite: 98, 102]。

3.  **光稳定性 (Photostability)**：光稳定性决定了探针在持续激光照射下能够维持光开关循环的总次数（即开关循环数）和总的发光时间 [cite: 82, 111, 112]。理想的STORM探针应能进行数百甚至数千次的光开关循环而不发生永久性光漂白 [cite: 113, 115]。此外，“存活分数”，即在特定照射时间后仍能进行光开关的探针比例，也是衡量光稳定性的一个重要指标 [cite: 124]。

## 有机荧光探针的光开关/光闪烁机制

有机荧光探针的光开关或光闪烁是STORM成像的核心 [cite: 6]。常用的STORM有机染料主要包括花菁 (Cyanine)、罗丹明 (Rhodamine) 和噁嗪 (Oxazine) 衍生物等几大家族 [cite: 128, 129, 131]。通常倾向于选择具有红移发射/激发的染料，因为它们对活细胞的光损伤较小，且细胞自发荧光背景较低 [cite: 130]。

光开关过程涉及荧光分子在至少两个可区分的稳定状态（荧光态和暗态）之间的可逆或不可逆转换 [cite: 143, 144]。这些状态转换可以通过光照、化学环境（如氧化还原剂、硫醇的存在）等方式精确调控。例如，花菁染料（如Cy5）在硫醇存在下，可以通过光诱导的氧化还原反应在荧光态和长寿命的暗态（如自由基态或硫醇加合物）之间切换 [cite: 146, 159, 171]。其他机制还包括光致异构化（如顺反异构）、光致成环/开环反应（如罗丹明内酰胺/内酯的开关）、光解 caged 基团等 [cite: 145, 160, 182]。

成像缓冲液在调控有机染料的光开关行为中扮演着至关重要的角色 [cite: 164, 165]。缓冲液中通常包含特定的化学添加剂，如还原剂（如$\beta$-巯基乙醇 (BME)、巯基乙胺 (MEA)、二硫苏糖醇 (DTT)）、氧化剂、氧气清除系统（如葡萄糖氧化酶和过氧化氢酶，GLOX系统）和三线态淬灭剂（如环辛四烯 (COT)）等 [cite: 173, 179, 180]。这些组分协同作用，优化染料的光开关动力学，延长其寿命并提高成像质量。

## 有机染料在STORM成像中的应用进展

自2006年STORM技术首次报道以来，有机荧光探针的开发和应用极大地推动了其发展。以下将从多色成像、三维成像和活细胞成像等方面总结其应用。

1.  **多色STORM/dSTORM成像**：生物系统的复杂性要求同时观察多种分子或结构 [cite: 193]。多色STORM通过使用具有不同光谱特性的光开关探针，实现了对多个靶标的同时超高分辨率成像 [cite: 205]。Zhuang课题组率先使用Cy2-Alexa 647和Cy3-Alexa 647染料对，分别对微管和网格蛋白进行了双色STORM成像，分辨率达到20-30纳米 [cite: 206]。他们后续筛选了多种染料，如ATTO 488（蓝）、Cy3B（橙）、Alexa Fluor 647（红）和Alexa Fluor 750（近红外），为四色STORM成像奠定了基础 [cite: 211, 212]。为解决多色成像中的光谱串扰和配准误差问题，发展了光谱解混dSTORM (SD-dSTORM) 等技术 [cite: 239, 240]。Hell课题组则利用罗丹明螺内酰胺类染料，基于其独特的光谱特性，实现了低串扰的同时多色纳米显微成像 [cite: 224, 225]。dSTORM (direct STORM) 技术的出现，使得无需激活剂-报告剂对，仅使用常规花菁染料（如Cy5、Alexa 647）即可实现超分辨成像，并已成功应用于多色成像 [cite: 231, 232, 234]。

2.  **三维STORM成像**：为了获取细胞内纳米结构的完整三维形态信息，STORM技术从二维拓展到了三维 [cite: 247]。Zhuang课题组最早实现了三维STORM成像，通过引入柱面镜或更复杂的光学设计（如双物镜系统、双螺旋点扩散函数DH-PSF）来获取荧光分子的轴向位置信息，成功解析了网格蛋白包被囊泡等结构的三维形貌 [cite: 249, 250, 251, 256, 257, 258]。目前，横向分辨率可达10纳米以下，轴向分辨率可达20纳米以下 [cite: 257]。

3.  **活细胞STORM成像**：活细胞STORM成像面临巨大挑战，主要是由于成像过程通常需要数千帧图像数据，导致时间分辨率较低，难以捕捉快速的动态过程，且成像缓冲液中的某些化学物质（如高浓度硫醇）对细胞具有毒性 [cite: 263, 286, 290]。尽管如此，研究者们通过优化探针和成像条件，已在活细胞STORM成像方面取得了显著进展。Sauer课题组利用常规的Alexa Fluor和ATTO染料实现了活细胞超分辨成像，并开发了基于三甲氧苄氨嘧啶化学标签 (TMP-tag) 的ATTO655探针，用于活细胞内组蛋白H2B的dSTORM成像 [cite: 265, 269, 270]。Manley课题组使用商业化的花菁类DNA嵌入染料Picogreen，在优化缓冲液条件（如低浓度抗坏血酸和氧清除系统）后，成功实现了活细胞DNA的dSTORM成像 [cite: 274, 287, 288]。Zhuang课题组使用具有光开关特性的碳菁染料膜探针，实现了活细胞内细胞器膜结构的超分辨动态成像，时间分辨率达到1-2秒 [cite: 289]。Urano等人报道了一类基于分子内螺环化反应的自发闪烁荧光探针（如HMSiR），这类探针无需添加剂即可实现光开关，且所需激光功率较低，非常适合长时间的活细胞超分辨成像 [cite: 293, 294, 308]。Johnsson课题组开发的新型硅基罗丹明近红外探针，具有良好的细胞膜通透性、高量子产率和光稳定性，也成功用于活细胞内蛋白质的超分辨成像 [cite: 291, 292]。

4.  **其他STORM成像应用**：除了上述主要应用方向，有机染料还在其他STORM成像研究中发挥了作用。例如，利用YOYO-1、YO-PRO-1等嵌入型花菁染料对DNA进行标记和超分辨成像 [cite: 299, 300]；利用Hoechst和DAPI等DNA小沟结合染料研究染色质的精细结构 [cite: 306]；利用dSTORM技术解析核孔复合物的八重对称结构 [cite: 301, 302]；研究自修复花菁染料的分子内光稳定机制等 [cite: 303]。

## 结论与未来展望

STORM技术为在亚衍射极限分辨率下研究复杂的细胞过程提供了一个前景广阔的平台 [cite: 322]。有机小分子荧光探针的不断发展是STORM技术进步的关键驱动力之一 [cite: 323]。尽管现有有机荧光探针已在STORM成像中取得了巨大成功，但仍面临诸多挑战，例如在多色成像中，不同染料之间可能存在错误的激活脉冲响应、光谱串扰和纳米尺度下的色差校正困难等问题 [cite: 329, 330, 331]。因此，开发具有更高亮度、更优光稳定性、更理想光开关特性（如自发闪烁、低毒性条件下的高效开关）的新型有机荧光探针仍然是该领域的重要研究方向 [cite: 324, 327, 333]。未来，随着更多高性能探针的涌现和成像技术的不断完善，STORM有望在基础生物学研究、疾病诊断（如通过亚细胞器表达谱的定量信息进行诊断）和个性化治疗等领域发挥越来越重要的作用 [cite: 325, 335, 336]。本综述聚焦于有机荧光探针在STORM中的选择标准、设计思路和应用进展，希望能为相关领域的研究人员提供有益的参考，并推动新型探针的开发，进一步拓展超分辨成像的应用边界 [cite: 10, 336]。