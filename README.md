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
    <td>&ensp;<a href="#green-function">2.5 Green Function</a></td>
    <td>&ensp;<a href="#finite-element-&-volume">2.6 Finite Element & Volume</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#convolutional-filter">2.7 Convolutional Filter</a></td>
    <td>&ensp;<a href="#other-operators">2.8 Other Operators</a></td>
</tr>
<tr>
    <td>&ensp;<a href=#identification"">2.9 Identification</a></td>
    <td>&ensp;<a href="#machine-learning">2.10 Machine Learning</a></td>
</tr>
<tr>
    <td>&ensp;<a href=#ode"">2.11 ODE</a></td>
    <td>&ensp;<a href="#"></a></td>
</tr>
<tr><td colspan="2"><a href="#models">3. Mechanism</a></td></tr>
<tr>
    <td>&ensp;<a href="#library">3.1 Library</a></td>
    <td>&ensp;<a href="#analysis">3.2 Analysis</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#attention">3.3 Attention</a></td>
    <td>&ensp;<a href="#neural-implicit-flow">3.4 Neural Implicit Flow</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#disentangle">3.5 Disentangle</a></td>
    <td>&ensp;<a href="#meta-learning">3.6 Meta Learning</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#latent-space">3.7 Latent Space</a></td>
    <td>&ensp;<a href="#loss-function">3.8 Loss Function</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#decomposation">3.9 Decomposation</a></td>
    <td>&ensp;<a href="#mesh">3.10 Mesh</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#disentangle">3.11 Disentangle</a></td>
    <td>&ensp;<a href="#meta-learning">3.12 Meta Learning</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#gan">3.13 GAN</a></td>
    <td>&ensp;<a href="#gussian-process">3.14 Gussian Process</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#solver">3.15 Solver</a></td>
    <td>&ensp;<a href="#variations">3.16 Variations</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#bayesian">3.17 Bayesian</a></td>
    <td>&ensp;<a href="#lagrangian">3.18 Lagrangian</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#uncertainty-quantification">3.19 Uncertainty Quantification</a></td>
    <td>&ensp;<a href="#active-learning">3.20 Active Learning</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#active-learning">3.21 Active Learning</a></td>
    <td>&ensp;<a href="#multi-scale">3.22 Multi-Scale</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#multi-fidelity">3.23 Multi-Fidelity</a></td>
    <td>&ensp;<a href="#multi-grid">3.24 Multi-Grid</a></td>
</tr>
<tr><td colspan="2"><a href="#applications">4. Applications</a></td></tr> 
<tr>
    <td>&ensp;<a href="#Optimal-control">4.1 Optimal Control</a></td>
    <td>&ensp;<a href="#fuild">4.2 Fuild</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#reconstruction">4.3 Reconstruction</a></td>
    <td>&ensp;<a href="#physics">4.4 Physics</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#image">4.5 Image</a></td>
    <td>&ensp;<a href="#manufacturing">4.6 Manufacturing</a></td>
</tr> 
</table>



## [Survey Papers](#content)
1. **Physics-informed machine learning.** Nature Reviews Physics, 2021. [paper](https://www.nature.com/articles/s42254-021-00314-5)

   *George Em Karniadakis, Ioannis G. Kevrekidis, Lu Lu, Paris Perdikaris, Sifan Wang, and Liu Yang.*

1. **Neural operator: Learning maps between function spaces.** arXiv, 2021. [paper](https://arxiv.org/abs/2108.08481)

   *Nikola Kovachki, Zongyi Li, Burigede Liu, Kamyar Azizzadenesheli, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Physics-informed machine learning approach for augmenting turbulence models: A comprehensive framework.** Physical Review Fluids, 2018. [paper](https://journals.aps.org/prfluids/abstract/10.1103/PhysRevFluids.3.074602)

   *Jin-Long Wu, Heng Xiao, and Eric Paterson.* 

1. **A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001207?via%3Dihub)

   *Lu Lu,Xuhui Meng, Shengze Cai,Zhiping Mao, Somdatta Goswami, Zhongqiang Zhang, George EmKarniadakis.* 

1. **Scientific machine learning through physics–informed neural networks: Where we are and what’s next.** Beyond traditional AI: the impact of Machine Learning on Scientific Computing, 2022. [book](https://link.springer.com/article/10.1007/s10915-022-01939-z)

   *MingyuanYang and John T.Foster*

1. **When physics meets machine learning: A survey of physics-informed machine learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.16797)

   *Chuizheng Meng, Sungyong Seo, Defu Cao, Sam Griesemer, and Yan Liu.* 

1. **An overview on deep learning-based approximation methods for partial differential equations.** arXiv, 2020. [paper](https://arxiv.org/abs/2012.12348)

   *Christian Beck, Martin Hutzenthaler, Arnulf Jentzen, and Benno Kuckuck.* 

1. **Three ways to solve partial differential equations with neural networks—A review.** GAMM‐Mitteilungen, 2021. [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/gamm.202100006)

   *Jan Blechschmidt and Oliver G. Ernst.* 

1. **Combining machine learning and domain decomposition methods for the solution of partial differential equations—A review.** GAMM‐Mitteilungen, 2021. [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/gamm.202100001)

   *Alexander Heinlein, Axel Klawonn, Martin Lanser, and Janine Weber.* 

1. **Physics-guided, physics-informed, and physics-encoded neural networks in scientific computing.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.07377)

   *Salah A Faroughi, Nikhil Pawar, Celio Fernandes, Subasish Das, Nima K. Kalantari, and Seyed Kourosh Mahjour.* 

1. **Partial differential equations meet deep neural networks: A survey.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.05567)

   *Shudong Huang, Wentao Feng, Chenwei Tang, and Jiancheng Lv.* 

## [Models](#content) 
### [PINN](#content)

1. **Hidden fluid mechanics: Learning velocity and pressure fields from flow visualizations.** Science, 2020. [paper](https://www.science.org/doi/10.1126/science.aaw4741)

   *Raissi, Maziar and Yazdani, Alireza and Karniadakis, and George Em.*

1. **Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999118307125)

   *M.Raissia, P.Perdikarisb, and G.E.Karniadakisa.*

1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** Journal of Machine Learning Research, 2018. [paper](https://www.jmlr.org/papers/volume19/18-046/18-046.pdf)

   *Maziar Raissi.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/21M1397908)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **Parallel physics-informed neural networks via domain decomposition.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005787)

   *Khemraj Shukla, Ameya D.Jagtap, George EmKarniadakis.*

1. **Physics-informed multi-LSTM networks for meta-modeling of nonlinear structures.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520304114)

   *Ruiyang Zhang, Yang Liu, Hao Sun.*

