# Neural-PDE-Solver

PDE: Partial Differentiable Equation

Contributed by Chunyang Zhang.

## [Content](#content)

<table>
<tr><td colspan="2"><a href="#survey-papers">1. Survey</a></td></tr> 
<tr><td colspan="2"><a href="#models">2. Models</a></td></tr>
<tr>
    <td>&ensp;<a href="#pinn">2.1 PINN</a></td>
    <td>&ensp;<a href="#deeponet">2.2 DeepONet</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#fourier-operator">2.3 Fourier Operator</a></td>
    <td>&ensp;<a href="#graph-networks">2.4 Graph Networks</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#machine-learning">2.5 Machine Learning</a></td>
    <td>&ensp;<a href="#identification">2.6 Identification</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#finite-element&volume">2.7 Finite Element & Volume</a></td>
    <td>&ensp;<a href="#convolutional-filter">2.8 Convolutional Filter</a></td>
</tr>
<tr><td colspan="2"><a href="#models">3. Mechanism</a></td></tr>
<tr>
    <td>&ensp;<a href="#attention">3.1 Attention</a></td>
    <td>&ensp;<a href="#deeponet2">3.2 DeepONet2</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#operator3">3.3  Operator3</a></td>
    <td>&ensp;<a href="#graph-networks4">3.4 Graph Networks4</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#efficiency5">3.5 Efficiency5</a></td>
    <td>&ensp;<a href="#explainability6">3.6 Explainability6</a></td>
</tr>
<tr><td colspan="2"><a href="#applications">4. Applications</a></td></tr> 
<tr>
    <td>&ensp;<a href="#physics">4.1 Physics</a></td>
    <td>&ensp;<a href="#chemistry-and-biology">4.2 Chemistry and Biology</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#knowledge-graph">4.3 Knowledge Graph</a></td>
    <td>&ensp;<a href="#recommender-systems">4.4 Recommender Systems</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#computer-vision">4.5 Computer Vision</a></td>
    <td>&ensp;<a href="#natural-language-processing">4.6 Natural Language Processing</a></td>
</tr> 
</table>






## [Survey papers](#content)

1. **Physics-informed machine learning.** Nature Reviews Physics, 2021. [paper](https://www.nature.com/articles/s42254-021-00314-5)

   *George Em Karniadakis, Ioannis G. Kevrekidis, Lu Lu, Paris Perdikaris, Sifan Wang, and Liu Yang.*

1. **DeepXDE: A deep learning library for solving differential equations.** SIAM Review, 2021. [paper](https://epubs.siam.org/doi/abs/10.1137/19M1274067)

   *Lu Lu, Xuhui Meng, Zhiping Mao, and George Em Karniadakis.*

1. **Neural operator: Learning maps between function spaces.** arXiv, 2021. [paper](https://arxiv.org/abs/2108.08481)

   *Nikola Kovachki, Zongyi Li, Burigede Liu, Kamyar Azizzadenesheli, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Physics-informed machine learning approach for augmenting turbulence models: A comprehensive framework.** Physical Review Fluids, 2018. [paper](https://journals.aps.org/prfluids/abstract/10.1103/PhysRevFluids.3.074602)

   *Jin-Long Wu, Heng Xiao, and Eric Paterson.* 

1. **A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001207?via%3Dihub)

   *Lu Lu,Xuhui Meng, Shengze Cai,Zhiping Mao, Somdatta Goswami, Zhongqiang Zhang, George EmKarniadakis.* 

1. **When physics meets machine learning: A survey of physics-informed machine learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.16797)

   *Chuizheng Meng, Sungyong Seo, Defu Cao, Sam Griesemer, and Yan Liu.* 

1. **An overview on deep learning-based approximation methods for partial differential equations.** arXiv, 2020. [paper](https://arxiv.org/abs/2012.12348)

   *Christian Beck, Martin Hutzenthaler, Arnulf Jentzen, and Benno Kuckuck.* 

1. **Three ways to solve partial differential equations with neural networks—A review.** GAMM‐Mitteilungen, 2021. [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/gamm.202100006)

   *Jan Blechschmidt and Oliver G. Ernst.* 

1. **Combining machine learning and domain decomposition methods for the solution of partial differential equations—A review.** GAMM‐Mitteilungen, 2021. [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/gamm.202100001)

   *Alexander Heinlein, Axel Klawonn, Martin Lanser, and Janine Weber.* 

## [Models](#content) 

### [PINN](#content)

1. **Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999118307125)

   *M.Raissia, P.Perdikarisb, and G.E.Karniadakisa.*

1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** Journal of Machine Learning Research, 2018. [paper](https://www.jmlr.org/papers/volume19/18-046/18-046.pdf)

   *Maziar Raissi.*

1. **Characterizing possible failure modes in physics-informed neural networks.** NIPS, 2021. [paper](https://openreview.net/forum?id=a2Gr9gNFD-J)

   *Aditi Krishnapriyan, Aditi_Krishnapriyan, Amir Gholami, Shandian Zhe, Robert Kirby, Michael W. Mahoney.*

1. **Understanding and mitigating gradient flow pathologies in physics-informed neural networks.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/20M1318043)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, George EmKarniadakis.*

1. **Adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303584)

   *Yibo Yang and Paris Perdikaris.*

1. **hp-VPINNs: Variational physics-informed neural networks with domain decomposition.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520307325)

   *Ehsan Kharazmi, Zhongqiang Zhang, and George E.M.Karniadakis.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/21M1397908)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **Adaptive activation functions accelerate convergence in deep and physics-informed neural networks.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119308411)

   *Ameya D.Jagtap, KenjiKawaguchi, and George EmKarniadakis.*

