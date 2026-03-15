# BaTiO₃/沥青碳包覆石墨负极提升快充性能的作用机制研究

## 第一章 绪论

### 1.1 研究背景与意义

自20世纪90年代商业化以来，锂离子电池（Lithium-Ion Batteries, LIBs）凭借其高能量密度、长循环寿命和低自放电率等显著优势，已成为便携式电子设备、电动汽车（Electric Vehicles, EV）及规模储能系统的核心电源技术 [1, 2]。进入21世纪第二个十年，全球新能源汽车产业的爆发式增长对动力电池提出了更严苛的要求，其中快速充电性能已成为制约电动汽车大规模普及的核心技术瓶颈之一 [3]。消费者对"补能时间"的心理焦虑——即所谓"里程焦虑"的演变形式——要求动力电池能够在10至15分钟内完成80%以上电量的补充，对应等效充电倍率通常达到4C乃至6C以上 [4]。

然而，在如此高倍率充电条件下，传统石墨负极材料面临严峻挑战。石墨作为目前商业锂离子电池中最主流的负极材料，其理论比容量为372 mAh g⁻¹，具有成本低廉、资源丰富、与锂的嵌入/脱出电位适中（vs. Li⁺/Li ≈ 0.1 V）等突出优点 [5, 6]。然而石墨层状结构固有的各向异性导致锂离子仅能从边缘平面（edge plane）嵌入，而非从基面（basal plane）透过，这从根本上限制了锂离子的传输通量 [7]。在高倍率充电条件下，石墨颗粒表面局部电位迅速降至0 V (vs. Li⁺/Li) 以下，引发金属锂在负极表面的不可控沉积（锂枝晶，Lithium Plating），不仅造成不可逆容量损失，更带来严重的安全隐患，包括短路和热失控风险 [8, 9]。

因此，发展有效改善石墨负极快充动力学性能的策略，既具有重要的基础科学意义，又具有迫切的工程应用价值。本课题围绕BaTiO₃/沥青碳（Pitch Carbon, PC）复合包覆体系对石墨负极快充性能的提升机制展开系统研究，旨在从材料设计与界面工程的角度揭示多功能包覆层的协同作用规律，为高性能快充负极材料的开发提供理论依据与技术支撑。

---

### 1.2 石墨负极材料的快充限制机制

#### 1.2.1 锂离子在石墨中的嵌入动力学

石墨的嵌锂过程（Staging机制）是一个有序的相变过程，Dahn等人早在1991年便通过X射线衍射（XRD）系统阐明了LixC₆体系的相图 [6]。在完全嵌锂状态下，锂离子以LiC₆形式存在于每一层石墨烯层之间，形成Stage 1结构。锂离子在石墨中的扩散系数（DLi⁺）量级约为10⁻¹⁰～10⁻⁸ cm² s⁻¹，相对于液态电解质中的锂离子扩散系数（~10⁻⁶ cm² s⁻¹）低2～3个数量级 [5]。这意味着在高倍率充电条件下，固相扩散过程将成为速率控制步骤，导致严重的浓度极化。

如图1-1所示，锂离子从电解质嵌入石墨颗粒内部的完整过程涉及多个串联动力学步骤：①锂离子在电解液中的传质（液相扩散）；②锂离子在固体电解质界面膜（Solid Electrolyte Interphase, SEI）中的迁移；③锂离子在SEI/石墨界面的去溶剂化（Desolvation）；④锂离子在石墨层间的固相扩散；⑤电子在石墨颗粒内部及集流体间的传导 [10, 11]。在低倍率充电条件下，上述各步骤均处于准平衡态，SEI传输和去溶剂化为主要速率限制步骤；而在高倍率充电（>2C）条件下，固相扩散及SEI界面传输的动力学限制急剧放大，二者共同主导着负极的极化行为 [12]。

> **图1-1** 锂离子嵌入石墨负极的多步动力学过程示意图（改绘自 Nano-Micro Letters, 2023, 15, 215 [12]）

*[图注：从左至右依次展示电解液传质、SEI膜传输、界面去溶剂化、石墨层间固相扩散四个串联限速步骤。高倍率下（>4C），颗粒表面局部SOC（荷电状态）分布不均匀，导致边缘区域首先达到嵌锂饱和，进而引发锂金属析出。]*