1. **Gradient-enhanced physics-informed neural networks for forward and inverse PDE problems.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001438?via%3Dihub)

   *Jeremy Yu, Lu Lu, Xuhui Meng, George EmKarniadakis.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **PPINN: Parareal physics-informed neural network for time-dependent PDEs.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782520304357)

   *XuhuiMeng, ZhenLi, DongkunZhang, and George EmKarniadakis.*

1. **CAN-PINN: A fast physics-informed neural network based on coupled-automatic–numerical differentiation method.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522001906)

   *Pao-Hsiung Chiu, Jian Cheng Wong, Chinchun Ooi, My Ha Dao, and Yew-Soon Ong.*

1. **Physics-augmented learning: A new paradigm beyond physics-informed learning.** NIPS, 2021. [paper](https://www.iamwawa.cn/daxiaoxie.html)

   *Ziming Liu, Yuanqi Du, Yunyue Chen, and Max Tegmark.*

1. **Robust learning of physics informed neural networks.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13330)

   *Chandrajit Bajaj, Luke McLennan, Timothy Andeen, and Avik Roy.*

1. **Learning physics-informed neural networks without stacked back-propagation.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.09340)

   *Di He, Wenlei Shi, Shanda Li, Xiaotian Gao, Jia Zhang, Jiang Bian, Liwei Wang, and Tieyan Liu.*

1. **NeuralPDE: Automating physics-informed neural networks (PINNs) with error approximations.** arXiv, 2021. [paper](https://arxiv.org/abs/2107.09443)

   *Kirill Zubov, Zoe McCarthy, Yingbo Ma, Francesco Calisto, Valerio Pagliarino, Simone Azeglio, Luca Bottero, Emmanuel Luján, Valentin Sulzer, Ashutosh Bharambe, Nand Vinchhi, Kaushik Balakrishnan, Devesh Upadhyay, and Chris Rackauckas.*

1. **Physics informed RNN-DCT networks for time-dependent partial differential equations.** International Conference on Computational Science, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-08754-7_45)

   *Benjamin Wu, Oliver Hennigh, Jan Kautz, Sanjay Choudhry, and Wonmin Byeon.*

1. **Physics-informed Karhunen-Loéve and neural network approximations for solving inverse differential equation problems.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122002923)

   *Jing Li, and Alexandre M.Tartakovsky.*

1. **Physics-informed neural networks with adaptive localized artificial viscosity.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.08802)

   *E.J.R. Coutinho, M. Dall'Aqua, L. McClenny, M. Zhong, U. Braga-Neto, and E. Gildin.*

1. **Physics-informed neural operator for learning partial differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2111.03794)

   *Zongyi Li, Hongkai Zheng, Nikola Kovachki, David Jin, Haoxuan Chen, Burigede Liu, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Fast neural network based solving of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.08978)

   *Jaroslaw Rzepecki, Daniel Bates, and Chris Doran.*

### [DeepONet](#content)
1. **Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators.** Nature Machine Intelligence, 2021. [paper](https://www.nature.com/articles/s42256-021-00302-5)

   *Lu Lu, Pengzhan Jin, Guofei Pang, Zhongqiang Zhang, an George Em Karniadakis.*

1. **Learning the solution operator of parametric partial differential equations with physics-informed DeepONets.** Science Advances, 2021. [paper](https://www.science.org/doi/10.1126/sciadv.abi8605)

   *Wang Sifan, Hanwen Wang, and Paris Perdikaris.*

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

1. **SVD perspectives for augmenting DeepONet flexibility and interpretability.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.12670)

   *Simone Venturi and Tiernan Casey.*

1. **Accelerated replica exchange stochastic gradient Langevin diffusion enhanced Bayesian DeepONet for solving noisy parametric PDEs.** arXiv, 2021. [paper](https://arxiv.org/abs/2111.02484)

   *Guang Lin, Christian Moya, and Zecheng Zhang.*

1. **Bi-fidelity modeling of uncertain and partially unknown systems using DeepONet.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.00997)

   *Subhayan De, Matthew Reynolds, Malik Hassanaly, Ryan N. King, and Alireza Doostan.*

1. **Deep transfer learning for partial differential equations under conditional shift with DeepONet.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.09810)

   *Somdatta Goswami, Katiana Kontolati, Michael D. Shields, and George Em Karniadakis.*

1. **MultiAuto-DeepONet: A multi-resolution autoencoder DeepONet for nonlinear dimension reduction, uncertainty quantification and operator learning of forward and inverse stochastic problems.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.03193)

   *Jiahao Zhang, Shiqi Zhang, and Guang Lin.*