1. **Parallel physics-informed neural networks via domain decomposition.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005787)

   *Khemraj Shukla, Ameya D.Jagtap, George EmKarniadakis.*

1. **Physics-informed multi-LSTM networks for metamodeling of nonlinear structures.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520304114)

   *Ruiyang Zhang, Yang Liu, Hao Sun.*

1. **Gradient-enhanced physics-informed neural networks for forward and inverse PDE problems.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001438?via%3Dihub)

   *Jeremy Yu, Lu Lu, Xuhui Meng, George EmKarniadakis.*

1. **When and why PINNs fail to train: A neural tangent kernel perspective.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100663X)

   *SifanWang, XinlingYu, and ParisPerdikaris.*

1. **Understanding and mitigating gradient pathologies in physics-informed neural networks.** arXiv, 2020. [paper](https://arxiv.org/abs/2001.04536)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **Understanding and mitigating gradient pathologies in physics-informed neural networks.** arXiv, 2020. [paper](https://arxiv.org/abs/2001.04536)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1397908?journalCode=sjoce3)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **PPINN: Parareal physics-informed neural network for time-dependent PDEs.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782520304357)

   *XuhuiMeng, ZhenLi, DongkunZhang, and George EmKarniadakis.*

1. **Scientific machine learning through physics–informed neural networks: Where we are and what’s next.** Beyond traditional AI: the impact of Machine Learning on Scientific Computing, 2022. [book](https://link.springer.com/article/10.1007/s10915-022-01939-z)

   *MingyuanYang and John T.Foster*

1. **When do extended physics-informed neural networks (XPINNs) improve generalization?** SIAM Journal on Scientific Computing, 2022.  [paper](https://epubs.siam.org/doi/abs/10.1137/21M1447039)

   *Zheyuan Hu, Ameya D. Jagtap, George Em Karniadakis, and Kenji Kawaguchi.*

1. **Respecting causality is all you need for training physics-informed neural networks.** arXiv, 2021.  [paper](https://arxiv.org/abs/2203.07404)

   *Sifan Wang, Shyam Sankaran, and Paris Perdikaris.*

1. **Robust learning of physics informed neural networks.** arXiv, 2021.  [paper](https://arxiv.org/abs/2110.13330)

   *Chandrajit Bajaj, Luke McLennan, Timothy Andeen, and Avik Roy.*

1. **Learning physics-informed neural networks without stacked back-propagation.** arXiv, 2022.  [paper](https://arxiv.org/abs/2202.09340)

   *Di He, Wenlei Shi, Shanda Li, Xiaotian Gao, Jia Zhang, Jiang Bian, Liwei Wang, and Tieyan Liu.*

1. **Physics informed RNN-DCT networks for time-fependent partial differential equations.** International Conference on Computational Science, 2022.  [paper](https://link.springer.com/chapter/10.1007/978-3-031-08754-7_45)

   *Benjamin Wu, Oliver Hennigh, Jan Kautz, Sanjay Choudhry, and Wonmin Byeon.*

### [DeepONet](#content)

1. **Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators.** Nature Machine Intelligence, 2021. [paper](https://www.nature.com/articles/s42256-021-00302-5)

   *Lu Lu, Pengzhan Jin, Guofei Pang, Zhongqiang Zhang, an George Em Karniadakis.*

1. **Learning the solution operator of parametric partial differential equations with physics-informed DeepONets.** Science Advances, 2021. [paper](https://www.science.org/doi/10.1126/sciadv.abi8605)

   *Wang  Sifan, Hanwen Wang, and Paris Perdikaris.*

1. **Variable-input deep operator networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.11404)

   *Michael Prasthofer, Tim De Ryck, and Siddhartha Mishra..*

1. **MIONet: Learning multiple-input operators via tensor product.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.06137)

   *Jeremy Yu, Lu Lu, Xuhui Meng, George EmKarniadakis.*

1. **Error estimates for DeepONets: a deep learning framework in infinite dimensions.** Transactions of Mathematics and Its Applications, 2022. [paper](https://academic.oup.com/imatrm/article/6/1/tnac001/6542709)

   *Samuel Lanthaler, Siddhartha Mishra, and George E Karniadakis.*

1. **Long-time integration of parametric evolution equations with physics-informed DeepONets.** arXiv, 2021. [paper](https://arxiv.org/abs/2106.05384)

   *Sifan Wang and Paris Perdikaris.*

1. **Improved architectures and training algorithms for deep operator networks.** Journal of Scientific Computing, 2022. [paper](https://link.springer.com/article/10.1007/s10915-022-01881-0)

   *Sifan Wang, Hanwen Wang ,and Paris Perdikaris.*


### [Fourier Operator](#content)

1. Fourier neural operator for parametric partial differential equations.** ICLR, 2021. [paper](https://openreview.net/forum?id=c8P9NQVtmnO)

   *Zongyi Li, Nikola Borislavov Kovachki, Kamyar Azizzadenesheli, Burigede liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Neural Operator: Graph Kernel Network for Partial Differential Equations.** arXiv, 2020. [paper](https://arxiv.org/abs/2003.03485)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Multipole graph neural operator for parametric partial differential equations.** NeurIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496291)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Factorized fourier neural operators.** ICLR, 2023. [paper](https://openreview.net/forum?id=tmIiMPl4IPa)

   *Alasdair Tran, Alexander Mathews, Lexing Xie, and Cheng Soon Ong.*

1. **On the eigenvector bias of Fourier feature networks: From regression to solving multi-scale PDEs with physics-informed neural networks.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521002759)

   *Sifan Wang, Hanwen Wang, and Paris Perdikaris.*

### [Graph Networks](#content)

1. **Message passing neural PDE solvers.** ICLR,  2022. [paper](https://openreview.net/forum?id=vSix3HPYKSU)

   *Johannes Brandstetter, Daniel E. Worrall, and Max Welling.*

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR, 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP)

   *Xu Han, Han Gao, Tobias Pfaff, Jian-Xun Wang, and Liping Liu.*

1. **Learning mesh-based simulation with graph networks.** ICLR, 2021. [paper](https://openreview.net/forum?id=roNqYL0_XP)

   *Tobias Pfaff, Meire Fortunato, Alvaro Sanchez-Gonzalez, and Peter Battaglia.*
   
1. **Modular flows: Differential molecular generation.** NIPS, 2022. [paper](https://openreview.net/forum?id=kCnwOP-FYdz)

   *Yogesh Verma, Samuel Kaski, Markus Heinonen, and Vikas Garg.*
1. **On the robustness of graph neural diffusion to topology perturbations.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.07754)

   *Yang Song, Qiyu Kang, Sijie Wang, Zhao Kai, and Wee Peng Tay.*

1. **STONet: A neural-operator-driven spatio-temporal network.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.08414)

   *Haitao Lin, Guojiang Zhao, Lirong Wu, and Stan Z. Li.*

1. **GRAND: Graph neural diffusion.** ICML, 2021. [paper](https://openreview.net/forum?id=_1fu_cjsaRE)

   *Benjamin Paul Chamberlain, James Rowbottom, Maria I. Gorinova, Stefan D Webb, Emanuele Rossi, and Michael M. Bronstein.*

1. **GRAND++: Graph neural diffusion with a source term.** ICML, 2022. [paper](https://openreview.net/forum?id=EMxu-dzvJk)

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.*

1. **Learning continuous-time PDEs from sparse data with graph neural networks.** ICLR, 2021. [paper](https://openreview.net/pdf?id=aUX5Plaq7Oy)

   *Valerii Iakovlev, Markus Heinonen, and Harri Lähdesmäki.*

### [Machine Learning](#content)
1. **Machine learning–accelerated computational fluid dynamics.** Proceedings of the National Academy of Sciences, 2021. [paper](https://www.pnas.org/doi/10.1073/pnas.2101784118)

   *Dmitrii Kochkov,  Jamie A. Smith, Ayya Alieva, and Stephan Hoyer.*

1. **Solving high-dimensional partial differential equations using deep learning.** Proceedings of the National Academy of Sciences, 2018. [paper](https://www.pnas.org/doi/10.1073/pnas.1718942115)

   *Jiequn Han, Arnulf Jentzen, and Weinan E.*

1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** Journal of Machine Learning Research, 2018. [paper](https://www.jmlr.org/papers/v19/18-046.html)

   *Maziar Raissi.*


1. **Nonlocal kernel network (NKN): A stable and resolution-independent deep neural network.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122005988)

   *HuaiqianYou, Yue Yu, Marta D'Elia, Tian Gao, Stewart Silling.*

1. **The cost-accuracy trade-off in operator learning with neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.13181)

   *Maarten V. de Hoop, Daniel Zhengyu Huang, Elizabeth Qian,amd  Andrew M. Stuart.*

1. **Multi-scale deep neural networks for solving high dimensional PDEs.** arXiv, 2019. [paper](https://www.science.org/doi/10.1126/sciadv.1602614)

   *Samuel H. Rudy, Steven L. Brunton,  Joshua L. Proctor, and  J. Nathan Kutz.*

1. **Model reduction and neural networks for parametric PDEs.** SMAI Journal of Computational Mathematics, 2021. [paper](https://smai-jcm.centre-mersenne.org/item/SMAI-JCM_2021__7__121_0/)

   *Kaushik Bhattacharya, Bamdad Hosseini, Nikola B. Kovachki, and Andrew M. Stuart.*

1. **MOD-Net: A Machine Learning Approach via Model-Operator-Data Network for Solving PDEs.** Communications in Computational Physics, 2022. [paper](https://global-sci.org/intro/article_detail/cicp/20860.html#)

   *Lulu Zhang, Tao Luo, Yaoyu Zhang, Weinan E, Zhi-Qin John Xu, and Zheng Ma.*

### [Identification](#content)
1. **Data-driven discovery of partial differential equations.** Science Advance, 2017. [paper](https://arxiv.org/abs/1910.11710)

   *Wei Cai, Zhi-Qin John Xu.*

1. **Discovering nonlinear PDEs from scarce data with physics-encoded learning.** ICLR, 2022. [paper](https://openreview.net/pdf?id=Vog_3GXsgmb)

   *Chengping Rao, Pu Ren, Yang Liu, and Hao Sun.*

1. **Data-driven discovery of partial differential equation models with latent variables.** Physical Review E, 2019. [paper](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.100.022219)

   *Patrick A. K. Reinbold and Roman O. Grigoriev.*

1. **Deep neural network modeling of unknown partial differential equations in nodal space.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100677X)

   *Zhen Chen, and Victor Churchill, Kailiang Wu, and Dongbin Xiu.*

1. **PDE-READ: Human-readable partial differential equation discovery using deep learning.** Neural Networks, 2022. [paper](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.100.022219)

   *Robert Stephany and Christopher Earls.*

### [Finite Element/Volume](#content)
1. **Composing partial differential equations with physics-aware neural networks.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/karlbauer22a/karlbauer22a.pdf)

   *Matthias Karlbauer, Timothy Praditia, Sebastian Otte, Sergey Oladyshkin, and Wolfgang Nowak.*

1. **Learning the dynamics of physical systems from sparse observations with finite element networks.** ICLR, 2022. [paper](https://openreview.net/forum?id=HFmAukZ-k-2)

   *Marten Lienen and Stephan Günnemann.*

1. **Hybrid finite difference with the physics-informed neural network for solving PDE in complex geometries** arXiv, 2022. [paper](https://arxiv.org/pdf/2202.07926.pdf)

   *Zixue Xiang, Wei Peng, Weien Zhou, and Wen Yao.*

### [Convolutional Filter](#content)
1. **PDE-Net: Learning PDEs from data.** ICML, 2018.. [paper](https://proceedings.mlr.press/v80/long18a.html)

   *Zichao Long, Yiping Lu, Xianzhong Ma, and Bin Dong.*

1. **PDE-Net 2.0: Learning PDEs from data with a numeric-symbolic hybrid deep network.** Journal of Computational Physics, 2019.. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119306308)

   *ZichaoLong, YipingLu, and  Bin Dong.*

## [Mechanism](#content) 
### [Attention](#content)
1. **Learning operators with coupled attention.** Journal of Machine Learning Research, 2022. [paper](https://www.jmlr.org/papers/v23/21-1521.html) 

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.* 

1. **Choose a Transformer: Fourier or Galerkin.** NIPS, 2021. [paper](https://openreview.net/forum?id=ssohLcmn4-r)

   *Shuhao Cao.* 

1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS, 2021. [paper](https://arxiv.org/abs/2009.04544) 

   *Levi D. McClenny and Ulisses Braga-Neto.*

1. **Transformer for partial differential equations' operator learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.13671) 

   *Zijie Li, Kazem Meidani, and Amir Barati Farimani.*

1. **SiT: Simulation transformer for particle-based physics simulation.** ICLR, 2022. [paper](https://openreview.net/forum?id=DBOibe1ISzB) 

   *Yidi Shao, Chen Change Loy, and Bo Dai.*

1. **Physics-informed attention-based neural network for hyperbolic partial differential equations: application to the Buckley–Leverett problem.**  Scientific Reports, 2022. [paper](https://www.nature.com/articles/s41598-022-11058-2) 

   *Ruben Rodriguez-Torrado, Pablo Ruiz, Luis Cueto-Felgueroso, Michael Cerny Green, Tyler Friesen, Sebastien Matringe,and Julian Togelius .*

1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS, 2021. [paper](https://github.com/levimcclenny/SA-PINNs) 

   *Levi McClenny and Ulisses Braga-Neto.*

### [Meta Learning](#content)
1. **Meta-auto-decoder for solving parametric partial differential equations.** NIPS,, 2022. [paper](https://openreview.net/pdf?id=PwlW5Jri1Xt) 

   *Xiang Huang, Zhanhong Ye, Hongsheng Liu, Beiji Shi, Zidong Wang, Kang Yang, Yang Li, Bingya Weng, Min Wang, Haotian Chu, Jing Zhou, Fan Yu, Bei Hua, Lei Chen, and Bin Dong.*

1. **One-shot learning for solution operators of partial differential equations.** ICLR, 2021. [paper](https://arxiv.org/abs/2104.05512) 

   *Lu Lu, Haiyang He, Priya Kasimbeg, Rishikesh Ranade, and Jay Pathak.*

1. **Meta-learning PINN loss functions.** Journal of Computational Physics, 2022.  [paper](https://www.sciencedirect.com/science/article/pii/S0021999122001838)

   *Apostolos F Psaros,Kenji Kawaguchi, and George Em Karniadakis.*

1. **Physics-informed neural networks (PINNs) for parameterized PDEs: A Meta-learning approach.** arXiv,. 2021. [paper](https://arxiv.org/abs/2110.13361)

   *Michael Penwarden, Shandian Zhe, Akil Narayan, and Robert M. Kirby.*

### [Latent Space](#content)
1. **A Latent space solver for PDE generalization.** ICLR, 2021. [paper](https://arxiv.org/abs/2104.02452)

   *Rishikesh Ranade, Chris Hill, Haiyang He, Amir Maleki, and Jay Pathak.*

### [Benchmark](#content)
1. **PDEBench: An extensive benchmark for scientific machine learning.** NIPS, 2022. [paper](https://openreview.net/forum?id=dh_MkX0QfrK)

   *Makoto Takamoto, Timothy Praditia, Raphael Leiteritz, Dan MacKinlay, Francesco Alesiani, and Dirk Pflüger, Mathias Niepert.*

### [GAN](#content)
1. **A framework for data-driven solution and parameter estimation of PDEs using conditional generative adversarial networks.** Nature Computational Science, 2021. [paper](https://www.nature.com/articles/s43588-021-00171-3)

   *Teeratorn Kadeethum, Daniel O’Malley, Jan Niklas Fuhg, Youngsoo Choi, Jonghyun Lee, Hari S. Viswanathan, and Nikolaos Bouklas.*

1. **Weak adversarial networks for high-dimensional partial differential equations.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120301832)

   *YaohuaZang, GangBao, XiaojingYe, and HaominZhou.*

1. **Wasserstein generative adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003321)

   *YihangGao and Michael K.Ng.*

### [Solver](#content)
1. **Solver-in-the-loop: learning from differentiable physics to interact with iterative PDE-solvers.** NIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496237)

   *Kiwon Um, Robert Brand, Yun (Raymond) Fei, Philipp Holl, and Nils Thuerey.*

### [Variation](#content)
1. **PI-VAE: Physics-Informed Variational Auto-Encoder for stochastic differential equations.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522006193)

   *Weiheng Zhong, Hadi Meidani.*

1. **Variational Onsager Neural Networks (VONNs): A thermodynamics-based variational learning strategy for non-equilibrium PDEs.** Journal of the Mechanics and Physics of Solids, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0022509622000692)

   *Shenglin Huang, Zequn He, Bryan Chem, Celia Reina.*

### [Bayesian](#content)
1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, and George Em Karniadakis.*

## [Applications](#content)
### [Optimization](#content)
1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*

1. **An extended physics informed neural network for preliminary analysis of parametric optimal control problems.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13530)

   *Nicola Demo, Maria Strazzullo, and Gianluigi Rozza.*

1. **Optimal control of PDEs using physics-informed neural networks.** ICLR, 2022. [paper](https://openreview.net/forum?id=a3Rhl617hW)

   *Saviz Mowlavi and Saleh Nabi.*

1. **Solving PDE-constrained control problems using operator learning.** AAAI, 2022. [paper](https://aaai-2022.virtualchair.net/poster_aaai12978)

   *Rakhoon Hwang, Jae Yong Lee, Jin Young Shin, and Hyung Ju Hwang.*


### [Wave](#content)
1. **DeepONet prediction of linear instability waves in high-speed boundary layers.** arXiv, 2021. [paper](https://arxiv.org/abs/2105.08697)

   *Patricio Clark Di Leoni, Lu Lu, Charles Meneveau, George Karniadakis, and Tamer A. Zaki.*