#### 1.2.2 锂枝晶析出与安全性问题

当充电倍率超过临界阈值时，石墨负极表面的局部过电位使电极电位低于0 V (vs. Li⁺/Li)，热力学上有利于金属锂的还原沉积。Tomaszewska等人在2019年综述中系统指出，锂枝晶的形成过程受到电流密度分布、SEI均匀性及温度等多因素耦合影响，且枝晶一旦形成便具有高度不可逆性 [3]。枝晶向隔膜方向生长可直接导致正负极短路，引发热失控乃至电池起火，是快充电池安全性的最大威胁 [13]。

此外，非均匀锂嵌入还会导致石墨颗粒各处膨胀不一致，引发颗粒破裂和电极结构损坏，进一步加速容量衰减 [14]。Tu等人于2023年在Nature Energy上的工作表明，调控SEI的结晶结构（引入Li₃P晶态相）能够有效提升SEI的离子电导率，从而在不牺牲安全性的前提下实现6C快充能力，这一突破从侧面印证了SEI工程对快充性能的关键作用 [9]。

#### 1.2.3 电极宏观传输的限制

除颗粒级别的动力学限制外，电极层面的离子传输均匀性同样至关重要。在高倍率充电条件下，由于液相Li⁺浓度梯度的建立速率远快于其弛豫速率，电极厚度方向上形成显著的Li⁺浓度分布不均匀性，靠近隔膜侧的石墨颗粒优先嵌锂并最终过嵌，而靠近集流体侧的颗粒则相对利用率不足 [15]。Wang等人在2022年Science Advances报道的双梯度结构石墨负极（粒径-孔隙率协同梯度设计）有效缓解了上述电极级宏观传输限制，实现了10分钟内60%容量的快充目标，表明电极结构设计与颗粒级改性同等重要 [16]。

---

### 1.3 石墨负极快充改性策略综述

#### 1.3.1 石墨结构优化与粒径调控

减小石墨颗粒粒径是缩短固相扩散路径最直接有效的方法。当颗粒等效球径从20 μm减小至5 μm以下时，固相扩散时间常数（τ = r²/π²D）降低约一个数量级，可显著改善高倍率下的利用率 [12]。然而，粒径减小伴随着比表面积的急剧增大，与电解质接触的活性面积增加会导致更多SEI消耗锂源，首次库仑效率（ICE）下降，同时小颗粒石墨堆积密度低，不利于体积能量密度的保持 [17]。此外，天然石墨的片状形貌易导致颗粒沿基面方向优先取向，加剧电极各向异性，因此球形化处理是目前工业上改善石墨各向同性的常规手段 [3]。

#### 1.3.2 沥青碳包覆改性

沥青碳（Pitch Carbon）包覆是当前工业界应用最为广泛的石墨负极表面改性技术之一。沥青（Pitch）是煤焦油或石油深加工的副产物，含碳量高（>90 wt%）、价格低廉，经高温碳化（通常700～1100 °C）后在石墨颗粒表面形成均匀的无定形碳（Amorphous Carbon）包覆层 [18, 19]。

如图1-2所示，沥青碳包覆对石墨负极电化学性能的改善主要体现在以下几个维度 [19, 20]：

**(1) 提供额外的锂离子传输通道：** 无定形碳结构高度无序，其层间距（d₀₀₂ ≈ 0.38～0.42 nm）显著大于石墨（d₀₀₂ ≈ 0.335 nm），且拥有丰富的微孔和缺陷位点，可为锂离子提供多维度的嵌入/脱出路径，而非石墨单一的边缘平面通道，从而有效提升高倍率下的动力学响应 [20]。

**(2) 调控SEI的形成与组成：** 沥青碳包覆改变了石墨与电解质直接接触的化学环境。均匀的碳包覆层替代裸露的石墨边缘平面成为SEI的形成基底，有利于生成更均匀、致密、导离子性更优的SEI层。Oka等人（2022）通过对比实验证明，碳包覆石墨上形成的SEI中LiF等无机成分比例更高、厚度更均匀，迁移数和离子电导率均得到改善 [21]。

**(3) 抑制电解质共嵌入与石墨剥层：** 裸露石墨边缘平面易发生碳酸乙烯酯（EC）等溶剂分子的共嵌入，引发石墨层间距剧烈膨胀导致剥层（Exfoliation），降低循环稳定性。沥青碳包覆层作为物理屏障，有效隔绝了电解质溶剂与石墨层间的直接接触，显著抑制了共嵌入现象 [22]。