### [Fourier Operator](#content)
1. **Fourier neural operator for parametric partial differential equations.** ICLR, 2021. [paper](https://openreview.net/forum?id=c8P9NQVtmnO)

   *Zongyi Li, Nikola Borislavov Kovachki, Kamyar Azizzadenesheli, Burigede liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **On universal approximation and error bounds for Fourier neural operators.** Journal of Machine Learning Research, 2021. [paper](https://dl.acm.org/doi/abs/10.5555/3546258.3546548)

   *Nikola Kovachki, Samuel Lanthaler, Siddhartha Mishra.*

1. **Neural operator: Graph kernel network for partial Differential equations.** arXiv, 2020. [paper](https://arxiv.org/abs/2003.03485)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Multipole graph neural operator for parametric partial differential equations.** NeurIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496291)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Factorized Fourier neural operators.** ICLR, 2023. [paper](https://openreview.net/forum?id=tmIiMPl4IPa)

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

1. **Learning large-scale subsurface simulations with a hybrid graph network simulator.** KDD, 2022. [paper](https://arxiv.org/abs/2206.07680)

   *Tailin Wu, Qinchen Wang, Yinan Zhang, Rex Ying, Kaidi Cao, Rok Sosič, Ridwan Jalali, Hassan Hamam, Marko Maucec, and Jure Leskovec.*

1. **Physics-informed graph neural Galerkin networks: A unified framework for solving PDE-governed forward and inverse problems.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521007076)

   *Han Gao, Matthew J.Zahr, and Jian-XunWang.*

1. **Modular flows: Differential molecular generation.** NIPS, 2022. [paper](https://openreview.net/forum?id=kCnwOP-FYdz)

   *Yogesh Verma, Samuel Kaski, Markus Heinonen, and Vikas Garg.*

1. **Learning to solve PDE-constrained inverse problems with graph networks.** ICML, 2022. [paper](https://openreview.net/pdf?id=cLR6FCyMY5k)

   *Zhao Qingqing, David B. Lindell, and Gordon Wetzstein.*

1. **Physics-embedded neural networks: E(n)-equivariant graph neural PDE solvers.** NIPS, 2022. [paper](https://openreview.net/pdf/e2112b7c6c9f008200054c5e466671c1d571aa74.pdf)

   *Masanobu Horie and  Naoto Mitsume.*

1. **PDE-GCN: Novel architectures for graph neural networks motivated by partial differential equations.** ICLR, 2021. [paper](https://openreview.net/forum?id=wWtk6GxJB2x)

   *Moshe Eliasof, Eldad Haber, and Eran Treister.*

1. **Physics-aware difference graph networks for sparsely-observed dynamics.** ICLR, 2020. [paper](https://openreview.net/forum?id=r1gelyrtwH)

   *Sungyong Seo, Chuizheng Meng, and Yan Liu.*

1. **Combining differentiable PDE solvers and graph neural networks for fluid flow prediction.** ICML, 2022. [paper](https://dl.acm.org/doi/10.5555/3524938.3525162)

   *Filipe de Avila Belbute-Peres, Thomas D. Economon, and J. Zico Kolter.*

1. **Learning continuous-time PDEs from sparse data with graph neural networks.** ICLR, 2021. [paper](https://openreview.net/pdf?id=aUX5Plaq7Oy)

   *Valerii Iakovlev, Markus Heinonen, and Harri Lähdesmäki.*

1. **Learning to simulate complex physics with graph networks.** ICML, 2020. [paper](https://dl.acm.org/doi/10.5555/3524938.3525722)

   *Alvaro Sanchez-Gonzalez, Jonathan Godwin, Tobias Pfaff, Rex Ying, Jure Leskovec, and Peter W. Battaglia.*

1. **GRAND: Graph neural diffusion.** ICML, 2021. [paper](https://openreview.net/forum?id=_1fu_cjsaRE)

   *Benjamin Paul Chamberlain, James Rowbottom, Maria I. Gorinova, Stefan D Webb, Emanuele Rossi, and Michael M. Bronstein.*

1. **GRAND++: Graph neural diffusion with a source term.** ICML, 2022. [paper](https://openreview.net/forum?id=EMxu-dzvJk)

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.*

1. **Physics-constrained unsupervised learning of partial differential equations using meshes.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.16628)

   *Mike Y. Michelis and Robert K. Katzschmann.*

2. **Neural PDE solvers for irregular domains.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.03241)

   *Biswajit Khara, Ethan Herron, Zhanhong Jiang, Aditya Balu, Chih-Hsuan Yang, Kumar Saurabh, Anushrut Jignasu, Soumik Sarkar, Chinmay Hegde, Adarsh Krishnamurthy, and Baskar Ganapathysubramanian.*

1. **Learning time-dependent PDE solver using message passing graph neural networks.** arXiv, 2022. [paper](https://openreview.net/forum?id=oaKw-GmBZZ)

   *Pourya Pilva and Ahmad Zareei.*

1. **On the robustness of graph neural diffusion to topology perturbations.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.07754)

   *Yang Song, Qiyu Kang, Sijie Wang, Zhao Kai, and Wee Peng Tay.*

1. **STONet: A neural-operator-driven spatio-temporal network.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.08414)

   *Haitao Lin, Guojiang Zhao, Lirong Wu, and Stan Z. Li.*

1. **PhyGNNet: Solving spatiotemporal PDEs with physics-informed graph neural network.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.04319)

   *Longxiang Jiang, Liyuan Wang, Xinkun Chu, Yonghao Xiao, and Hao Zhang.*

1. **Differentiable physics-informed graph networks.** arXiv, 2019. [paper](https://arxiv.org/abs/1902.02950)

   *Sungyong Seo and Yan Liu.*

### [Green Function](#content)
1. **BI-GreenNet: Learning Green's functions by boundary integral network.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.13247)

   *Guochang Lin, Fukai Chen, Pipi Hu, Xiang Chen, Junqing Chen, Jun Wang, and Zuoqiang Shi.*

### [Finite Element & Volume](#content)
1. **Composing partial differential equations with physics-aware neural networks.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/karlbauer22a/karlbauer22a.pdf)

   *Matthias Karlbauer, Timothy Praditia, Sebastian Otte, Sergey Oladyshkin, and Wolfgang Nowak.*

1. **Learning the dynamics of physical systems from sparse observations with finite element networks.** ICLR, 2022. [paper](https://openreview.net/forum?id=HFmAukZ-k-2)

   *Marten Lienen and Stephan Günnemann.*

1. **Hybrid finite difference with the physics-informed neural network for solving PDE in complex geometries.** arXiv, 2022. [paper](https://arxiv.org/pdf/2202.07926.pdf)

   *Zixue Xiang, Wei Peng, Weien Zhou, and Wen Yao.*

1. **Amortized finite element analysis for fast PDE-constrained optimization.** ICML, 2020. [paper](https://proceedings.mlr.press/v119/xue20a.html)

   *Tianju Xue, Alex Beatson, Sigrid Adriaenssens, and Ryan Adams.*

### [Convolutional Filter](#content)
1. **PDE-Net: Learning PDEs from data.** ICML, 2018. [paper](https://proceedings.mlr.press/v80/long18a.html)

   *Zichao Long, Yiping Lu, Xianzhong Ma, and Bin Dong.*

1. **PDE-Net 2.0: Learning PDEs from data with a numeric-symbolic hybrid deep network.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119306308)

   *ZichaoLong, YipingLu, and  Bin Dong.*

1. **Physics-informed CNNs for super-resolution of sparse observations on dynamical systems.** NIPS, 2022. [paper](https://arxiv.org/abs/2210.17319)

   *Daniel Kelshaw, Georgios Rigas, and Luca Magri.*

1. **Deep convolutional Ritz  method: Parametric PDE surrogates without labeled data.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.04675)

   *Jan Niklas Fuhg, Arnav Karmarkar, Teeratorn Kadeethum, Hongkyu Yoon, and Nikolaos Bouklas.*

1. **SplineCNN: Fast geometric deep learning with continuous B-spline kernels.** CVPR, 2018. [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Fey_SplineCNN_Fast_Geometric_CVPR_2018_paper.pdf)

   *Matthias Fey, Jan Eric Lenssen, Frank Weichert, and Heinrich Muller.*

1. **Spline-PINN: Approaching PDEs without data using fast, physics-informed Hermite-Spline CNNs.** AAAI, 2019. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/20830/20589)

   *Nils Wandel, Michael Weinmann, Michael Neidlin, and Reinhard Klein.*

### [Other Operators](#content)

1. **Multiwavelet-based operator learning for differential equations.** NIPS, 2021. [paper](https://openreview.net/forum?id=LZDiWaC9CGL)

   *Gaurav Gupta, Xiongye Xiao, and Paul Bogdan.*

1. **Nonparametric learning of kernels in nonlocal operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.11006)

   *Fei Lu, Qingci An, and Yue Yu.*

1. **Spectral neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.10573)

   *V. Fanasko and  I. Oseledets.*

1. **NOMAD: Nonlinear manifold decoders for operator learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.03551)

   *Jacob H. Seidman, Georgios Kissas, Paris Perdikaris, and George J. Pappas.*

1. **U-NO: U-shaped neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.11127)

   *Md Ashiqur Rahman, Zachary E. Ross, and Kamyar Azizzadenesheli.*

1. **Wavelet neural operator: A neural operator for parametric partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.02191)

   *Tapas Tripura and Souvik Chakraborty.*

1. **Pseudo-differential integral operator for learning solution operators of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2201.11967)

*Jin Young Shin, Jae Yong Lee, and Hyung Ju Hwang.*

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

1. **Robust discovery of partial differential equations in complex situations.** Physical Review Research, 2021. [paper](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.033270)

   *Hao Xu and Dongxiao Zhang.*

1. **Modeling the dynamics of PDE systems with physics-constrained deep auto-regressive networks.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307612)

   *Nicholas Geneva and Nicholas Zabaras.*

1. **Neural operator with regularity structure for modeling dynamics driven by SPDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.06255)

   *Peiyan Hu, Qi Meng, Bingguang Chen, Shiqi Gong, Yue Wang, Wei Chen, Rongchan Zhu, Zhi-Ming Ma, and Tie-Yan Liu.*

1. **Predicting parametric spatiotemporal dynamics by multi-resolution PDE structure-preserved deep learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.03990)

   *Xin-Yang Liu, Hao Sun, and Jian-Xun Wang.*

1. **Data-driven modeling of Landau damping by physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.01021)

   *Yilan Qin, Jiayu Ma, Mingle Jiang, Chuanfei Dong, Haiyang Fu, Liang Wang, Wenjie Cheng, and Yaqiu Jin.*

### [Machine Learning](#content)
1. **Machine learning–accelerated computational fluid dynamics.** Proceedings of the National Academy of Sciences, 2021. [paper](https://www.pnas.org/doi/10.1073/pnas.2101784118)

   *Dmitrii Kochkov,  Jamie A. Smith, Ayya Alieva, and Stephan Hoyer.*

1. **Solving high-dimensional partial differential equations using deep learning.** Proceedings of the National Academy of Sciences, 2018. [paper](https://www.pnas.org/doi/10.1073/pnas.1718942115)

   *Jiequn Han, Arnulf Jentzen, and Weinan E.*

1. **Solving high-dimensional parabolic PDEs using the tensor train format.** ICML, 2021. [paper](https://arxiv.org/abs/2102.11830)

   *Lorenz Richter, Leon Sallandt, and Nikolas Nüsken.*

1. **Nonlocal kernel network (NKN): A stable and resolution-independent deep neural network.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122005988)

   *HuaiqianYou, Yue Yu, Marta D'Elia, Tian Gao, Stewart Silling.*

1. **GCN-FFNN: A two-stream deep model for learning solution to partial differential equations.** Neurocomputing, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0925231222011511?dgcid=rss_sd_all)

   *Onur Bilgin, Thomas Vergutz, Siamak Mehrkanoon.*

1. **Deep-HyROMnet: A deep learning-based operator approximation for hyper-reduction of nonlinear parametrized PDEs.** Journal of Scientific Computing, 2021. [paper](https://link.springer.com/article/10.1007/s10915-022-02001-8)

   *Ludovica Cicci, Stefania Fresca, and Andrea Manzoni.*

1. **Solving PDEs on unknown manifolds with machine learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2106.06682)

   *Senwei Liang, Shixiao W. Jiang, John Harlim, and Haizhao Yang.*

1. **Model reduction and neural networks for parametric PDEs.** SMAI Journal of Computational Mathematics, 2021. [paper](https://smai-jcm.centre-mersenne.org/item/SMAI-JCM_2021__7__121_0/)

   *Kaushik Bhattacharya, Bamdad Hosseini, Nikola B. Kovachki, and Andrew M. Stuart.*

1. **MOD-Net: A machine learning approach via model-operator-data network for solving PDEs.** Communications in Computational Physics, 2022. [paper](https://global-sci.org/intro/article_detail/cicp/20860.html#)

   *Shamsulhaq Basir and Inanc Senocak.*

### [ODE](#content)
1. **On robustness of neural ordinary differential equations.** ICLR, 2020. [paper](https://openreview.net/forum?id=-gBckR-V1i)

   *Hanshu Yan, Jiawei Du, Vincent Y. F. Tan, and Jiashi Feng.*

1. **Beyond finite layer neural networks: Bridging deep architectures and numerical differential equations.** ICML, 2018. [paper](https://arxiv.org/abs/1710.10121)

   *Yiping Lu, Aoxiao Zhong, Quanzheng Li, and Bin Dong.*

1. **Neural ordinary differential equations.** NIPS, 2018. [paper](https://proceedings.neurips.cc/paper/2018/hash/69386f6bb1dfed68692a24c8686939b9-Abstract.html)

   *Ricky T. Q. Chen, Yulia Rubanova, Jesse Bettencourt, and David K. Duvenaud.*

1. **Hamiltonian neural networks.** ICML, 2018. [paper](https://proceedings.neurips.cc/paper/2019/file/26cd8ecadce0d4efd6cc8a8725cbd1f8-Paper.pdf)

   *Sam Greydanus, Misko Dzamba, and Jason Yosinski.*

1. **Deep learning for universal linear embeddings of nonlinear dynamics.** Nature Communications, 2018. [paper](https://www.nature.com/articles/s41467-018-07210-0)

   *Bethany Lusch, J. Nathan Kutz, and Steven L. Brunton.*

1. **Stochastic physics-informed neural ordinary differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2109.01621)

   *Jared O'Leary, Joel A. Paulson, and Ali Mesbah.*

## [Mechanism](#content) 
### [Library](#content)
1. **PDEBench: An extensive benchmark for scientific machine learning.** NIPS, 2022. [paper](https://openreview.net/forum?id=dh_MkX0QfrK)

   *Makoto Takamoto, Timothy Praditia, Raphael Leiteritz, Dan MacKinlay, Francesco Alesiani, and Dirk Pflüger, Mathias Niepert.*

1. **DeepXDE: A deep learning library for solving differential equations.** SIAM Review, 2021. [paper](https://epubs.siam.org/doi/abs/10.1137/19M1274067)

   *Lu Lu, Xuhui Meng, Zhiping Mao, and George Em Karniadakis.*

1. **A research framework for writing differentiable PDE discretizations in JAX.** NIPS, 2021. [paper](https://arxiv.org/abs/2111.05218)

   *Antonio Stanziola, Simon R. Arridge, Ben T. Cox,and Bradley E. Treeby.* 

1. **NVIDIA SimNet™: An AI-accelerated multi-physics simulation framework.** International Conference on Computational Science, 2021. [paper](https://link.springer.com/chapter/10.1007/978-3-030-77977-1_36)

   *Oliver Hennigh, Susheela Narasimhan, Mohammad Amin Nabian, Akshay Subramaniam, Kaustubh Tangsali, Zhiwei Fang, Max Rietmann, Wonmin Byeon, and Sanjay Choudhry.*

### [Analysis](#content)
1. **DPM: Physics-informed Karhunen-Loéve and neural network approximations for solving inverse differential equation problems.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16992/16799)

   *Jungeun Kim, Kookjin Lee, Dongeun Lee, Sheo Yon Jin, and Noseong Park.*

1. **Characterizing possible failure modes in physics-informed neural networks.** NIPS, 2021. [paper](https://openreview.net/forum?id=a2Gr9gNFD-J)

   *Aditi Krishnapriyan, Aditi_Krishnapriyan, Amir Gholami, Shandian Zhe, Robert Kirby, Michael W. Mahoney.*

1. **Understanding and mitigating gradient flow pathologies in physics-informed neural networks.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/20M1318043)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **When and why PINNs fail to train: A neural tangent kernel perspective.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100663X)

   *SifanWang, XinlingYu, and ParisPerdikaris.*

1. **When do extended physics-informed neural networks (XPINNs) improve generalization?** SIAM Journal on Scientific Computing, 2022. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1447039)

   *Zheyuan Hu, Ameya D. Jagtap, George Em Karniadakis, and Kenji Kawaguchi.*

1. **Respecting causality is all you need for training physics-informed neural networks.** arXiv, 2021. [paper](https://arxiv.org/abs/2203.07404)

   *Sifan Wang, Shyam Sankaran, and Paris Perdikaris.*

1. **Understanding the difficulty of training physics-informed neural networks on dynamical systems.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.13648)

   *Franz M. Rohrhofer, Stefan Posch, Clemens Gößnitzer, and Bernhard C. Geiger.*

1. **Mitigating learning complexity in physics and equality constrained artificial neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01807)

   *Victor Churchill and Dongbin Xiu.*

1. **Improved training of physics-informed neural networks with model ensembles.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.05108)

   *Katsiaryna Haitsiukevich and Alexander Ilin.*
   
1. **The cost-accuracy trade-off in operator learning with neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.13181)
   
   *Maarten V. de Hoop, Daniel Zhengyu Huang, Elizabeth Qian,amd  Andrew M. Stuart.*

### [Attention](#content)
1. **Learning operators with coupled attention.** Journal of Machine Learning Research, 2022. [paper](https://www.jmlr.org/papers/v23/21-1521.html) 

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.* 

1. **Choose a Transformer: Fourier or Galerkin.** NIPS, 2021. [paper](https://openreview.net/forum?id=ssohLcmn4-r)

   *Shuhao Cao.* 

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR, 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP) 

   *Xu Han, Han Gao, Tobias Pfaff, Jian-Xun Wang, and Liping Liu.*

1. **SiT: Simulation transformer for particle-based physics simulation.** ICLR, 2022. [paper](https://openreview.net/forum?id=DBOibe1ISzB) 

   *Yidi Shao, Chen Change Loy, and Bo Dai.*

1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS, 2021. [paper](https://arxiv.org/abs/2009.04544) 

   *Levi D. McClenny and Ulisses Braga-Neto.*

1. **Transformer for partial differential equations' operator learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.13671) 

   *Zijie Li, Kazem Meidani, and Amir Barati Farimani.*

1. **Physics-informed attention-based neural network for hyperbolic partial differential equations: Application to the Buckley–Leverett problem.**  Scientific Reports, 2022. [paper](https://www.nature.com/articles/s41598-022-11058-2) 

   *Ruben Rodriguez-Torrado, Pablo Ruiz, Luis Cueto-Felgueroso, Michael Cerny Green, Tyler Friesen, Sebastien Matringe,and Julian Togelius .*

1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS, 2021. [paper](https://github.com/levimcclenny/SA-PINNs) 

   *Levi McClenny and Ulisses Braga-Neto.*

### [Neural Implicit Flow](#content)
1. **Neural implicit flow: A mesh-agnostic dimensionality reduction paradigm of spatio-temporal data.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.03216) 

   *Shaowu Pan, Steven L. Brunton, and J. Nathan Kutz.*

1. **CROM: Continuous reduced-order modeling of PDEs using implicit neural representations.** ICLR , 2023. [paper](https://openreview.net/forum?id=FUORz1tG8Og) 

   *Peter Yichen Chen, Jinxu Xiang, Dong Heon Cho, Yue Chang, G A Pershing, Henrique Teles Maia, Maurizio Chiaramonte, Kevin Carlberg, and Eitan Grinspun.*

### [Disentangle](#content)
1. **PDE-driven spatiotemporal disentanglement.** ICLR , 2021. [paper](https://openreview.net/forum?id=vLaHRtHvfFp)

   *Jérémie Donà, Jean-Yves Franceschi, Sylvain Lamprier, and Patrick Gallinari.*

### [Meta Learning](#content)
1. **Meta-auto-decoder for solving parametric partial differential equations.** NIPS, 2022. [paper](https://openreview.net/pdf?id=PwlW5Jri1Xt) 

   *Xiang Huang, Zhanhong Ye, Hongsheng Liu, Beiji Shi, Zidong Wang, Kang Yang, Yang Li, Bingya Weng, Min Wang, Haotian Chu, Jing Zhou, Fan Yu, Bei Hua, Lei Chen, and Bin Dong.*

1. **Transfer learning with physics-informed neural networks for efficient simulation of branched flows.** NIPS, 2022. [paper](https://arxiv.org/abs/2211.00214) 

   *Raphaël Pellegrin, Blake Bullwinkel, Marios Mattheakis, and Pavlos Protopapas.*

1. **Identifying physical law of hamiltonian systems via meta-learning.** ICLR, 2021. [paper](https://openreview.net/pdf?id=45NZvF1UHam) 

   *Seungjun Lee, Haesang Yang, and Woojae Seong.*

1. **One-shot learning for solution operators of partial differential equations.** ICLR, 2021. [paper](https://arxiv.org/abs/2104.05512) 

   *Lu Lu, Haiyang He, Priya Kasimbeg, Rishikesh Ranade, and Jay Pathak.*

1. **Meta-MgNet: Meta multigrid networks for solving parameterized partial differential equations.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122000584)

   *Yuyan Chen, Bin Dong, and JinchaoXu.*

1. **Meta-learning PINN loss functions.** Journal of Computational Physics, 2022.  [paper](https://www.sciencedirect.com/science/article/pii/S0021999122001838)

   *Apostolos F Psaros,Kenji Kawaguchi, and George Em Karniadakis.*

1. **HyperPINN: Learning parameterized differential equations with physics-informed hypernetworks.** NIPS, 2021. [paper](https://openreview.net/pdf?id=LxUuRDUhRjM)

   *Filipe de Avila Belbute-Peres, Yi-fan Chen, and Fei Sha.*
   
1. **Physics-informed neural networks (PINNs) for parameterized PDEs: A meta-learning approach.** arXiv,. 2021. [paper](https://arxiv.org/abs/2110.13361)

   *Michael Penwarden, Shandian Zhe, Akil Narayan, and Robert M. Kirby.*

1. **Auto-PINN: Understanding and optimizing physics-informed neural architecture.** arXiv,. 2022. [paper](https://arxiv.org/abs/2110.13361)

   *Yicheng Wang, Xiaotian Han, Chia-Yuan Chang, Daochen Zha, Ulisses Braga-Neto, and Xia Hu.*

1. **Transfer learning based physics-informed neural networks for solving inverse problems in engineering structures under different loading scenarios.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.07731)

   *Chen Xu, Ba Trung Cao, Yong Yuan, and Günther Meschke.*

### [Latent Space](#content)
1. **A Latent space solver for PDE generalization.** ICLR, 2021. [paper](https://arxiv.org/abs/2104.02452)

   *Rishikesh Ranade, Chris Hill, Haiyang He, Amir Maleki, and Jay Pathak.*

1. **Approximate latent force model inference.** AAAI, 2021. [paper](https://ml4physicalsciences.github.io/2021/files/NeurIPS_ML4PS_2021_78.pdf)

   *Jacob D. Moss, Felix L. Opolka, Bianca Dumitrascu, and Pietro Lió.*

1. **Learning to accelerate partial differential equations via latent global evolution.** NIPS, 2022. [paper](https://arxiv.org/abs/2206.07681)

   *Tailin Wu, Takashi Maruyama, and Jure Leskovec.*

### [Loss Function](#content)
1. **Adaptive activation functions accelerate convergence in deep and physics-informed neural networks.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119308411)

   *Ameya D.Jagtap, KenjiKawaguchi, and George EmKarniadakis.*

1. **Adaptive deep neural networks methods for high-dimensional partial differential equations.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122002947#)

   *Shaojie Zeng, Zong Zhang, and Qingsong Zou.*

1. **Self-adaptive loss balanced Physics-informed neural networks.** Neurocomputing, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S092523122200546X)

   *Zixue Xiang, Wei Peng, Xu Liu, and Wen Yao.*

1. **Multi-objective loss balancing for physics-informed deep learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.09813)

   *Rafael Bischof, and Michael Kraus.*

1. **Self-scalable Tanh (Stan): Faster convergence and better generalization in physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.12589)

   *Raghav Gnanasambandam, Bo Shen, Jihoon Chung, Xubo Yue, and Zhenyu (James) Kong.*

1. **Is L2 physics-informed loss always suitable for training physics-informed neural network?** arXiv, 2022. [paper](https://arxiv.org/abs/2206.02016)

   *Chuwei Wang, Shanda Li, Di He, and Liwei Wang.*

1. **Self-scalable Tanh (Stan): Faster convergence and better generalization in physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.12589)

   *Raghav Gnanasambandam, Bo Shen, Jihoon Chung, Xubo Yue, and Zhenyu (James) Kong.*

1. **Loss landscape engineering via data regulation on PINNs.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.07843)

   *Vignesh Gopakumar, Stanislas Pamela, and Debasmita Samaddar.*

### [Decomposition](#content)
1. **Composing partial differential equations with physics-aware neural networks.** ICLR, 2022. [paper](https://openreview.net/forum?id=DIsWHvtU7lF)

   *Matthias Karlbauer, Timothy Praditia, Sebastian Otte, Sergey Oladyshkin, Wolfgang Nowak, and Martin V. Butz.*

1. **Learning composable energy surrogates for PDE order reduction.** NIPS, 2020. [paper](https://proceedings.neurips.cc/paper/2020/file/0332d694daab22e0e0eaf7a5e88433f9-Paper.pdf)

   *Alex Beatson, Jordan T. Ash, Geoffrey Roeder, Tianju Xue, and Ryan P. Adams.*

1. **PFNN-2: A domain decomposed penalty-free neural network method for solving partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.00593)

   *Hailong Shen and Chao Yang.*

1. **Finite Basis Physics-Informed Neural networks (FBPINNs): A scalable domain decomposition approach for solving differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2107.07871)

   *Ben Moseley, Andrew Markham, and Tarje Nissen-Meyer.*

1. **Finite basis physics-informed neural networks as a Schwarz domain decomposition method.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.05560)

   *Victorita Dolean, Alexander Heinlein, Siddhartha Mishra, and Ben Moseley.*

1. **NeuralStagger: Accelerating physics constrained neural PDE solver with spatialtemporal decomposition.** ICLR, 2023. [paper](https://openreview.net/forum?id=pGR2gNO5c4p)

   *Anonymous authors.*

1. **Augmenting physical models with deep networksfor complex dynamics forecasting.** Journal of Statistical Mechanics: Theory and Experiment, 2021. [paper](https://iopscience.iop.org/article/10.1088/1742-5468/ac3ae5/meta)

   *Yuan Yin, Vincent Le Guen, Jérémie Dona, Emmanuel de Bézenac, Ibrahim Ayed, Nicolas Thome, and Patrick Gallinari.*

1. **LordNet: Learning to solve parametric partial differential equations without simulated data.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.09418)

   *Wenlei Shi, Xinquan Huang, Xiaotian Gao, Xinran Wei, Jia Zhang, Jiang Bian, Mao Yang, and Tie-Yan Liu.*

### [Mesh](#content)
1. **M2N: Mesh movement networks for PDE solvers.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.11188)

   *Wenbin Song, Mingrui Zhang, Joseph G. Wallwork, Junpeng Gao, Zheng Tian, Fanglei Sun, Matthew D. Piggott, Junqing Chen, Zuoqiang Shi, Xiang Chen, and Jun Wang.*

1. **RANG: A residual-based adaptive node generation method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.01051)

   *Wei Peng, Weien Zhou, Xiaoya Zhang, Wen Yao, and Zheliang Liu.*

1. **Learning a mesh motion technique with application to fluid-structure interaction and shape optimization.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.02217)

   *Johannes Haubne and, Miroslav Kuchta.*

1. **Accelerated training of physics-informed neural networks (PINNs) using meshless discretizations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.09332)

   *Ramansh Sharma and  Varun Shankar.*

1. **Mesh-free Eulerian physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01545)

   *Fabricio Arend Torres, Marcello Massimo Negri, Monika Nagy-Huber, Maxim Samarin, and Volker Roth.*

### [GAN](#content)
1. **A framework for data-driven solution and parameter estimation of PDEs using conditional generative adversarial networks.** Nature Computational Science, 2021. [paper](https://www.nature.com/articles/s43588-021-00171-3)

   *Teeratorn Kadeethum, Daniel O’Malley, Jan Niklas Fuhg, Youngsoo Choi, Jonghyun Lee, Hari S. Viswanathan, and Nikolaos Bouklas.*

1. **PID-GAN: A GAN framework based on a physics-informed discriminator for uncertainty quantification with physics.** KDD, 2021. [paper](https://dl.acm.org/doi/abs/10.1145/3447548.3467449)

   *Arka Daw, M. Maruf, and Anuj Karpatne.*

1. **Generative adversarial neural operators.** Transactions on Machine Learning Research, 2022. [paper](https://openreview.net/forum?id=X1VzbBU6xZ&referrer=%5BTMLR%5D(%2Fgroup%3Fid%3DTMLR))

   *Md Ashiqur Rahman, Manuel A Florez, Anima Anandkumar, Zachary E Ross, and Kamyar Azizzadenesheli.*

1. **Weak adversarial networks for high-dimensional partial differential equations.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120301832)

   *YaohuaZang, GangBao, XiaojingYe, and HaominZhou.*

1. **Wasserstein generative adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003321)

   *YihangGao and Michael K.Ng.*

1. **Competitive physics informed networks.** ICLR, 2021. [paper](https://openreview.net/forum?id=rMz_scJ6lc)

   *Qi Zeng, Spencer H Bryngelson, and Florian Tobias Schaefer.*

1. **Learning generative neural networks with physics knowledge.** Research in the Mathematical Sciences, 2022. [paper](https://link.springer.com/article/10.1007/s40687-022-00329-z)

   *Kailai Xu, Weiqiang Zhu, and Eric Darve.*

1. **Revisiting PINNs: Generative adversarial physics-informed neural networks and point-weighting method.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.08754)

   *Wensheng Li, Chao Zhang, Chuncheng Wang, Hanting Guan, and Dacheng Tao.*

### [Gaussian Process](#content)
1. **PAGP: A physics-assisted Gaussian process framework with active learning for forward and inverse problems of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.02583)

   *Jiahao Zhang, Shiqi Zhang, and Guang Lin.*

1. **Solving and learning nonlinear PDEs with Gaussian processes.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005635)

   *Yifan Chen, Bamdad Hosseini, Houman Owhadi, and Andrew M.Stuart.*

### [Solver](#content)
1. **Solver-in-the-loop: learning from differentiable physics to interact with iterative PDE-solvers.** NIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496237)

   *Kiwon Um, Robert Brand, Yun (Raymond) Fei, Philipp Holl, and Nils Thuerey.*
   
1. **Lie point symmetry data augmentation for neural PDE solvers.** ICML, 2022. [paper](https://arxiv.org/abs/2202.07643)

   *Johannes Brandstetter, Max Welling, and Daniel E. Worrall.*

1. **Incorporating symmetry into deep dynamics models for improved generalization.** ICLR, 2021. [paper](https://openreview.net/forum?id=wta_8Hx2KD)

   *Rui Wang, Robin Walters, and Rose Yu.*

1. **HyperSolvers: Toward fast continuous-depth models.** NIPS, 2020. [paper](http://www.robot.t.u-tokyo.ac.jp/~yamashita/paper/B/B268Final.pdf)

   *Michael Poli, Stefano Massaroli, Atsushi Yamashita, Hajime Asama, and Jinkyoo Park.*

### [Variations](#content) 
1. **PI-VAE: Physics-Informed Variational Auto-Encoder for stochastic differential equations.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522006193)

   *Weiheng Zhong, Hadi Meidani.*

1. **hp-VPINNs: Variational physics-informed neural networks with domain decomposition.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520307325)

   *Ehsan Kharazmi, Zhongqiang Zhang, and George E.M.Karniadakis.*

1. **Variational Onsager Neural Networks (VONNs): A thermodynamics-based variational learning strategy for non-equilibrium PDEs.** Journal of the Mechanics and Physics of Solids, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0022509622000692)

   *Shenglin Huang, Zequn He, Bryan Chem, Celia Reina.*

1. **Solving PDEs by variational physics-informed neural networks: An a posteriori error analysis.** ANNALI DELL'UNIVERSITA' DI FERRARA, 2022. [paper](https://link.springer.com/article/10.1007/s11565-022-00441-6)

   *Stefano Berrone, Claudio Canuto, and Moreno Pintore.*

1. **Variational Monte Carlo approach to partial differential equations with neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01927)

   *Moritz Reh and Martin Gärttner.*

1. **Variational Bayes deep operator network: A data-driven Bayesian solver for parametric differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.05655)

   *Shailesh Garg and Souvik Chakraborty.*

### [Bayesian](#content)
1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, and George Em Karniadakis.*

1. **Solving inverse problems in stochastic models using deep neural networks and adversarial training.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521003078)

   *Kailai Xu, and EricDarve.*

1. **Bayesian deep learning for partial differential equation parameter discovery with sparse and noisy data.** Journal of Computational Physics: X, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S2590055222000117?via%3Dihub)

   *ChristopheBonneville, and ChristopherEarls.*

1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, George EmKarniadakis.*

1. **Approximate Bayesian neural operators: Uncertainty quantification for parametric PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.01565)

   *Emilia Magnani, Nicholas Krämer, Runa Eschenhagen, Lorenzo Rosasco, and Philipp Hennig.*

### [Lagrangian](#content)
1. **Lagrangian PINNs: A causality–conforming solution to failure modes of physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.02902)

   *Rambod Mojgani, Maciej Balajewicz, and Pedram Hassanzadeh.*

1. **AL-PINNs: Augmented Lagrangian relaxation method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.01059)

   *Hwijae Son, Sung Woong Cho, and Hyung Ju Hwang.*

### [Uncertainty Quantification](#content)
1. **Quantifying total uncertainty in physics-informed neural networks for solving forward and inverse stochastic problems.** arXiv, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119305340)

   *Dongkun Zhang, Lu Lu, Ling Guo, and George EmKarniadakis.*

1. **Adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303584)

   *Yibo Yang and Paris Perdikaris.*

### [Active Learning](#content)
1. **Neural Galerkin scheme with active learning for high-dimensional evolution equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.01360)

   *Joan Bruna, Benjamin Peherstorfer, and Eric Vanden-Eijnden.*

1. **Discovering and forecasting extreme events via active learning in neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.02488)

   *Pickering, Ethan and Karniadakis, George Em and Sapsis, and Themistoklis P.*

### [Multi-Scale](#content)
1. **Hierarchical deep learning of multiscale differential equation time-steppers.** Philosophical Transactions of the Royal Society A, 2022. [paper](https://royalsocietypublishing.org/doi/10.1098/rsta.2021.0200)

   *Yuying Liu, J. Nathan Kutz, and Steven L. Brunton.*

1. **NH-PINN: Neural homogenization-based physics-informed neural network for multiscale problems.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122006015)

   *Wing Tat Leung, Guang Lin, and Zecheng Zhang.*

1. **Multi-scale deep neural networks for solving high dimensional PDEs.** arXiv, 2019. [paper](https://www.science.org/doi/10.1126/sciadv.1602614)

   *Samuel H. Rudy, Steven L. Brunton,  Joshua L. Proctor, and  J. Nathan Kutz.*

### [Multi-Fidelity](#content)
1. **Multifidelity deep operator networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.09157)

   *Amanda A. Howard, Mauro Perego, George E. Karniadakis, and Panos Stinis.*

1. **Physics and equality constrained artificial neural networks: Application to forward and inverse problems with multi-fidelity data fusion.** Journal of Computational Physics, 2022. [paper](https://dl.acm.org/doi/abs/10.1016/j.jcp.2022.111301)

   *Lulu Zhang, Tao Luo, Yaoyu Zhang, Weinan E, Zhi-Qin John Xu, and Zheng Ma.*

1. **Multifidelity deep neural operators for efficient learning of partial differential equations with application to fast inverse design of nanoscale heat transport.** Physical Review Research, 2022. [paper](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.4.023210)

   *Lu Lu, Raphaël Pestourie, Steven G. Johnson, and Giuseppe Romano.*

### [Multi-Grid](#content)

1. **Learning to optimize multigrid PDE solvers.** ICML, 2019. [paper](http://proceedings.mlr.press/v97/greenfeld19a.html)

   *Daniel Greenfeld, Meirav Galun, Ronen Basri, Irad Yavneh, and Ron Kimmel.*


## [Applications](#content)
### [Optimal Control](#content)
1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*

1. **An extended physics informed neural network for preliminary analysis of parametric optimal control problems.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13530)

   *Nicola Demo, Maria Strazzullo, and Gianluigi Rozza.*

1. **Optimal control of PDEs using physics-informed neural networks.** ICLR, 2022. [paper](https://openreview.net/forum?id=a3Rhl617hW)

   *Saviz Mowlavi and Saleh Nabi.*

1. **Solving PDE-constrained control problems using operator learning.** AAAI, 2022. [paper](https://aaai-2022.virtualchair.net/poster_aaai12978)

   *Rakhoon Hwang, Jae Yong Lee, Jin Young Shin, and Hyung Ju Hwang.*

1. **PDE-based optimal strategy for unconstrained online learning.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22d.html)

   *Zhiyu Zhang, Ashok Cutkosky,and  Ioannis Paschalidis.*

1. **Neural solvers for fast and accurate numerical optimal control.** NIPS, 2021. [paper](https://openreview.net/forum?id=rwMWDGOjaQF)

   *Federico Berto, Stefano Massaroli, Michael Poli, and  Jinkyoo Park.*

1. **Control of partial differential equations via physics-informed neural networks.** Journal of Optimization Theory and Applications, 2022. [paper](https://link.springer.com/article/10.1007/s10957-022-02100-4)

   *Carlos J. García-Cervera, Mathieu Kessler, and Francisco Periago.*

1. **Bi-level physics-informed neural networks for pde constrained optimization using Broyden's hypergradients.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.07075)

   *Zhongkai Hao, Chengyang Ying, Hang Su, Jun Zhu, Jian Song, and Ze Cheng.*

### [Fuild](#content)
1. **DeepONet prediction of linear instability waves in high-speed boundary layers.** arXiv, 2021. [paper](https://arxiv.org/abs/2105.08697)

   *Patricio Clark Di Leoni, Lu Lu, Charles Meneveau, George Karniadakis, and Tamer A. Zaki.*

1. **Towards physics-informed deep learning for turbulent flow prediction.** KDD, 2020. [paper](https://dl.acm.org/doi/10.1145/3394486.3403198)

   *Rui Wang, Karthik Kashinath, Mustafa Mustafa, Adrian Albert, Rose Yu.*

1. **Learning to estimate and refine fluid motion with physical dynamics.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22ad/zhang22ad.pdf)

   *Mingrui Zhang, Jianhong Wang, James Tlhomole, and Matthew D. Piggott.*

1. **Physics informed neural fields for smoke reconstruction with sparse data.** ACM Transactions on Graphics, 2022. [paper](https://dl.acm.org/doi/10.1145/3528223.3530169)

   *Mengyu Chu, Lingjie Liu, Quan Zheng, Erik Franz, Hans-Peter Seidel, Christian Theobalt, andRhaleb Zayer.*

### [Reconstruction](#content)
1. **Occupancy networks: Learning 3D reconstruction in function space.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mescheder_Occupancy_Networks_Learning_3D_Reconstruction_in_Function_Space_CVPR_2019_paper.pdf)

   *Lars Mescheder, Michael Oechsle, Michael Niemeyer, Sebastian Nowozin, and Andreas Geiger.*

### [Physics](#content)
1. **FourCastNet: A global data-driven high-resolution weather model using adaptive fourier neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.11214)

   *Jaideep Pathak, Shashank Subramanian, Peter Harrington, Sanjeev Raja, Ashesh Chattopadhyay, Morteza Mardani, Thorsten Kurth, David Hall, Zongyi Li, Kamyar Azizzadenesheli, Pedram Hassanzadeh, Karthik Kashinath, and Animashree Anandkumar.*

1. **Learning two-phase microstructure evolution using neural operators and autoencoder architectures.**  NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00876-7)

   *Vivek Oommen, Khemraj Shukla, Somdatta Goswami, Rémi Dingreville, and George Em Karniadakis.*

### [Image](#content)
1. **Learning to diffuse: A new perspective to design PDEs for visual analysis.** TPAMI, 2016. [paper](https://ieeexplore.ieee.org/document/7393839)

   *Liu, Risheng, Zhong, Guangyu, Cao, Junjie, Lin, Zhouchen, Shan, Shiguang, and Luo, Zhongxuan.*

1. **Reformulating optical flow to solve image-based inverse problems and quantify uncertainty.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9870569)

   *Aleix Boquet-Pujadas and Jean-Christophe Olivo-Marin.*

### [Manufacturing](#content)
1. **Physics-aware machine learning surrogates for real-time manufacturing digital twin.** Manufacturing Letters, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S2213846322001845)

   *Aditya Balu,Soumik Sarkar, Baskar Ganapathysubramanian, and Adarsh Krishnamurthy.*