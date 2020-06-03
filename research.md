---
layout: article
titles:
  # @start locale config
  en      : &EN       Research
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS  研究方向
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT  研究方向
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  ko      : &KO       Research
  ko-KR   : *KO
  fr      : &FR       Research
  fr-BE   : *FR
  fr-CA   : *FR
  fr-CH   : *FR
  fr-FR   : *FR
  fr-LU   : *FR
  # @end locale config
key: page-research
show_title: false
show_edit_on_github: true
---

## 半刚性高分子的自洽场理论及数值方法

很多实际运用的高分子体系中存在一定程度的链刚性。例如，为了提高材料的力学强度， 通常在柔性单元中引入刚性单体与之共聚；应用于光电器件的含共轭键刚性单元的嵌段高分子； 合成多肽；生物大分子，蛋白质，聚电解质及DNA等都是半刚性高分子。我们用蠕虫状链（wormlike chain） 代替柔性高分子的Gaussian chain模型，发展了各种含有半刚性特征的主链/侧链液晶高分子的自洽平均场理论。 然而，相比于高斯链，由于增加了链段的取向自由度，求解蠕虫状链的构象微分方程要困难许多， 整个计算不仅维数更高，而且在求解关于链段分布的扩散方程时难于使用高斯链体系中非常有效的谱方法和实空间方法。 我们通过采用三角网格化离散的单位球面描述链段的取向 ，直接在3D实空间用有限体积法解出含有链段取向的链传播子的扩散方程。 从而可以方便地考虑链段的三维空间取向。如图1所示，我们得到了刚－柔嵌段高分子的组成分布在1D空间的相图。 

<img src="https://s1.ax1x.com/2020/06/03/tdJPKI.png" alt="pic01" width="35%" height="auto" /><img src="https://s1.ax1x.com/2020/06/03/tdJirt.jpg" alt="research01" width="45%" height="auto" />

在成功实现了在一维位置空间有效、精确数值求解半刚性高分子链自洽场方程的基础上，进一步将其推广到二维空间。 采用目前流行的显卡核心计算（GPU）以提高求解速度和效率。除了包括一维空间中典型的isotropic、nematic及层状smectic相以外， 还包括非层状相，如四角堆积的椭圆形结构。此外，与一维空间得到的相图相同，相图中的大部分区间是层状结构，如图2所示。 通过在位置空间及取向空间分别采用FFTW和球谐变换（借助spherepack库）， 我们进一步发展了用高效、稳定的准谱方法求解半刚性高分子的自洽场方法。

<img src="https://s1.ax1x.com/2020/06/03/tdJS8H.jpg" alt="research02" width="95%" height="auto" />

## 弯曲曲面上的高分子接枝刷、任意复杂几何形状基底受限的嵌段高分子

采用所谓的“masking”方法，即采用“空穴”函数来描述有一定厚度的硬壁， 从而利用基于快速Fourier变换的准谱方法有效求解球面上共混高分子刷的自洽场方程， 得到了一系列海岛数目从2到12而且高度对称的海岛结构及刷子的尺寸标度关系。如图3所示， 我们的工作将对结构明确的两组分聚合物刷在环境保护、纳米技术及其它领域的应用产生重要意义。

<img src="https://s1.ax1x.com/2020/06/03/tdJp2d.jpg" alt="research03" width="55%" height="auto" />

## 非均相体系动力学

将可变元胞形状方法引入动态自洽场理论，用于研究空间非均相复杂高分子体系的流变及动力学行为。 相比以往的唯象动力学理论方法，我们的方法可考虑链构型特点，可计算体系的应力分布及应力-应变行为 。例如预测了二元共混物与二嵌段共聚物在外加剪切流场的作用下的形态及应力-应变行为，如图4所示，与实验结果吻合。 该方法还可用于模拟动态力学性能测试以及其他的动态力学测试方法如恒温频率扫描和同频率温度扫描。

<img src="https://s1.ax1x.com/2020/06/03/tdJ9xA.jpg" alt="research04" width="95%" height="auto" />

## 嵌段高分子在稀溶液中的聚集行为

运用自洽平均场理论，考察了复杂拓扑链结构的嵌段高分子及共混物在溶液中的聚集行为， 得到了许多新的胶束和囊泡的形态及其形成规律。例如，发现ABC线型三嵌段高分子本身的微相分离 与高分子与溶剂间发生宏观相分离并存的现象。研究了星型ABC三嵌段高分子/AB两嵌段高分子共混体系 在溶液中的聚集行为，发现采用嵌段高分子共混可以得到一些复杂有趣的胶束，例如相当长的wormlike， raspberry等胶束，如图5所示。巧妙地设计了由两种不同链长嵌段高分子组成的共混物， 研究了这种特殊的多分散嵌段高分子体系在溶液中的自组装形态，发现短链更易分布在囊泡内壁， 而长链更易分布在外壁，与自组装领域著名的实验小组Eisenberg的实验结果吻合。

<img src="https://s1.ax1x.com/2020/06/03/tdGzPe.jpg" alt="research05" width="85%" height="auto" />