> **图1-2** 沥青碳包覆石墨的结构示意图与电化学性能对比（改绘自 Materials, 2022, 15, 4713 [20] 及 J. Power Sources, 2022, 541, 231698 [21]）

*[图注：（a）裸露石墨颗粒的截面示意，锂离子仅通过边缘平面嵌入，同时溶剂分子可共嵌入；（b）沥青碳包覆石墨截面示意，无定形碳层提供多维传输通道，形成均匀SEI；（c）倍率性能对比曲线，显示碳包覆样品在2C、4C条件下的容量保持率明显优于裸石墨。]*

Kim等人（2024）在J. Energy Storage的研究进一步揭示了沥青结晶度对碳包覆层性能的决定性影响：各向同性沥青碳化后形成无序度更高的碳层，在倍率性能改善方面更具优势；而各向异性中间相沥青碳化后形成具有一定石墨化度的碳层，对首次库仑效率的提升更为显著 [22]。这为针对特定应用场景优化沥青碳包覆工艺提供了理论指导。

#### 1.3.3 异质元素掺杂与表面功能化

除碳包覆外，异质元素（N、B、S、P等）的掺杂改性也是改善石墨负极快充性能的重要策略。氮掺杂可在石墨层间引入吡啶氮、吡咯氮等活性位点，增强对锂离子的吸附能力，同时提升材料本征电导率，有利于快充条件下的电荷转移 [23]。磷元素引入可在颗粒表面原位形成富磷SEI，Wang等人（2023）在ACS Energy Letters中报道了纳米磷层修饰石墨负极后，EIS分析表明Li⁺在SEI中的迁移活化能从28.3 kJ/mol降至17.6 kJ/mol，显著提升了低温和高倍率下的充电能力 [24]。

#### 1.3.4 电解质与界面调控

电解质组成对SEI性质的调控是另一重要维度。高浓度电解质（HCE）和局域高浓度电解质（LHCE）通过提高溶剂化结构中无机盐的比例，使SEI中形成更多LiF等低界面阻抗无机组分，从而提升Li⁺穿越SEI的迁移速率 [13]。此外，添加剂（如FEC、VC）的引入可精确调控SEI的有机/无机组成比例。光化学处理（γ射线照射）、原位电化学处理等新技术也被用于构建富无机组分的功能性SEI，Nature Communications（2021）的工作表明，该类SEI使石墨负极在10.8分钟内实现80%容量补充 [25]。

---

### 1.4 BaTiO₃在电化学储能中的应用

#### 1.4.1 BaTiO₃的基本物理化学性质

BaTiO₃（钛酸钡）是一种典型的钙钛矿型铁电/压电陶瓷材料，室温下具有四方对称性（a = b ≠ c），Ti⁴⁺离子在氧八面体内沿c轴方向偏离中心位置，产生自发极化（Ps ≈ 26 μC cm⁻²）[26]。其居里温度（Tc）约为120 °C，在此温度以下维持铁电相。BaTiO₃的压电系数d₃₃ ≈ 191 pC N⁻¹，相对介电常数ε_r在室温下高达1000～3000（依频率和颗粒尺寸而异）[27]。这些独特的铁电与压电性质使其在传感器、执行器、储能电容器等领域有广泛应用。

值得注意的是，纳米级BaTiO₃颗粒（~10 nm）虽然因尺寸效应导致铁电相稳定性下降，但最新的物理实验表明，其仍保持显著的Ti偏心位移和自发极化 [27]，这对电池界面应用中的电场调控效果至关重要。

如图1-3所示，BaTiO₃晶体的四方相结构中，Ti⁴⁺的自发偏移导致正负电荷中心不重合，形成自发电偶极矩，在材料整体上表现为自发极化。当外加应力或温度变化时，极化强度随之改变（压电效应/热电效应），在材料表面产生感应电荷，在材料内部建立局域内建电场（Built-in Electric Field）。

> **图1-3** BaTiO₃钙钛矿结构及铁电极化机制示意图（改绘自 ACS Energy Letters, 2023, 8, 4357 [28]）

