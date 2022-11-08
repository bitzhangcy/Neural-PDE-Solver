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
    <td>&ensp;<a href="#efficiency">2.5 Efficiency</a></td>
    <td>&ensp;<a href="#explainability">2.6 Explainability</a></td>
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

1. **Physics-informed machine learning approach for augmenting turbulence models: A comprehensive framework.** Physical Review Fluids 2018. [paper](https://journals.aps.org/prfluids/abstract/10.1103/PhysRevFluids.3.074602)

   *Jin-Long Wu, Heng Xiao, and Eric Paterson.* 

1. **Physics-informed machine learning approach for augmenting turbulence models: A comprehensive framework.** Physical Review Fluids 2018. [paper](https://journals.aps.org/prfluids/abstract/10.1103/PhysRevFluids.3.074602)

   *Chuizheng Meng, Sungyong Seo, Defu Cao, Sam Griesemer, and Yan Liu.* 

1. **A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data.** Computer Methods in Applied Mechanics and Engineering 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001207?via%3Dihub)

   *Lu Lu,Xuhui Meng, Shengze Cai,Zhiping Mao, Somdatta Goswami, Zhongqiang Zhang, George EmKarniadakis.* 

1. **When physics meets machine learning: A survey of physics-informed machine learning.** arXiv 2022. [paper](https://arxiv.org/abs/2203.16797)

   *Chuizheng Meng, Sungyong Seo, Defu Cao, Sam Griesemer, and Yan Liu.* 

1. **An overview on deep learning-based approximation methods for partial differential equations.** arXiv 2020. [paper](https://arxiv.org/abs/2012.12348)

   *Christian Beck, Martin Hutzenthaler, Arnulf Jentzen, and Benno Kuckuck.* 

1. **Three ways to solve partial differential equations with neural networks—A review.** GAMM‐Mitteilungen 2021. [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/gamm.202100006)

   *Jan Blechschmidt and Oliver G. Ernst.* 

1. **Combining machine learning and domain decomposition methods for the solution of partial differential equations—A review.** GAMM‐Mitteilungen 2021. [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/gamm.202100001)

   *Alexander Heinlein, Axel Klawonn, Martin Lanser, and Janine Weber.* 

## [Models](#content) 

### [PINN](#content)

1. **Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations.** Journal of Computational Physics 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999118307125)

   *M.Raissia, P.Perdikarisb, and G.E.Karniadakisa.*

1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** Journal of Machine Learning Research 2018. [paper](https://www.jmlr.org/papers/volume19/18-046/18-046.pdf)

   *Maziar Raissi.*

1. **Understanding and mitigating gradient flow pathologies in physics-informed neural networks.** SIAM Journal on Scientific Computing 2021. [paper](https://epubs.siam.org/doi/10.1137/20M1318043)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, George EmKarniadakis.*

1. **Adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303584)

   *Yibo Yang and Paris Perdikaris.*

1. **hp-VPINNs: Variational physics-informed neural networks with domain decomposition.** Computer Methods in Applied Mechanics and Engineering 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520307325)

   *Ehsan Kharazmi, Zhongqiang Zhang, and George E.M.Karniadakis.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing 2021. [paper](https://epubs.siam.org/doi/10.1137/21M1397908)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **Adaptive activation functions accelerate convergence in deep and physics-informed neural networks.** Journal of Computational Physics 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119308411)

   *Ameya D.Jagtap, KenjiKawaguchi, and George EmKarniadakis.*

1. **Parallel physics-informed neural networks via domain decomposition.** Journal of Computational Physics 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005787)

   *Khemraj Shukla, Ameya D.Jagtap, George EmKarniadakis.*

1. **Physics-informed multi-LSTM networks for metamodeling of nonlinear structures.** Computer Methods in Applied Mechanics and Engineering 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520304114)

   *Ruiyang Zhang, Yang Liu, Hao Sun.*

1. **Gradient-enhanced physics-informed neural networks for forward and inverse PDE problems.** Computer Methods in Applied Mechanics and Engineering 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001438?via%3Dihub)

   *Jeremy Yu, Lu Lu, Xuhui Meng, George EmKarniadakis.*

1. **When and why PINNs fail to train: A neural tangent kernel perspective.** Journal of Computational Physics 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100663X)

   *SifanWang, XinlingYu, and ParisPerdikaris.*