*[图注：（a）BaTiO₃的立方相（T > 120 °C，顺电相）与四方相（T < 120 °C，铁电相）晶体结构对比，展示Ti⁴⁺在氧八面体内的中心偏移；（b）铁电畴结构示意及宏观极化示意；（c）在应力（振动）或温度变化下，压电效应产生的局域内建电场对Li⁺定向迁移的驱动示意。]*

#### 1.4.2 BaTiO₃在锂离子电池中的应用进展

BaTiO₃的铁电极化特性赋予其在锂离子电池界面调控中的独特优势。2016年，Lee等人在ACS Nano率先报道了碳纳米管/Si/BaTiO₃纳米复合负极，实验证明压电BaTiO₃产生的局域电势能够有效增强锂离子的迁移动力学，该体系在1C倍率下循环100圈后容量保持率较未添加BaTiO₃的对照组提升约30% [29]。这一开创性工作确立了利用BaTiO₃的铁电性增强离子传输的基本概念。

后续研究进一步拓展了BaTiO₃在电池中的应用场景。Zhang等人（2023）在ACS Energy Letters的综述中系统梳理了铁电材料在高能量密度电池中的作用机制，归纳出铁电材料通过以下途径影响电池性能 [28]：①铁电极化产生的内建电场对Li⁺迁移的定向驱动作用；②铁电材料高介电常数对界面空间电荷层的抑制效应；③铁电/压电材料在充放电应力循环中产生的动态极化辅助离子输运。研究还报道了BaTiO₃@Ti₃C₂ MXene异质结用于锂硫电池，以及铁电材料改性隔膜用于稳定锂金属负极等多种应用场景。

在石墨负极领域，BaTiO₃的引入被期望通过两条路径发挥协同作用：其一，利用BaTiO₃的高介电常数（ε_r > 1000）增强界面区域Li⁺的浓度和迁移速率；其二，利用BaTiO₃与石墨颗粒界面处的极化电荷降低Li⁺的去溶剂化势垒，加快Li⁺穿越SEI的速率 [28, 29]。然而，目前将BaTiO₃与沥青碳复合包覆体系相结合，系统研究其对石墨负极快充性能提升机制的工作尚属罕见，相关物理化学机制尚不明确，这正是本课题研究的出发点。

---

### 1.5 研究现状分析与存在的科学问题

综合上述文献调研，当前石墨负极快充改性领域的研究现状可概括为以下几点：

**（1）单一改性策略的局限性已引起广泛关注。** 单纯沥青碳包覆在提升倍率性能的同时，往往以牺牲首次库仑效率为代价，且大量无定形碳的引入会降低材料的压实密度，影响体积能量密度 [19, 20]。单纯引入BaTiO₃虽能提升界面离子传输动力学，但BaTiO₃本身电子电导率极低（~10⁻¹² S cm⁻¹），易增加界面接触电阻，同时其在锂离子电池工作电位窗口内的化学稳定性尚需深入研究 [28]。

**（2）BaTiO₃与碳包覆的协同效应机制尚未厘清。** 理论上，沥青碳包覆可解决BaTiO₃的导电性问题，同时BaTiO₃的铁电极化可弥补沥青碳对SEI调控能力的不足；但二者在空间分布、载量比例及碳化工艺等方面对协同效应的影响规律缺乏系统研究。

**（3）BaTiO₃在石墨负极体系中的作用机制尚需实验验证。** 现有文献多基于含Si负极或分离器改性场景中研究BaTiO₃的电场调控作用，在石墨层间嵌锂这一特定电化学过程中，BaTiO₃极化电场如何与SEI形成动力学、锂离子去溶剂化过程及固相扩散耦合，需要结合原位/非原位表征手段进行深入探讨。

**（4）快充条件下的材料稳定性与安全性评估不足。** 高倍率充电带来的大电流密度、局部温升以及机械应力（体积膨胀/收缩），对BaTiO₃/沥青碳复合包覆层的结构完整性和电化学性能稳定性的影响，有待通过系统的循环测试和失效分析加以明确。

---

### 1.6 本课题的研究内容与目标

针对上述科学问题，本论文以构建BaTiO₃/沥青碳双功能复合包覆石墨负极为核心目标，系统开展以下研究工作：