1. **Understanding and mitigating gradient pathologies in physics-informed neural networks.** arXiv 2020. [paper](https://arxiv.org/abs/2001.04536)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **Understanding and mitigating gradient pathologies in physics-informed neural networks.** arXiv 2020. [paper](https://arxiv.org/abs/2001.04536)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing 2021. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1397908?journalCode=sjoce3)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **PPINN: Parareal physics-informed neural network for time-dependent PDEs.** Computer Methods in Applied Mechanics and Engineering 2020. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782520304357)

   *XuhuiMeng, ZhenLi, DongkunZhang, and George EmKarniadakis.*

1. **Scientific machine learning through physics–informed neural networks: Where we are and what’s next.** Beyond traditional AI: the impact of Machine Learning on Scientific Computing 2022. [book](https://link.springer.com/article/10.1007/s10915-022-01939-z)

   *MingyuanYang and John T.Foster*

1. **When do extended physics-informed neural networks (XPINNs) improve generalization?** SIAM Journal on Scientific Computing 2022.  [paper](https://epubs.siam.org/doi/abs/10.1137/21M1447039)

   *Zheyuan Hu, Ameya D. Jagtap, George Em Karniadakis, and Kenji Kawaguchi.*

### [DeepONet](#content)

1. **Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators.** Nature Machine Intelligence 2021. [paper](https://www.nature.com/articles/s42256-021-00302-5)

   *Lu Lu, Pengzhan Jin, Guofei Pang, Zhongqiang Zhang, an George Em Karniadakis.*

1. **Learning the solution operator of parametric partial differential equations with physics-informed DeepONets.** Science Advances 2021. [paper](https://www.science.org/doi/10.1126/sciadv.abi8605)

   *Wang  Sifan, Hanwen Wang, and Paris Perdikaris.*

1. **Variable-input deep operator networks.** arXiv 2022. [paper](https://arxiv.org/abs/2205.11404)

   *Michael Prasthofer, Tim De Ryck, and Siddhartha Mishra..*

1. **MIONet: Learning multiple-input operators via tensor product.** arXiv 2022. [paper](https://arxiv.org/abs/2202.06137)

   *Jeremy Yu, Lu Lu, Xuhui Meng, George EmKarniadakis.*

### [Fourier Operator](#content)

1. Fourier neural operator for parametric partial differential equations.** ICLR 2021. [paper](https://openreview.net/forum?id=c8P9NQVtmnO)

   *Zongyi Li, Nikola Borislavov Kovachki, Kamyar Azizzadenesheli, Burigede liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Neural Operator: Graph Kernel Network for Partial Differential Equations.** arXiv 2020. [paper](https://arxiv.org/abs/2003.03485)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Multipole graph neural operator for parametric partial differential equations.** NeurIPS 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496291)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

### [Graph Networks](#content)

1. **Message passing neural PDE solvers.** ICLR  2022. [paper](https://openreview.net/forum?id=vSix3HPYKSU)

   *Johannes Brandstetter, Daniel E. Worrall, and Max Welling.*

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP)

   *Xu Han, Han Gao, Tobias Pfaff, Jian-Xun Wang, and Liping Liu.*

1. **Learning mesh-based simulation with graph networks.** ICLR 2021. [paper](https://openreview.net/forum?id=roNqYL0_XP)

   *Tobias Pfaff, Meire Fortunato, Alvaro Sanchez-Gonzalez, and Peter Battaglia.*
   
1. **Modular flows: Differential molecular generation.** NIPS 2022. [paper](https://openreview.net/forum?id=kCnwOP-FYdz)

   *Yogesh Verma, Samuel Kaski, Markus Heinonen, and Vikas Garg.*
1. **On the robustness of graph neural diffusion to topology perturbations.** arXiv 2022. [paper](https://arxiv.org/abs/2209.07754)

   *Yang Song, Qiyu Kang, Sijie Wang, Zhao Kai, and Wee Peng Tay.*

1. **STONet: A neural-operator-driven spatio-temporal network.** arXiv 2022. [paper](https://arxiv.org/abs/2204.08414)

   *Haitao Lin, Guojiang Zhao, Lirong Wu, and Stan Z. Li.*

1. **GRAND: Graph neural diffusion.** ICML 2021. [paper](https://openreview.net/forum?id=_1fu_cjsaRE)

   *Benjamin Paul Chamberlain, James Rowbottom, Maria I. Gorinova, Stefan D Webb, Emanuele Rossi, and Michael M. Bronstein.*

1. **GRAND++: Graph neural diffusion with a source term.** ICML 2022. [paper](https://openreview.net/forum?id=EMxu-dzvJk)

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.*

### [Machine Learning](#content)
1. **Machine learning–accelerated computational fluid dynamics.** Proceedings of the National Academy of Sciences, 2021. [paper](https://www.pnas.org/doi/10.1073/pnas.2101784118)

   *Dmitrii Kochkov,  Jamie A. Smith, Ayya Alieva, and Stephan Hoyer.*

1. **Solving high-dimensional partial differential equations using deep learning.** Proceedings of the National Academy of Sciences 2018. [paper](https://www.pnas.org/doi/10.1073/pnas.1718942115)

   *Jiequn Han, Arnulf Jentzen, and Weinan E.*


1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** Journal of Machine Learning Research 2018. [paper](https://www.jmlr.org/papers/v19/18-046.html)

   *Maziar Raissi.*




### [Explainability](#content)



## [Mechanism](#content) 

### [Attention](#content)
   1. **Learning operators with coupled attention.** ICML 2022. [paper](https://www.jmlr.org/papers/v23/21-1521.html)

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.*

   1. **GRAND++: Graph neural diffusion with a source term.** Journal of Machine Learning Research 2022. [paper](https://openreview.net/forum?id=EMxu-dzvJk)

   *Georgios Kissas, Jacob H. Seidman, Leonardo Ferreira Guilhoto, Victor M. Preciado, George J. Pappas, and Paris Perdikaris.*

   1. **Choose a Transformer: Fourier or Galerkin.** NIPS  2021. [paper](https://openreview.net/forum?id=ssohLcmn4-r)

   *Shuhao Cao.* 

   1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS  2021. [paper](https://arxiv.org/abs/2009.04544)

   *Levi D. McClenny and Ulisses Braga-Neto.*

   1. **Transformer for partial differential equations' operator learning.** arXiv   2022. [paper](https://arxiv.org/abs/2205.13671)

   *Zijie Li, Kazem Meidani, and Amir Barati Farimani.*

   1. **SiT: Simulation transformer for particle-based physics simulation.** ICLR  2022. [paper](https://openreview.net/forum?id=DBOibe1ISzB)

   *Yidi Shao, Chen Change Loy, and Bo Dai.*

### [Meta Learning](#content)
   1. **Meta-auto-decoder for solving parametric partial differential equations.** arXiv 2022. [paper](https://arxiv.org/abs/2111.08823)

   *Xiang Huang, Zhanhong Ye, Hongsheng Liu, Beiji Shi, Zidong Wang, Kang Yang, Yang Li, Bingya Weng, Min Wang, Haotian Chu, Jing Zhou, Fan Yu, Bei Hua, Lei Chen, and Bin Dong.*

   1. **One-shot learning for solution operators of partial differential equations.** ICLR 2021. [paper](https://arxiv.org/abs/2104.05512)

   *Lu Lu, Haiyang He, Priya Kasimbeg, Rishikesh Ranade, and Jay Pathak.*


### [Benchmark](#content)
1. **PDEBench: An extensive benchmark for scientific machine learning.** NIPS 2022. [paper](https://openreview.net/forum?id=dh_MkX0QfrK)

   *Makoto Takamoto, Timothy Praditia, Raphael Leiteritz, Dan MacKinlay, Francesco Alesiani, and Dirk Pflüger, Mathias Niepert.*

### [GAN](#content)
1. **Weak adversarial networks for high-dimensional partial differential equations.** Journal of Computational Physics 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120301832)

   *YaohuaZang, GangBao, XiaojingYe, and HaominZhou.*



## [Applications](#content)
### [Optimization](#content)
1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*

1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*

1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*

1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*


### [Wave](#content)
1. **DeepONet prediction of linear instability waves in high-speed boundary layers.** arXiv 2021. [paper](https://arxiv.org/abs/2105.08697)

   *Patricio Clark Di Leoni, Lu Lu, Charles Meneveau, George Karniadakis, and Tamer A. Zaki.*