**研究内容一：BaTiO₃/沥青碳复合包覆石墨的制备工艺研究。** 通过液相混合-高温碳化路线，探索BaTiO₃纳米颗粒与沥青碳在石墨颗粒表面的协同分布规律，优化BaTiO₃载量（1～10 wt%）、沥青碳化温度（700～1100 °C）及时间等关键工艺参数，建立制备工艺-微观结构关联。

**研究内容二：BaTiO₃/沥青碳包覆对石墨快充性能的提升效果评估。** 通过恒流充放电（CCCV）、电化学阻抗谱（EIS）、恒电位间歇滴定（GITT）、循环伏安（CV）等多种电化学测试方法，定量表征包覆处理前后石墨负极在不同倍率（0.1C～6C）下的容量、首次库仑效率、倍率性能及循环稳定性变化。

**研究内容三：BaTiO₃/沥青碳包覆改善快充性能的物理化学机制解析。** 结合透射电子显微镜（TEM）、X射线光电子能谱（XPS）、飞行时间二次离子质谱（TOF-SIMS）、低温电子显微镜（Cryo-EM）等先进表征手段，揭示包覆层的空间分布特征、SEI的组成演变及BaTiO₃的极化特性对界面动力学的调控规律。

**研究内容四：快充循环过程中材料稳定性与失效机制分析。** 针对4C以上快充条件下的循环衰减行为，系统分析包覆层结构破坏、SEI演变及石墨颗粒完整性变化等失效模式，为进一步优化复合包覆体系提供指导。

本课题的研究目标是：阐明BaTiO₃铁电极化与沥青碳界面调控的协同作用机制，开发出在4C充电倍率下容量保持率≥90%、500次循环后容量保持率≥80%的高性能快充石墨负极材料，为下一代快充动力电池的负极材料设计提供科学依据。

如图1-4所示，本文的研究思路可概括为"材料设计—性能评价—机制解析—失效分析"的闭环研究框架。

> **图1-4** 本论文研究框架示意图

*[图注：研究框架分为四个模块：（1）左上：BaTiO₃/沥青碳复合包覆石墨的制备与结构调控；（2）右上：多尺度电化学表征与快充性能评估；（3）左下：界面化学与SEI机制分析（XPS、TOF-SIMS、Cryo-EM）；（4）右下：快充失效机制与循环稳定性分析。四个模块通过中心的"快充机制"核心问题有机衔接，最终形成结构-性能-机制的完整知识链条。]*

---

### 参考文献

[1] Tarascon J M, Armand M. Issues and challenges facing rechargeable lithium batteries [J]. *Nature*, 2001, **414**(6861): 359–367.

[2] Goodenough J B, Kim Y. Challenges for rechargeable Li batteries [J]. *Chemistry of Materials*, 2010, **22**(3): 587–603.

[3] Tomaszewska A, Chu Z, Feng X, et al. Lithium-ion battery fast charging: A review [J]. *eTransportation*, 2019, **1**: 100011.

[4] Li Y, Qian K, He Y B, et al. Fast charging of lithium-ion batteries at all temperatures [J]. *Proceedings of the National Academy of Sciences*, 2018, **115**(26): 6590–6595.

[5] Persson K, Hinuma Y, Meng Y S, et al. Thermodynamic and kinetic properties of the Li-graphite system from first-principles calculations [J]. *Physical Review B*, 2010, **82**(12): 125416.

[6] Dahn J R. Phase diagram of LixC6 [J]. *Physical Review B*, 1991, **44**(17): 9170–9177.

[7] Buqa H, Würsig A, Goers D, et al. Behaviour of highly crystalline graphites in lithium-ion cells with propylene carbonate containing electrolytes [J]. *Journal of Power Sources*, 2003, **119–121**: 160–166.

[8] Peled E, Menkin S. Review—SEI: Past, present and future [J]. *Journal of the Electrochemical Society*, 2017, **164**(7): A1703–A1719.

[9] Tu Z, Choudhury S, Ates M N, et al. Fast-charging capability enabled by a Li₃P-based crystalline solid-electrolyte interphase [J]. *Nature Energy*, 2023, **8**(12): 1365–1374.

[10] Jow T R, Delp S A, Allen J L, et al. Factors limiting Li+ charge transfer kinetics in Li-ion batteries [J]. *Journal of the Electrochemical Society*, 2018, **165**(2): A361–A367.

[11] Xu K. Electrolytes and interphases in Li-ion batteries and beyond [J]. *Chemical Reviews*, 2014, **114**(23): 11503–11618.

[12] Yang C, Chen J, Ji X, et al. Kinetic limits of graphite anode for fast-charging lithium-ion batteries [J]. *Nano-Micro Letters*, 2023, **15**: 215.

[13] Zhao J, Liao L, Shi F, et al. Challenges and strategies of fast-charging Li-ion batteries with a focus on Li plating [J]. *Energy Material Advances*, 2023: 0113.

[14] Kasnatscheew J, Röser S, Börner M, et al. Do increased Ni contents in LiNixMnyCozO2 (NMC) electrodes decrease structural and electrochemical stabilities? [J]. *ACS Applied Energy Materials*, 2019, **2**(11): 7733–7737.

[15] Zhang S S. The effect of the charging protocol on the cycle life of a Li-ion battery [J]. *Journal of Power Sources*, 2006, **161**(2): 1385–1391.

[16] Wang C, Liu T, Yang X, et al. Fast charging of energy-dense lithium-ion batteries [J]. *Science Advances*, 2022, **8**(6): eabm6624.

[17] Wu Y P, Wan C R, Jiang C Y, et al. Carbon anode materials for lithium ion batteries [J]. *Journal of Power Sources*, 2003, **114**(2): 228–236.

[18] Zhao Y, Liu J, Zhang H, et al. Modification mechanism of graphite anode in lithium-ion battery coated with ethylene tar pitch [J]. *Journal of Applied Electrochemistry*, 2024, **54**: 1123–1135.

[19] Zhang K, Li H, Chen Q, et al. Effect and mechanism of pitch coating on the rate performance improvement of lithium-ion batteries [J]. *Materials*, 2022, **15**(13): 4713.

[20] Oka H, Kasahara N, Kameyama T, et al. Effect of amorphous carbon coating on the formation of solid electrolyte interphase and electrochemical properties of a graphite electrode [J]. *Journal of Power Sources*, 2022, **541**: 231698.

[21] Kim C, Ahn H J, Kim S W, et al. Effect of pitch crystallinity on electrochemical performance of graphite carbon coatings [J]. *Journal of Energy Storage*, 2024, **86**: 111148.

[22] Dong Y, Zhang Z, Wang Y, et al. Review on graphite anodes for fast-charging lithium-ion batteries: Mechanism, modification and characterizations [J]. *Advanced Functional Materials*, 2025, **35**: 2506190.

[23] Shi F, Ross P N, Zhao H, et al. A catalytic path for electrolyte reduction in lithium-ion cells revealed by in situ attenuated total reflection-Fourier transform infrared spectroscopy [J]. *Journal of the American Chemical Society*, 2015, **137**(9): 3181–3184.

[24] Wu B, Lochala J, Taverne T, et al. Mitigating electrode-level heterogeneity using phosphorus nanolayers on graphite for fast-charging batteries [J]. *ACS Energy Letters*, 2023, **8**(9): 3835–3843.

[25] Liu G, Chen H, Ye H, et al. Photochemically driven solid electrolyte interphase for extremely fast-charging lithium-ion batteries [J]. *Nature Communications*, 2021, **12**: 7034.

[26] Lines M E, Glass A M. *Principles and Applications of Ferroelectrics and Related Materials* [M]. Oxford: Oxford University Press, 1977.

[27] Smith M B, Page K, Siegrist T, et al. Crystal structure and the paraelectric-to-ferroelectric phase transition of nanoscale BaTiO₃ [J]. *Journal of the American Chemical Society*, 2008, **130**(22): 6955–6963.

[28] Zhang T, Ran F. Ferroelectric materials for high energy density batteries: Progress and outlook [J]. *ACS Energy Letters*, 2023, **8**(10): 4357–4370.

[29] Lee B S, Son S B, Park K M, et al. A carbon nanotube/Si/BaTiO₃ nanocomposite anode: Evidence for enhanced lithium-ion mobility induced by the local piezoelectric potential [J]. *ACS Nano*, 2016, **10**(2): 2617–2627.

[30] Wang A, Kadam S, Li H, et al. Review on modeling of the anode solid electrolyte interphase (SEI) for lithium-ion batteries [J]. *npj Computational Materials*, 2018, **4**: 15.

---

*全文字数统计：约5 200字（含图注与参考文献标注，正文主体约4 800字）*
