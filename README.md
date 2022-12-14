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
    <td>&ensp;<a href="#graph-network">2.4 Graph Network</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#green-function">2.5 Green Function</a></td>
    <td>&ensp;<a href="#finite-element">2.6 Finite Element</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#convolutional-filter">2.7 Convolutional Filter</a></td>
    <td>&ensp;<a href="#autoencoder">2.8 AutoEncoder</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#operator">2.9 Operator</a></td>
    <td>&ensp;<a href="#identification">2.10 Identification</a></td>
<tr>
    <td>&ensp;<a href="#machine-learning">2.11 Machine Learning</a></td>
    <td>&ensp;<a href="#ode">2.12 ODE</a></td>
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
    <td>&ensp;<a href="#nas">3.7 NAS</a></td>
    <td>&ensp;<a href="#sampling">3.8 Sampling</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#latent-space">3.9 Latent Space</a></td>
    <td>&ensp;<a href="#loss-function">3.10 Loss Function</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#decomposition">3.11 Decomposition</a></td>
    <td>&ensp;<a href="#mesh">3.12 Mesh</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#generative-models">3.13 Generative Models</a></td>
    <td>&ensp;<a href="#gaussian-process">3.14 Gaussian Process</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#solver">3.15 Solver</a></td>
    <td>&ensp;<a href="#variation">3.16 Variation</a></td>
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
    <td>&ensp;<a href="#multi-scale">3.22 Multi Scale</a></td>
</tr>
 <tr>
    <td>&ensp;<a href="#multi-fidelity">3.23 Multi Fidelity</a></td>
    <td>&ensp;<a href="#multi-grid">3.24 Multi Grid</a></td>
</tr>
<tr><td colspan="2"><a href="#applications">4. Applications</a></td></tr> 
<tr>
    <td>&ensp;<a href="#optimization">4.1 Optimization</a></td>
    <td>&ensp;<a href="#fluid">4.2 Fluid</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#reconstruction">4.3 Reconstruction</a></td>
    <td>&ensp;<a href="#physics">4.4 Physics</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#image">4.5 Image</a></td>
    <td>&ensp;<a href="#mechanics">4.6 Mechanics</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#robotics">4.7 Robotics</a></td>
    <td>&ensp;<a href="#cybernetics">4.8 Cybernetics</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#quantum">4.9 Quantum</a></td>
    <td>&ensp;<a href="#nash-equilibrial">4.10 Nash Equilibrial</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#manufacturing">4.11 Manufacturing</a></td>
    <td>&ensp;<a href="#"></a></td>
</tr> 
</table>








## [Survey Papers](#content)
1. **Physics-informed machine learning.** Nature Reviews Physics, 2021. [paper](https://www.nature.com/articles/s42254-021-00314-5)

   *George Em Karniadakis, Ioannis G. Kevrekidis, Lu Lu, Paris Perdikaris, Sifan Wang, and Liu Yang.*

1. **Neural operator: Learning maps between function spaces.** arXiv, 2021. [paper](https://arxiv.org/abs/2108.08481)

   *Nikola Kovachki, Zongyi Li, Burigede Liu, Kamyar Azizzadenesheli, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Physics-informed machine learning approach for augmenting turbulence models: A comprehensive framework.** Physical Review Fluids, 2018. [paper](https://journals.aps.org/prfluids/abstract/10.1103/PhysRevFluids.3.074602)

   *Jin-Long Wu, Heng Xiao, and Eric Paterson.* 

1. **Integrating scientific knowledge with machine learning for engineering and environmental systems.** ACM Computing Surveys, 2023. [paper](https://dl.acm.org/doi/full/10.1145/3514228)

   *Jared Willard, Xiaowei Jia, Shaoming Xu, Michael Steinbach, and Vipin Kumar.* 

1. **Physical laws meet machine intelligence: Current developments and future directions.** Artificial Intelligence Review, 2022. [paper](https://link.springer.com/article/10.1007/s10462-022-10329-8)

   *Temoor Muther, Amirmasoud Kalantari Dahaghi, Fahad Iqbal Syed, and Vuong Van Pham.* 

1. **A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001207?via%3Dihub)

   *Lu Lu, Xuhui Meng, Shengze Cai, Zhiping Mao, Somdatta Goswami, Zhongqiang Zhang, and George Em Karniadakis.* 

1. **Scientific machine learning through physics–informed neural networks: Where we are and what’s next.** Beyond traditional AI: the impact of Machine Learning on Scientific Computing, 2022. [book](https://link.springer.com/article/10.1007/s10915-022-01939-z)

   *MingyuanYang and John T.Foster*

1. **When physics meets machine learning: A survey of physics-informed machine learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.16797)

   *Chuizheng Meng, Sungyong Seo, Defu Cao, Sam Griesemer, and Yan Liu.* 

1. **Physics-guided, physics-informed, and physics-encoded neural networks in scientific computing.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.07377)

   *Salah A. Faroughi, Nikhil M. Pawar, C´elio Fernandes, Subasish Das, Nima K. Kalantari, and Seyed Kourosh Mahjour.* 
   
1. **Physics-informed machine learning: A survey on problems, methods and applications.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.08064)

   *Zhongkai Hao, Songming Liu, Yichi Zhang, Chengyang Ying, Yao Feng, Hang Su, and Jun Zhu.* 

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

   *Raissi Maziar, Alireza Yazdani, and George Em Karniadakis.*

1. **Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999118307125)

   *M.Raissia, P.Perdikarisb, and George Em Karniadakis.*

1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** JMLR, 2018. [paper](https://www.jmlr.org/papers/volume19/18-046/18-046.pdf)

   *Maziar Raissi.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/21M1397908)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **A universal PINNs method for solving partial differential equations with a point source.** IJCAI, 2022. [paper](https://www.ijcai.org/proceedings/2022/533)

   *Xiang Huang, Hongsheng Liu, Beiji Shi, Zidong Wang, Kang Yang, Yang Li, Min Wang, Haotian Chu, Jing Zhou, Fan Yu, Bei Hua, Bin Dong, and Lei Chen.*
   
1. **Parallel physics-informed neural networks via domain decomposition.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005787)

   *Khemraj Shukla, Ameya D.Jagtap, and George Em Karniadakis.*

1. **Exact imposition of boundary conditions with distance functions in physics-informed deep neural networks.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521006186)

   *N.Sukumar and Ankit Srivastava.*

1. **Physics-informed multi-LSTM networks for meta-modeling of nonlinear structures.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520304114)

   *Ruiyang Zhang, Yang Liu, and Hao Sun.*

1. **Gradient-enhanced physics-informed neural networks for forward and inverse PDE problems.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001438?via%3Dihub)

   *Jeremy Yu, Lu Lu, Xuhui Meng, and George Em Karniadakis.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **PPINN: Parareal physics-informed neural network for time-dependent PDEs.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782520304357)

   *Xuhui Meng, Zhen Li, Dongkun Zhang, and George Em Karniadakis.*

1. **CAN-PINN: A fast physics-informed neural network based on coupled-automatic–numerical differentiation method.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522001906)

   *Pao-Hsiung Chiu, Jian Cheng Wong, Chinchun Ooi, My Ha Dao, and Yew-Soon Ong.*

1. **Derivative-informed projected neural networks for high-dimensional parametric maps governed by PDEs.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521005302)

   *Thomas O’Leary-Roseberry, Umberto Villa, Peng Chen, and Omar Ghattas.*

1. **Physics-augmented learning: A new paradigm beyond physics-informed learning.** NIPS, 2021. [paper](https://www.iamwawa.cn/daxiaoxie.html)

   *Ziming Liu, Yuanqi Du, Yunyue Chen, and Max Tegmark.*

1. **Data-driven vector soliton solutions of coupled nonlinear Schrödinger equation using a deep learning algorithm.** Physics Letters A, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0375960121006034)

   *Yifan Mo, Liming Ling, and Delu Zeng.*

1. **Solving Benjamin–Ono equation via gradient balanced PINNs approach.** The European Physical Journal Plus, 2022. [paper](https://link.springer.com/article/10.1140/epjp/s13360-022-03078-8)

   *Xiangyu Yang and Zhen Wang.*

1. **Robust learning of physics informed neural networks.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13330)

   *Chandrajit Bajaj, Luke McLennan, Timothy Andeen, and Avik Roy.*

1. **Learning physics-informed neural networks without stacked back-propagation.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.09340)

   *Di He, Wenlei Shi, Shanda Li, Xiaotian Gao, Jia Zhang, Jiang Bian, Liwei Wang, and Tieyan Liu.*

1. **NeuralPDE: Automating physics-informed neural networks (PINNs) with error approximations.** arXiv, 2021. [paper](https://arxiv.org/abs/2107.09443)

   *Kirill Zubov, Zoe McCarthy, Yingbo Ma, Francesco Calisto, Valerio Pagliarino, Simone Azeglio, Luca Bottero, Emmanuel Luján, Valentin Sulzer, Ashutosh Bharambe, Nand Vinchhi, Kaushik Balakrishnan, Devesh Upadhyay, and Chris Rackauckas.*

1. **Physics informed RNN-DCT networks for time-dependent partial differential equations.** ICCS, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-08754-7_45)

   *Benjamin Wu, Oliver Hennigh, Jan Kautz, Sanjay Choudhry, and Wonmin Byeon.*

1. **Physics-informed Karhunen-Loéve and neural network approximations for solving inverse differential equation problems.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122002923)

   *Jing Li and Alexandre M.Tartakovsky.*

1. **Theory-guided physics-informed neural networks for boundary layer problems with singular perturbation.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122008312)

   *Amirhossein Arzani, Kevin W.Cassel, and Roshan M.D'Souza.*

1. **A-PINN: Auxiliary physics informed neural networks for forward and inverse problems of nonlinear integro-differential equations.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003229)

   *Lei Yuan, Yi-Qing Ni, Xiang-Yun Deng, and Shuo Hao.*

1. **A mixed formulation for physics-informed neural networks as a potential solver for engineering problems in heterogeneous domains: Comparison with finite element method.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522005722)

   *Shahed Rezaei, Ali Harandi, Ahmad Moeineddin, Baixiang Xua, and Stefanie Reese.*

1. **A novel sequential method to train physics informed neural networks for Allen Cahn and Cahn Hilliard equations.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521006939)

   *Revanth Mattey and Susanta Ghosh.*

1. **RPINNs: Rectified-physics informed neural networks for solving stationary partial differential equations.** Computers and Fluids, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045793022001955)

   *Pai Peng, Jiangong Pan, Hui Xu, and Xinlong Feng.*
   
1. **A-WPINN algorithm for the data-driven vector-soliton solutions and parameter discovery of general coupled nonlinear equations.** Physica D: Nonlinear Phenomena, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0167278922002664)

   *Shumei Qin, Min Li, Tao Xu, and Shaoqun Dong.*

1. **Physics-informed neural networks with adaptive localized artificial viscosity.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.08802)

   *E.J.R. Coutinho, M. Dall'Aqua, L. McClenny, M. Zhong, U. Braga-Neto, and E. Gildin.*

1. **Physics-informed neural operator for learning partial differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2111.03794)

   *Zongyi Li, Hongkai Zheng, Nikola Kovachki, David Jin, Haoxuan Chen, Burigede Liu, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Anisotropic, sparse and interpretable physics-informed neural networks for PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.00377)

   *Amuthan A. Ramabathiran and Prabhu Ramachandran.*

1. **Fast neural network based solving of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.08978)

   *Jaroslaw Rzepecki, Daniel Bates, and Chris Doran.*

1. **Discontinuity computing using physics-informed neural network.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.03864)

   *Li Liu, Shengping Liu, Hui Xie, Fansheng Xiong, Tengchao Yu, Mengjuan Xiao, Lufeng Liu, and Heng Yong.*

1. **Learning differentiable solvers for systems with hard constraints.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.08675)

   *Geoffrey Négiar, Michael W. Mahoney, and Aditi S. Krishnapriyan.*

1. **Momentum diminishes the effect of spectral bias in physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.14862)

   *Ghazal Farhani, Alexander Kazachek, and Boyu Wang.*

1. **Δ-PINNs: Physics-informed neural networks on complex geometries.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.03984)

    *Francisco Sahli Costabal, Simone Pezzuto, and Paris Perdikaris.*

1. **Replacing automatic differentiation by Sobolev Cubatures fastens physics informed neural nets and strengthens their approximation power.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15443)

   *Juan Esteban Suarez Cardona and Michael Hecht.*
   
1. **FO-PINNs: A first-order formulation for physics informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.14320)

   *Rini J. Gladstone, Mohammad A. Nabian, and Hadi Meidani.*

1. **Augmented physics-informed neural networks (APINNs): A gating network-based soft domain decomposition methodology.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.08939)

   *Zheyuan Hu, Ameya D. Jagtap, George Em Karniadakis, and Kenji Kawaguchi.*

1. **Physics-informed Koopman network.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.09419)

   *Yuying Liu, Aleksei Sholokhov, Hassan Mansour, and Saleh Nabi.*

1. **Physics-informed neural networks for operator equations with stochastic data.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.10344)

   *Paul Escapil-Inchauspé and Gonzalo A. Ruz.*

1. **Physics-informed neural networks with unknown measurement noise.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15498)

   *Philipp Pilar and Niklas Wahlstrom.*

1. **On the compatibility between a neural network and a partial differential equation for physics-informed learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00270)

   *Kuangdai Leng and Jeyan Thiyagalingam.*

1. **Pre-training strategy for solving evolution equations based on physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00798)

   *Jiawei Guo, Yanzhong Yao, Han Wang, and Tongxiang Gu.*

### [DeepONet](#content)
1. **Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators.** NMI, 2021. [paper](https://www.nature.com/articles/s42256-021-00302-5)

   *Lu Lu, Pengzhan Jin, Guofei Pang, Zhongqiang Zhang, and George Em Karniadakis.*

1. **Learning the solution operator of parametric partial differential equations with physics-informed DeepONets.** Science Advances, 2021. [paper](https://www.science.org/doi/10.1126/sciadv.abi8605)

   *Wang Sifan, Hanwen Wang, and Paris Perdikaris.*

1. **Deep transfer operator learning for partial differential equations under conditional shift.** NMI, 2022. [paper](https://www.nature.com/articles/s42256-022-00569-2) 

   *Somdatta Goswami, Katiana Kontolati, Michael D. Shields, and George Em Karniadakis.*

1. **Variable-input deep operator networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.11404)

   *Michael Prasthofer, Tim De Ryck, and Siddhartha Mishra..*

1. **MIONet: Learning multiple-input operators via tensor product.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.06137)

   *Jeremy Yu, Lu Lu, Xuhui Meng, and George Em Karniadakis.*

1. **Error estimates for DeepONets: A deep learning framework in infinite dimensions.** Transactions of Mathematics and Its Applications, 2022. [paper](https://academic.oup.com/imatrm/article/6/1/tnac001/6542709)

   *Samuel Lanthaler, Siddhartha Mishra, and George E Karniadakis.*

1. **Long-time integration of parametric evolution equations with physics-informed DeepONets.** arXiv, 2021. [paper](https://arxiv.org/abs/2106.05384)

   *Sifan Wang and Paris Perdikaris.*

1. **Improved architectures and training algorithms for deep operator networks.** Journal of Scientific Computing, 2022. [paper](https://link.springer.com/article/10.1007/s10915-022-01881-0)

   *Sifan Wang, Hanwen Wang, and Paris Perdikaris.*

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

1. **On universal approximation and error bounds for Fourier neural operators.** JMLR, 2021. [paper](https://dl.acm.org/doi/abs/10.5555/3546258.3546548)

   *Nikola Kovachki, Samuel Lanthaler, and Siddhartha Mishra.*

1. **HyperFNO: Improving the generalization behavior of Fourier neural operators.** NIPS, 2022. [paper](https://ml4physicalsciences.github.io/2022/files/NeurIPS_ML4PS_2022_89.pdf)

   *Francesco Alesiani, Makoto Takamoto, and Mathias Niepert.*

1. **Neural operator: Graph kernel network for partial Differential equations.** arXiv, 2020. [paper](https://arxiv.org/abs/2003.03485)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Fourier neural operator with learned deformations for PDEs on general geometries.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.05209)

   *Zongyi Li, Daniel Zhengyu Huang, Burigede Liu, and Anima Anandkumar.*

1. **Multipole graph neural operator for parametric partial differential equations.** NeurIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496291)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Fast sampling of diffusion models via operator learning.** NeurIPS, 2022. [paper](https://openreview.net/forum?id=XrhofG6qg7Y)

   *Hongkai Zheng, Weili Nie, Arash Vahdat, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Factorized Fourier neural operators.** ICLR, 2023. [paper](https://openreview.net/forum?id=tmIiMPl4IPa)

   *Alasdair Tran, Alexander Mathews, Lexing Xie, and Cheng Soon Ong.*

1. **Model inversion for spatio-temporal processes using the Fourier neural operator.** NIPS, 2023. [paper](https://ml4physicalsciences.github.io/2021/files/NeurIPS_ML4PS_2021_8.pdf)

   *Dan MacKinlay, Dan Pagendam, Petra M. Kuhnert, Tao Cui, David Robertson, and Sreekanth Janardhanan.*

1. **Learning deep implicit Fourier neural operators (IFNOs) with applications to heterogeneous material modeling.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522004078)

   *Huaiqian You, Quinn Zhang, Colton J. Ross, Chung-Hao Lee, and Yue Yu.*

1. **On the eigenvector bias of Fourier feature networks: From regression to solving multi-scale PDEs with physics-informed neural networks.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521002759)

   *Sifan Wang, Hanwen Wang, and Paris Perdikaris.*

1. **Semi-supervised learning of partial differential operators and dynamical flows.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.14366)

   *Michael Rotman, Amit Dekel, Ran Ilan Ber, Lior Wolf, and Yaron Oz.*

1. **Non-equispaced Fourier neural solvers for PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04689)

   *Haitao Lin, Lirong Wu, Yongjie Xu, Yufei Huang, Siyuan Li, Guojiang Zhao, Stan Z, and Li Cari.*

1. **Incremental Fourier neural operator.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15188)

   *Jiawei Zhao, Robert Joseph George, Yifei Zhang, Zongyi Li, and Anima Anandkumar.*

1. **Fourier continuation for exact derivative computation in physics-informed neural operators.** NIPS, 2022. [paper](https://arxiv.org/abs/2211.15188)

   *Haydn Maust, Zongyi Li, Yixuan Wang, Daniel Leibovici, Oscar Bruno, Thomas Hou, and Anima Anandkumar.*

### [Graph Network](#content)
1. **Message passing neural PDE solvers.** ICLR, 2022. [paper](https://openreview.net/forum?id=vSix3HPYKSU)

   *Johannes Brandstetter, Daniel E. Worrall, and Max Welling.*

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR, 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP)

   *Xu Han, Han Gao, Tobias Pfaff, Jian-Xun Wang, and Liping Liu.*

1. **Learning mesh-based simulation with graph networks.** ICLR, 2021. [paper](https://openreview.net/forum?id=roNqYL0_XP)

   *Tobias Pfaff, Meire Fortunato, Alvaro Sanchez-Gonzalez, and Peter Battaglia.*

1. **Learning large-scale subsurface simulations with a hybrid graph network simulator.** KDD, 2022. [paper](https://arxiv.org/abs/2206.07680)

   *Tailin Wu, Qinchen Wang, Yinan Zhang, Rex Ying, Kaidi Cao, Rok Sosič, Ridwan Jalali, Hassan Hamam, Marko Maucec, and Jure Leskovec.*

1. **Unravelling the performance of physics-informed graph neural networks for dynamical systems.** NIPS, 2022. [paper](https://openreview.net/forum?id=tXEe-Ew_ikh)

   *Abishek Thangamuthu, Gunjan Kumar, Suresh Bishnoi, Ravinder Bhattoo, N M Anoop Krishnan, and Sayan Ranu.*

1. **Learning the solution operator of boundary value problems using graph neural networks.** ICML, 2022. [paper](https://arxiv.org/abs/2206.14092)

   *Winfried Lötzsch, Simon Ohler, and Johannes S. Otterbach.*

1. **Physics-informed graph neural Galerkin networks: A unified framework for solving PDE-governed forward and inverse problems.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521007076)

   *Han Gao, Matthew J.Zahr, and Jian-Xun Wang.*

1. **Modular flows: Differential molecular generation.** NIPS, 2022. [paper](https://openreview.net/forum?id=kCnwOP-FYdz)

   *Yogesh Verma, Samuel Kaski, Markus Heinonen, and Vikas Garg.*

1. **Learning to solve PDE-constrained inverse problems with graph networks.** ICML, 2022. [paper](https://openreview.net/pdf?id=cLR6FCyMY5k)

   *Zhao Qingqing, David B. Lindell, and Gordon Wetzstein.*

1. **Physics-embedded neural networks: E(n)-equivariant graph neural PDE solvers.** NIPS, 2022. [paper](https://openreview.net/pdf/e2112b7c6c9f008200054c5e466671c1d571aa74.pdf)

   *Masanobu Horie and Naoto Mitsume.*

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

1. **Multi-scale physical representations for approximating PDE solutions with graph neural operators.** ICLR, 2022. [paper](https://arxiv.org/abs/2206.14687)

   *Léon Migus, Yuan Yin, Jocelyn Ahmed Mazari, and Patrick Gallinari.*

1. **DS-GPS : A deep statistical graph Poisson solver (for faster CFD simulations).** NIPS, 2022. [paper](https://arxiv.org/abs/2211.11763)

   *Matthieu Nastorg, Marc Schoenauer, Guillaume Charpiat, Thibault Faney, Jean-Marc Gratien, and Michele-Alessandro Bucci.*

1. **GRAND: Graph neural diffusion.** ICML, 2021. [paper](https://openreview.net/forum?id=_1fu_cjsaRE)

   *Benjamin Paul Chamberlain, James Rowbottom, Maria I. Gorinova, Stefan D Webb, Emanuele Rossi, and Michael M. Bronstein.*

1. **GRAND++: Graph neural diffusion with a source term.** ICML, 2022. [paper](https://openreview.net/forum?id=EMxu-dzvJk)

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.*

1. **Neural networks trained to solve differential equations learn general representations.** NIPS, 2018. [paper](https://proceedings.neurips.cc/paper/2018/hash/d7a84628c025d30f7b2c52c958767e76-Abstract.html)

   *Martin Magill, Faisal Qureshi, and Hendrick de Haan.*

1. **Graph element networks: Adaptive, structured computation and memory.** ICML, 2019. [paper](http://proceedings.mlr.press/v97/alet19a.html?ref=https://githubhelp.com)

   *Ferran Alet, Adarsh Keshav Jeewajee, Maria Bauza Villalonga, Alberto Rodriguez, Tomas Lozano-Perez, and Leslie Kaelbling.*

1. **Physics-constrained unsupervised learning of partial differential equations using meshes.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.16628)

   *Mike Y. Michelis and Robert K. Katzschmann.*

2. **Neural PDE solvers for irregular domains.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.03241)

   *Biswajit Khara, Ethan Herron, Zhanhong Jiang, Aditya Balu, Chih-Hsuan Yang, Kumar Saurabh, Anushrut Jignasu, Soumik Sarkar, Chinmay Hegde, Adarsh Krishnamurthy, and Baskar Ganapathysubramanian.*

2. **Bi-stride multi-scale graph neural network for mesh-based physical simulation.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.02573)

   *Yadi Cao, Menglei Chai, Minchen Li, and Chenfanfu Jiang.*

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
1. **Learning Green's functions associated with time-dependent partial differential equations.** JMLR, 2022. [paper](https://www.jmlr.org/papers/volume23/22-0433/22-0433.pdf)

   *Nicolas Boullé, Seick Kim, Tianyi Shi, and Alex Townsend.*

1. **BI-GreenNet: Learning Green's functions by boundary integral network.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.13247)

   *Guochang Lin, Fukai Chen, Pipi Hu, Xiang Chen, Junqing Chen, Jun Wang, and Zuoqiang Shi.*

1. **DeepGreen: deep learning of Green’s functions for nonlinear boundary value problems.** Scientific Reports, 2021. [paper](https://www.nature.com/articles/s41598-021-00773-x)

   *Craig R. Gin, Daniel E. Shea, Steven L. Brunton, and J. Nathan Kutz.*

1. **Data-driven discovery of Green’s functions with human-understandable deep learning.** Scientific Reports, 2022. [paper](https://www.nature.com/articles/s41598-022-08745-5)

   *Nicolas Boullé, Christopher J. Earls, and Alex Townsend.*

1. **Data-driven discovery of Green's functions.** Doctoral Dissertation, 2022. [Ph.D.](https://arxiv.org/abs/2210.16016)

   *Nicolas Boullé.*
   
1. **Principled interpolation of Green's functions learned from data.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.06299)

   *Harshwardhan Praveen, Nicolas Boulle, and Christopher Earls.*

### [Finite Element](#content)
1. **Composing partial differential equations with physics-aware neural networks.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/karlbauer22a/karlbauer22a.pdf)

   *Matthias Karlbauer, Timothy Praditia, Sebastian Otte, Sergey Oladyshkin, and Wolfgang Nowak.*

1. **Learning the dynamics of physical systems from sparse observations with finite element networks.** ICLR, 2022. [paper](https://openreview.net/forum?id=HFmAukZ-k-2)

   *Marten Lienen and Stephan Günnemann.*

1. **A unified hard-constraint framework for solving geometrically complex PDEs.** NIPS, 2022. [paper](https://arxiv.org/abs/2210.03526)

   *Songming Liu, Zhongkai Hao, Chengyang Ying, Hang Su, Jun Zhu, and Ze Cheng.*

1. **LSH-SMILE: Locality sensitive Hashing accelerated simulation and learning.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/3d98b79ac6c8d1cef43d7bf1dadf8647-Abstract.html)

   *Chonghao Sima and Yexiang Xue.*

1. **Amortized finite element analysis for fast PDE-constrained optimization.** ICML, 2020. [paper](https://proceedings.mlr.press/v119/xue20a.html)

   *Tianju Xue, Alex Beatson, Sigrid Adriaenssens, and Ryan Adams.*

1. **Learning neural PDE solvers with convergence guarantees.** ICLR, 2019. [paper](https://openreview.net/forum?id=rklaWn0qK7)

   *Jun-Ting Hsieh, Shengjia Zhao, Stephan Eismann, Lucia Mirabella, and Stefano Ermon.*

1. **Hybrid finite difference with the physics-informed neural network for solving PDE in complex geometries.** arXiv, 2022. [paper](https://arxiv.org/pdf/2202.07926.pdf)

   *Zixue Xiang, Wei Peng, Weien Zhou, and Wen Yao.*

1. **Multilayer perceptron-based surrogate models for finite element analysis.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.09380)

   *Lawson Oliveira Lima, Julien Rosenberger, Esteban Antier, and Frederic Magoules.*

### [Convolutional Filter](#content)
1. **PDE-Net: Learning PDEs from data.** ICML, 2018. [paper](https://proceedings.mlr.press/v80/long18a.html)

   *Zichao Long, Yiping Lu, Xianzhong Ma, and Bin Dong.*

1. **PDE-Net 2.0: Learning PDEs from data with a numeric-symbolic hybrid deep network.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119306308)

   *ZichaoLong, YipingLu, and Bin Dong.*

1. **Physics-informed CNNs for super-resolution of sparse observations on dynamical systems.** NIPS, 2022. [paper](https://arxiv.org/abs/2210.17319)

   *Daniel Kelshaw, Georgios Rigas, and Luca Magri.*

1. **Deep-pretrained-FWI: Combining supervised learning with physics-informed neural network.** NIPS, 2022. [paper](https://arxiv.org/abs/2212.02338)

   *Ana Paula O. Muller, Clecio R. Bom, Jessé C. Costa, Matheus Klatt, Elisângela L. Faria, Marcelo P. de Albuquerque, and Márcio P. de Albuquerque.*

1. **Learning time-dependent PDEs with a linear and nonlinear separate convolutional neural network.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121008238)

   *Jiagang Qu, Weihua Cai, and YijunZhao.*

1. **PhyCRNet: Physics-informed convolutional-recurrent network for solving spatiotemporal PDEs.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521006514)

   *Pu Ren, Chengping Rao, Yang Liu, Jian-Xun Wang, and Hao Sun.*

1. **Deep-pretrained-FWI: Combining supervised learning with physics-informed neural network.** NIPS, 2022. [paper](https://arxiv.org/abs/2212.02338)

   *Ana Paula O. Muller, Clecio R. Bom, Jessé C. Costa, Matheus Klatt, Elisângela L. Faria, Marcelo P. de Albuquerque, and Márcio P. de Albuquerque.*

1. **Spline-PINN: Approaching PDEs without data using fast, physics-informed Hermite-Spline CNNs.** AAAI, 2019. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/20830/20589)

   *Nils Wandel, Michael Weinmann, Michael Neidlin, and Reinhard Klein.*

1. **Deep convolutional Ritz method: Parametric PDE surrogates without labeled data.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.04675)

   *Jan Niklas Fuhg, Arnav Karmarkar, Teeratorn Kadeethum, Hongkyu Yoon, and Nikolaos Bouklas.*

1. **Deep convolutional architectures for extrapolative forecasts in time-dependent flow problems.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.09651)

   *Pratyush Bhatt, Yash Kumar, and Azzeddine Soulaimani.*

1. **Phase2Vec: Dynamical systems embedding with a physics-informed convolutional network.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.03857)

   *Matthew Ricci, Noa Moriel, and Zoe Piran, Mor Nitzan.*

1. **Numerical approximation based on deep convolutional neural network for high-dimensional fully nonlinear merged PDEs and 2BSDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.04997)

   *Xu Xiao and Wenlin Qiu.*

1. **SplineCNN: Fast geometric deep learning with continuous B-spline kernels.** CVPR, 2018. [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Fey_SplineCNN_Fast_Geometric_CVPR_2018_paper.pdf)

   *Matthias Fey, Jan Eric Lenssen, Frank Weichert, and Heinrich Muller.*

1. **Spline-PINN: Approaching PDEs without data using fast, physics-informed Hermite-Spline CNNs.** AAAI, 2019. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/20830/20589)

   *Nils Wandel, Michael Weinmann, Michael Neidlin, and Reinhard Klein.*

1. **Physics-informed deep super-resolution for spatiotemporal data.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.01462)

   *Pu Ren, Chengping Rao, Yang Liu, Zihan Ma, Qi Wang, Jian-Xun Wang, and Hao Sun.*

1. **An unsupervised latent/output physics-informed convolutional-LSTM network for solving partial differential equations using peridynamic differential operator.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.12177)

   *A. Mavi, A.C. Bekar, E. Haghighat, and E. Madenci.*

1. **MeshFreeFLowNet: A physics-constrained deep continuous space-time super-resolution framework.** SC, 2020. [paper](https://ieeexplore.ieee.org/document/9355293)

   *Chiyu Max Jiang, Soheil Esmaeilzadeh, Kamyar Azizzadenesheli, Karthik Kashinath, Mustafa Mustafa, Hamdi A. Tchelepi, Philip Marcus Prabhat, and Anima Anandkumar.*

### [AutoEncoder](#content)
1. **Integral autoencoder network for discretization-invariant learning.** JMLR, 2022. [paper](https://www.jmlr.org/papers/v23/22-0297.html)

   *Yong Zheng Ong, Zuowei Shen, and Haizhao Yang.*

### [Operator](#content)
1. **Multiwavelet-based operator learning for differential equations.** NIPS, 2021. [paper](https://openreview.net/forum?id=LZDiWaC9CGL)

   *Gaurav Gupta, Xiongye Xiao, and Paul Bogdan.*

1. **On the representation of solutions to elliptic PDEs in Barron space.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/32cfdce9631d8c7906e8e9d6e68b514b-Abstract.html)

   *Ziang Chen, Jianfeng Lu, and Yulong Lu.*

1. **Low-rank registration based manifolds for convection-dominated PDEs.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16116)

   *Rambod Mojgani and Maciej Balajewicz.*

1. **A nonlocal physics-informed deep learning framework using the peridynamic differential operator.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521003431)

   *Ehsan Haghighat, Ali CanBekar, Erdogan Madenci, and Ruben Juanes.*

1. **Kernel Flows: From learning kernels from data into the abyss.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119302232)

   *Houman Owhadi and Gene Ryan Yoo.*

1. **On neurosymbolic solutions for PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.06240)

   *Ritam Majumdar, Vishal Jadhav, Anirudh Deodhar, Shirish Karande, and Lovekesh Vig.*

1. **An introduction to kernel and operator learning methods for homogenization by self-consistent clustering analysis.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00802)

   *Owen Huang, Sourav Saha, Jiachen Guo, and Wing Kam Liu.*

1. **Nonparametric learning of kernels in nonlocal operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.11006)

   *Fei Lu, Qingci An, and Yue Yu.*

1. **Spectral neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.10573)

   *V. Fanasko and I. Oseledets.*

1. **NOMAD: Nonlinear manifold decoders for operator learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.03551)

   *Jacob H. Seidman, Georgios Kissas, Paris Perdikaris, and George J. Pappas.*

1. **U-NO: U-shaped neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.11127)

   *Md Ashiqur Rahman, Zachary E. Ross, and Kamyar Azizzadenesheli.*

1. **Wavelet neural operator: A neural operator for parametric partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.02191)

   *Tapas Tripura and Souvik Chakraborty.*

1. **Pseudo-differential integral operator for learning solution operators of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2201.11967)

   *Jin Young Shin, Jae Yong Lee, and Hyung Ju Hwang.*

1. **Nonlinear reconstruction for operator learning of PDEs with discontinuities.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.01074)

   *Samuel Lanthaler, Roberto Molinaro, Patrik Hadorn, and Siddhartha Mishra.*

1. **GeONet: A neural operator for learning the Wasserstein geodesic.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.14440)

   *Andrew Gracyk and Xiaohui Chen.*

1. **Render unto numerics: Orthogonal polynomial neural operator for PDEs with non-periodic boundary conditions.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.12698)

   *Ziyuan Liu, Haifeng Wang, Kaijuna Bao, Xu Qian, Hong Zhang, and Songhe Song.*

1. **DOSNet as a non-black-box PDE solver: When deep learning meets operator splitting.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.05571)

   *Yuan Lan, Zhen Li, Jie Sun, and Yang Xiang.*

### [Identification](#content)
1. **Data-driven discovery of partial differential equations.** SA, 2017. [paper](https://arxiv.org/abs/1910.11710)

   *Wei Cai and Zhi-Qin John Xu.*

1. **Robust learning from noisy, incomplete, high-dimensional experimental data via physically constrained symbolic regression.** NC, 2021. [paper](https://www.nature.com/articles/s41467-021-23479-0)

   *Patrick A. K. Reinbold, Logan M. Kageorge, Michael F. Schatz, and Roman O. Grigoriev.*

1. **Discovering nonlinear PDEs from scarce data with physics-encoded learning.** ICLR, 2022. [paper](https://openreview.net/pdf?id=Vog_3GXsgmb)

   *Chengping Rao, Pu Ren, Yang Liu, and Hao Sun.*

1. **Differential spectral normalization (DSN) for PDE discovery.** AAAI, 2021. [paper](https://openreview.net/pdf?id=Vog_3GXsgmb)

   *Chi Chiu So, Tsz On Li, Chufang Wu, and Siu Pang Yung.*

1. **Learning differential operators for interpretable time series modeling.** KDD, 2022. [paper](https://dl.acm.org/doi/abs/10.1145/3534678.3539245)

   *Yingtao Luo, Chang Xu, Yang Liu, Weiqing Liu, Shun Zheng, and Jiang Bian.*

1. **Learning emergent partial differential equations in a learned emergent space.** NC, 2022. [paper](https://www.nature.com/articles/s41467-022-30628-6)

   *Felix P. Kemeth, Tom Bertalan, Thomas Thiem, Felix Dietrich, Sung Joon Moon, Carlo R. Laing, and Ioannis G. Kevrekidis.*

1. **Physics-informed learning of governing equations from scarce data.** NC, 2021. [paper](https://www.nature.com/articles/s41467-021-26434-1)

   *Zhao Chen, Yang Liu, and Hao Sun.*

1. **Machine Learning Hidden Symmetries.** PRL, 2022. [paper](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.128.180201)

   *Ziming Liu and Max Tegmark.*

1. **Data-driven discovery of partial differential equation models with latent variables.** Physical Review E, 2019. [paper](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.100.022219)

   *Patrick A. K. Reinbold and Roman O. Grigoriev.*

1. **Physics constrained learning for data-driven inverse modeling from sparse observations.** Physical Review E, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121008330)

   *Kailai Xua and Eric Darve.*

1. **Deep neural network modeling of unknown partial differential equations in nodal space.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100677X)

   *Zhen Chen, and Victor Churchill, Kailiang Wu, and Dongbin Xiu.*

1. **DeepMoD: Deep learning for model discovery in noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120307592)

   *Gert-Jan Both, Subham Choudhury, Pierre Sens, and Remy Kusters.*

1. **Theory-guided hard constraint projection (HCP): A knowledge-based data-driven scientific machine learning method.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005192)

   *Yuntian Chen, Dou Huang, Dongxiao Zhang, Junsheng Zeng, Nanzhe Wang, Haoran Zhang, and Jinyue Yan.*

1. **Deep-learning based discovery of partial differential equations in integral form from sparse and noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121004873)

   *Hao Xua, Dongxiao Zhang, and Nanzhe Wang.*

1. **Peridynamics enabled learning partial differential equations.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121000887)

   *Ali C.Bekar and Erdogan Madenci.*

1. **Data-driven deep learning of partial differential equations in modal space.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120300814)

   *Kailiang Wu and Dongbin Xiu.*

1. **DLGA-PDE: Discovery of PDEs with incomplete candidate library via combination of deep learning and genetic algorithm.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120303582)

   *Hao Xu, Haibin Chang, and Dongxiao Zhang.*

1. **Learning nonlocal constitutive models with neural networks.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521002644)

   *Xu-Hui Zhou, Jiequn Han, and Heng Xiao.*

1. **Data-driven identification of parametric partial differential equations.** SIAM Journal on Applied Dynamical Systems, 2019. [paper](https://epubs.siam.org/doi/abs/10.1137/18M1191944)

   *Samuel Rudy, Alessandro Alla, Steven L. Brunton, and J. Nathan Kutz.*

1. **PDE-READ: Human-readable partial differential equation discovery using deep learning.** Neural Networks, 2022. [paper](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.100.022219)

   *Robert Stephany and Christopher Earls.*

1. **Discover: Deep identification of symbolic open-form PDEs via enhanced reinforcement-learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.02181)

   *Mengge Du, Yuntian Chen, and Dongxiao Zhang.*

1. **ModLaNets: Learning generalisable dynamics via modularity and physical inductive bias.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/lu22c/lu22c.pdf)

   *Yupu Lu, Shijie Lin, Guanqi Chen, and Jia Pan.*

1. **Robust discovery of partial differential equations in complex situations.** Physical Review Research, 2021. [paper](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.033270)

   *Hao Xu and Dongxiao Zhang.*

1. **Modeling the dynamics of PDE systems with physics-constrained deep auto-regressive networks.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307612)

   *Nicholas Geneva and Nicholas Zabaras.*

1. **Deep learning and inverse discovery of polymer self-consistent field theory inspired by physics-informed neural networks.** Physical Review E, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307612)

   *Danny Lin and Hsiu-Yu Yu.*

1. **Data-driven solutions and parameter discovery of the Sasa–Satsuma equation via the physics-informed neural networks method.** Physica D, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0167278922002044)

   *Haotian Luo, Lei Wang, Ya-Bin Zhang, Gui Lu, Jing-Jing Su, and Yin-Chuan Zhao.*
   
1. **Neural operator with regularity structure for modeling dynamics driven by SPDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.06255)

   *Peiyan Hu, Qi Meng, Bingguang Chen, Shiqi Gong, Yue Wang, Wei Chen, Rongchan Zhu, Zhi-Ming Ma, and Tie-Yan Liu.*
   
1. **A PINN approach to symbolic differential operator discovery with sparse data.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04630)

   *Lena Podina, Brydon Eastman, and Mohammad Kohandel.*
   
1. **WeakIdent: Weak formulation for identifying differential equations using narrow-fit and trimming.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.03134)

   *Mengyi Tang, Wenjing Liao, Rachel Kuske, and Sung Ha Kang.*

1. **Predicting parametric spatiotemporal dynamics by multi-resolution PDE structure-preserved deep learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.03990)

   *Xin-Yang Liu, Hao Sun, and Jian-Xun Wang.*

1. **Data-driven modeling of Landau damping by physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.01021)

   *Yilan Qin, Jiayu Ma, Mingle Jiang, Chuanfei Dong, Haiyang Fu, Liang Wang, Wenjie Cheng, and Yaqiu Jin.*

1. **Discovering governing equations in discrete systems using PINNs.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00971)

   *Sheikh Saqlain, Wei Zhu, Efstathios G. Charalampidis, and Panayotis G. Kevrekidis.*

1. **PDE-LEARN: Using deep learning to discover partial differential equations from noisy, limited data.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04971)

   *Robert Stephany and Christopher Earls.*

### [Machine Learning](#content)
1. **Data-driven discovery of intrinsic dynamics.** NMI, 2022. [paper](https://www.nature.com/articles/s42256-022-00575-4)

   *Daniel Floryan and Michael D. Graham.*

1. **Machine learning–accelerated computational fluid dynamics.** PNAS, 2021. [paper](https://www.pnas.org/doi/10.1073/pnas.2101784118)

   *Dmitrii Kochkov, Jamie A. Smith, Ayya Alieva, and Stephan Hoyer.*

1. **Learning data-driven discretization for partial differential equations.** PNAS, 2019. [paper](https://www.pnas.org/doi/10.1073/pnas.1814058116)

   *Yohai Bar-Sinai, Stephan Hoyer, Jason Hickey, and Michael P. Brenner.*

1. **Solving high-dimensional partial differential equations using deep learning.** PNAS, 2018. [paper](https://www.pnas.org/doi/10.1073/pnas.1718942115)

   *Jiequn Han, Arnulf Jentzen, and Weinan E.*

1. **Enhancing computational fluid dynamics with machine learning.** NCS, 2022. [paper](https://www.nature.com/articles/s43588-022-00264-7)

   *Ricardo Vinuesa and Steven L. Brunton.*

1. **Solving high-dimensional parabolic PDEs using the tensor train format.** ICML, 2021. [paper](https://arxiv.org/abs/2102.11830)

   *Lorenz Richter, Leon Sallandt, and Nikolas Nüsken.*

1. **A hybrid reduced basis and machine-learning algorithm for building surrogate models: A first application to electromagnetism.** NIPS, 2022. [paper](https://www.researchgate.net/profile/Alejandro-Ribes/publication/365152878_A_hybrid_Reduced_Basis_and_Machine-Learning_algorithm_for_building_Surrogate_Models_a_first_application_to_electromagnetism/links/6366a7de37878b3e87852084/A-hybrid-Reduced-Basis-and-Machine-Learning-algorithm-for-building-Surrogate-Models-a-first-application-to-electromagnetism.pdf)

   *Alejandro Ribés and Ruben Persicot.*

1. **Numerically solving parametric families of high-dimensional Kolmogorov partial differential equations via deep learning.** NIPS, 2020. [paper](https://proceedings.neurips.cc/paper/2020/hash/c1714160652ca6408774473810765950-Abstract.html)

   *Julius Berner, Markus Dablander, and Philipp Grohs.*

1. **Nonlocal kernel network (NKN): A stable and resolution-independent deep neural network.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122005988)

   *Huaiqian You, Yue Yu, Marta D'Elia, Tian Gao, and Stewart Silling.*

1. **On computing the hyperparameter of extreme learning machines: Algorithm and application to computational PDEs, and comparison with classical and high-order finite elements.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003527#!)

   *Suchuan Dong and Jielin Yang.*

1. **Int-Deep: A deep learning initialized iterative method for nonlinear problems.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120304496)

   *Jianguo Huang, Haoqin Wang, and Haizhao Yang.*

1. **DeLISA: Deep learning based iteration scheme approximation for solving PDEs.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121007798)

   *Ying Li, Zuojia Zhou, and Shihui Ying.*

1. **Physics-informed machine learning for reduced-order modeling of nonlinear problems.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005611)

   *Wenqian Chen, Qian Wang, Jan S.Hesthaven, and Chuhua Zhang.*

1. **SelectNet: Self-paced learning for high-dimensional partial differential equations.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121003399)

   *Yiqi Gu, Haizhao Yang, and Chao Zhou.*

1. **DPM: A deep learning PDE augmentation method with application to large-eddy simulation.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120305854)

   *Justin Sirignano, Jonathan F.MacArt, and Jonathan B.Freund.*

1. **Deep least-squares methods: An unsupervised learning-based numerical method for solving elliptic PDEs.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120304812)

   *Zhiqiang Cai, Jingshuang Chen, MinLiu, and Xinyu Liu.*

1. **Local extreme learning machines and domain decomposition for solving linear and nonlinear partial differential equations.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521004606)

   *Suchuan Dong and Zongwei Li.*

1. **Iterative surrogate model optimization (ISMO): An active learning algorithm for PDE constrained optimization with deep neural networks.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S004578252030760X)

   *Kjetil O.Lye, Siddhartha Mishra, Deep Ray, and Praveen Chandrashekar.*

1. **Probabilistic learning on manifolds constrained by nonlinear partial differential equations for small datasets.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521001134)

   *C. Soize and R. Ghanem.*

1. **An energy approach to the solution of partial differential equations in computational mechanics via machine learning: Concepts, implementation and applications.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782519306826)

   *E. Samaniego, C. Anitescu, S.Goswami, V.M.Nguyen-Thanh, H.Guo, K.Hamdia, ,X.Zhuang, and T.Rabczuk.*

1. **Reduced order modeling for parameterized time-dependent PDEs using spatially and memory aware deep learning.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S1877750321000934)

   *Nikolaj T.Mücke, Sander M.Bohté, and Cornelis W.Oosterlee.*

1. **GCN-FFNN: A two-stream deep model for learning solution to partial differential equations.** Neurocomputing, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0925231222011511?dgcid=rss_sd_all)

   *Onur Bilgin, Thomas Vergutz, Siamak Mehrkanoon.*

1. **Deep-HyROMnet: A deep learning-based operator approximation for hyper-reduction of nonlinear parametrized PDEs.** Journal of Scientific Computing, 2021. [paper](https://link.springer.com/article/10.1007/s10915-022-02001-8)

   *Ludovica Cicci, Stefania Fresca, and Andrea Manzoni.*

1. **HybridNet: Integrating Model-based and Data-driven Learning to Predict Evolution of Dynamical Systems.** CoRL, 2018. [paper](https://proceedings.mlr.press/v87/long18a.html)

   *Yun Long, Xueyuan She, and Saibal Mukhopadhyay.*

1. **A model-constrained tangent slope learning approach for dynamical systems.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.04995)

   *Hai V. Nguyen and Tan Bui-Thanh.*

1. **Convergence analysis of a quasi-Monte Carlo-based deep learning algorithm for solving partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.16196)

   *Fengjiang Fu and Xiaoqun Wang.*

1. **Quantum-inspired tensor neural networks for partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.02235)

   *Raj Patel, Chia-Wei Hsing, Serkan Sahin, Saeed S. Jahromi, Samuel Palmer, Shivam Sharma, Christophe Michel, Vincent Porte, Mustafa Abid, Stephane Aubert, Pierre Castellani, Chi-Guhn Lee, Samuel Mugel, and Roman Orus.*

1. **Solving PDEs on unknown manifolds with machine learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2106.06682)

   *Senwei Liang, Shixiao W. Jiang, John Harlim, and Haizhao Yang.*

1. **Model reduction and neural networks for parametric PDEs.** SIAM Journal of Computational Mathematics, 2021. [paper](https://smai-jcm.centre-mersenne.org/item/SMAI-JCM_2021__7__121_0/)

   *Kaushik Bhattacharya, Bamdad Hosseini, Nikola B. Kovachki, and Andrew M. Stuart.*

1. **MOD-Net: A machine learning approach via model-operator-data network for solving PDEs.** Communications in Computational Physics, 2022. [paper](https://global-sci.org/intro/article_detail/cicp/20860.html#)

   *Shamsulhaq Basir and Inanc Senocak.*

### [ODE](#content)
1. **Neural rough differential equations for long time series.** ICML, 2021. [paper](http://proceedings.mlr.press/v139/morrill21b.html)

   *James Morrill, Cristopher Salvi, Patrick Kidger, and James Foster.*

1. **LEADS: Learning dynamical systems that generalize across environments.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/3df1d4b96d8976ff5986393e8767f5b2-Abstract.html)

   *Yuan Yin, Ibrahim Ayed, Emmanuel de Bézenac, and Nicolas Baskiotis, and Patrick Gallinari.*

1. **On robustness of neural ordinary differential equations.** ICLR, 2020. [paper](https://openreview.net/forum?id=-gBckR-V1i)

   *Hanshu Yan, Jiawei Du, Vincent Y. F. Tan, and Jiashi Feng.*

1. **Spectrum dependent learning curves in kernel regression and wide neural networks.** ICML, 2020. [paper](http://proceedings.mlr.press/v119/bordelon20a.html)

   *Blake Bordelon, Abdulkadir Canatar, and Cengiz Pehlevan.*

1. **Beyond finite layer neural networks: Bridging deep architectures and numerical differential equations.** ICML, 2018. [paper](https://arxiv.org/abs/1710.10121)

   *Yiping Lu, Aoxiao Zhong, Quanzheng Li, and Bin Dong.*

1. **Neural ordinary differential equations.** NIPS, 2018. [paper](https://proceedings.neurips.cc/paper/2018/hash/69386f6bb1dfed68692a24c8686939b9-Abstract.html)

   *Ricky T. Q. Chen, Yulia Rubanova, Jesse Bettencourt, and David K. Duvenaud.*

1. **Hamiltonian neural networks.** ICML, 2018. [paper](https://proceedings.neurips.cc/paper/2019/file/26cd8ecadce0d4efd6cc8a8725cbd1f8-Paper.pdf)

   *Sam Greydanus, Misko Dzamba, and Jason Yosinski.*

1. **Hamiltonian neural networks for solving equations of motion.** Physical Review E, 2022. [paper](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.105.065305)

   *Marios Mattheaki , David Sondak, Akshunna S. Dogra, and Pavlos Protopapas.*

1. **Deep learning for universal linear embeddings of nonlinear dynamics.** NC, 2018. [paper](https://www.nature.com/articles/s41467-018-07210-0)

   *Bethany Lusch, J. Nathan Kutz, and Steven L. Brunton.*

1. **Stochastic physics-informed neural ordinary differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2109.01621)

   *Jared O'Leary, Joel A. Paulson, and Ali Mesbah.*

## [Mechanism](#content) 
### [Library](#content)
1. **PDEBench: An extensive benchmark for scientific machine learning.** NIPS, 2022. [paper](https://openreview.net/forum?id=dh_MkX0QfrK)

   *Makoto Takamoto, Timothy Praditia, Raphael Leiteritz, Dan MacKinlay, Francesco Alesiani, Dirk Pflüger, and Mathias Niepert.*

1. **DeepXDE: A deep learning library for solving differential equations.** SIAM Review, 2021. [paper](https://epubs.siam.org/doi/abs/10.1137/19M1274067)

   *Lu Lu, Xuhui Meng, Zhiping Mao, and George Em Karniadakis.*

1. **A research framework for writing differentiable PDE discretizations in JAX.** NIPS, 2021. [paper](https://arxiv.org/abs/2111.05218)

   *Antonio Stanziola, Simon R. Arridge, Ben T. Cox, and Bradley E. Treeby.* 

1. **An extensible benchmarking graph-mesh dataset for studying steady-state incompressible Navier-Stokes equations.** ICLR, 2022. [paper](https://openreview.net/forum?id=rqUUi4-kpeq)

   *Florent Bonnet, Jocelyn Ahmed Mazari, Thibaut Munzer, Pierre Yser, and Patrick Gallinari.* 

1. **PhiFlow: A differentiable PDE solving framework for deep learning via physical simulations.** NIPS, 2020. [paper](https://montrealrobotics.ca/diffcvgp/assets/papers/3.pdf)

   *Philipp Holl, Vladlen Koltun, Kiwon Um, and Nils Thuerey.* 

1. **NVIDIA SimNet™: An AI-accelerated multi-physics simulation framework.** ICCS, 2021. [paper](https://link.springer.com/chapter/10.1007/978-3-030-77977-1_36)

   *Oliver Hennigh, Susheela Narasimhan, Mohammad Amin Nabian, Akshay Subramaniam, Kaustubh Tangsali, Zhiwei Fang, Max Rietmann, Wonmin Byeon, and Sanjay Choudhry.*


1. **PyDEns: A python framework for solving differential equations with neural networks.** arXiv, 2019. [paper](https://arxiv.org/abs/1909.11544)

   *Alexander Koryagin, Roman Khudorozkov, and Sergey Tsimfer.*

### [Analysis](#content)
1. **DPM: Physics-informed Karhunen-Loéve and neural network approximations for solving inverse differential equation problems.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16992/16799)

   *Jungeun Kim, Kookjin Lee, Dongeun Lee, Sheo Yon Jin, and Noseong Park.*

1. **Characterizing possible failure modes in physics-informed neural networks.** NIPS, 2021. [paper](https://openreview.net/forum?id=a2Gr9gNFD-J)

   *Aditi Krishnapriyan, Amir Gholami, Shandian Zhe, Robert Kirby, and Michael W. Mahoney.*

1. **Understanding and mitigating gradient flow pathologies in physics-informed neural networks.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/20M1318043)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **When and why PINNs fail to train: A neural tangent kernel perspective.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100663X)

   *SifanWang, XinlingYu, and Paris Perdikaris.*

1. **When do extended physics-informed neural networks (XPINNs) improve generalization?** SIAM Journal on Scientific Computing, 2022. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1447039)

   *Zheyuan Hu, Ameya D. Jagtap, George Em Karniadakis, and Kenji Kawaguchi.*

1. **MARS: A method for the adaptive removal of stiffness in PDEs.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122006878#!)

   *Laurent Duchemin and Jen Eggers.*

1. **Learning similarity metrics for numerical simulations.** ICML, 2020. [paper](https://proceedings.mlr.press/v119/kohl20a.html)

   *Georg Kohl, Kiwon Um, and Nils Thuerey.*

1. **A curriculum-training-based strategy for distributing collocation points during
physics-informed neural network training.** NIPS, 2021. [paper](https://arxiv.org/abs/2211.11396)

   *Marcus Münzer and Chris Bard.*

1. **Parametric complexity bounds for approximating PDEs with neural networks.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/7edccc661418aeb5761dbcdc06ad490c-Abstract.html)

   *Tanya Marwah, Zachary Lipton, and Andrej Risteski.*

1. **Respecting causality is all you need for training physics-informed neural networks.** arXiv, 2021. [paper](https://arxiv.org/abs/2203.07404)

   *Sifan Wang, Shyam Sankaran, and Paris Perdikaris.*

1. **CP-PINNS: Changepoints detection in PDEs using physics informed neural networks with total-variation penalty.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.08626)

   *Zhikang Dong and Pawel Polak.*

1. **Stochastic projection based approach for gradient free physics informed learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.13724)

   *Navaneeth N and Souvik Chakraborty.*

1. **Understanding the difficulty of training physics-informed neural networks on dynamical systems.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.13648)

   *Franz M. Rohrhofer, Stefan Posch, Clemens Gößnitzer, and Bernhard C. Geiger.*

1. **Mitigating learning complexity in physics and equality constrained artificial neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01807)

   *Victor Churchill and Dongbin Xiu.*

1. **Improved training of physics-informed neural networks with model ensembles.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.05108)

   *Katsiaryna Haitsiukevich and Alexander Ilin.*
   
1. **The cost-accuracy trade-off in operator learning with neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.13181)
   
   *Maarten V. de Hoop, Daniel Zhengyu Huang, Elizabeth Qian, and Andrew M. Stuart.*
   
1. **Neural tangent kernel analysis of PINN for advection-diffusion equation.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.11716)
   
   *M. H. Saadat, B. Gjorgiev, L. Das, and G. Sansavini.* 

1. **Separable PINN: Mitigating the curse of dimensionality in physics-informed neural networks.** NIPS, 2022. [paper](https://openreview.net/forum?id=jGk3DgkHB_)
   
   *Junwoo Cho, Seungtae Nam, Hyunmo Yang, Seok-Bae Yun, Youngjoon Hong, and Eunbyung Park.*

1. **A curriculum-training-based strategy for distributing collocation points during physics-informed neural network training.** NIPS, 2022. [paper](https://arxiv.org/pdf/2211.11396.pdf)
   
   *Marcus Münzer and Chris Bard.*
   
1. **Robustness of physics-informed neural networks to noise in sensor data.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.12042)
   
   *Jian Cheng Wong, Pao-Hsiung Chiu, Chin Chun Ooi, and My Ha Da.* 

### [Attention](#content)
1. **Learning operators with coupled attention.** JMLR, 2022. [paper](https://www.jmlr.org/papers/v23/21-1521.html) 

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.* 

1. **Choose a Transformer: Fourier or Galerkin.** NIPS, 2021. [paper](https://openreview.net/forum?id=ssohLcmn4-r)

   *Shuhao Cao.* 

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR, 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP) 

   *Xu Han, Han Gao, Tobias Pfaff, Jian-Xun Wang, and Liping Liu.*

1. **SiT: Simulation transformer for particle-based physics simulation.** ICLR, 2022. [paper](https://openreview.net/forum?id=DBOibe1ISzB) 

   *Yidi Shao, Chen Change Loy, and Bo Dai.*

1. **Physics-informed long-sequence forecasting from multi-resolution spatiotemporal data.** IJCAI, 2022. [paper](https://www.ijcai.org/proceedings/2022/304) 

   *Chuizheng Meng, Hao Niu, Guillaume Habault, Roberto Legaspi, Shinya Wada, Chihiro Ono, and Yan Liu.*

1. **TransFlowNet: A physics-constrained Transformer framework for spatio-temporal super-resolution of flow simulations.** Journal of Computational Science, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S1877750322002654) 

   *Xinjie Wang, Siyuan Zhu, Yundong Guo, Peng Han, Yucheng Wang, Zhiqiang Wei, and Xiaogang Jin.*

1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS, 2021. [paper](https://arxiv.org/abs/2009.04544) 

   *Levi D. McClenny and Ulisses Braga-Neto.*

1. **Transformer for partial differential equations' operator learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.13671) 

   *Zijie Li, Kazem Meidani, and Amir Barati Farimani.*

1. **Physics-informed attention-based neural network for hyperbolic partial differential equations: Application to the Buckley–Leverett problem.** Scientific Reports, 2022. [paper](https://www.nature.com/articles/s41598-022-11058-2) 

   *Ruben Rodriguez-Torrado, Pablo Ruiz, Luis Cueto-Felgueroso, Michael Cerny Green, Tyler Friesen, Sebastien Matringe, and Julian Togelius.*

1. **Self-adaptive physics-informed neural networks using a soft attention mechanism.** AAAI-MLPS, 2021. [paper](https://github.com/levimcclenny/SA-PINNs) 

   *Levi Mc Clenny and Ulisses Braga-Neto.*

### [Neural Implicit Flow](#content)
1. **Neural implicit flow: A mesh-agnostic dimensionality reduction paradigm of spatio-temporal data.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.03216) 

   *Shaowu Pan, Steven L. Brunton, and J. Nathan Kutz.*

1. **CROM: Continuous reduced-order modeling of PDEs using implicit neural representations.** ICLR , 2023. [paper](https://openreview.net/forum?id=FUORz1tG8Og) 

   *Peter Yichen Chen, Jinxu Xiang, Dong Heon Cho, Yue Chang, G A Pershing, Henrique Teles Maia, Maurizio Chiaramonte, Kevin Carlberg, and Eitan Grinspun.*

1. **MAgNet: Mesh agnostic neural PDE solver.** NIPS , 2022. [paper](https://openreview.net/pdf?id=tbIJmAdqYc8) 

   *Oussama Boussif, Dan Assouline, Loubna Benabbou, and Yoshua Bengio.*

1. **NTopo: Mesh-free topology optimization using implicit neural representations.** NIPS , 2021. [paper](http://crl.ethz.ch/papers/NTopoNeurIPS2021.pdf) 

   *Jonas Zehnder, Yue Li, Stelian Coros, and Bernhard Thomaszewski.*

1. **ContactNets: Learning discontinuous contact dynamics with smooth, implicit representations.** ICLR , 2020. [paper](https://proceedings.mlr.press/v155/pfrommer21a.html) 

   *Samuel Pfrommer, Mathew Halm, and Michael Posa.*

1. **Continuous PDE dynamics forecasting with implicit neural representations.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.14855) 

   *Yuan Yin, Matthieu Kirchmeyer, Jean-Yves Franceschi, Alain Rakotomamonjy, and Patrick Gallinari.*

### [Disentangle](#content)
1. **PDE-driven spatiotemporal disentanglement.** ICLR , 2021. [paper](https://openreview.net/forum?id=vLaHRtHvfFp)

   *Jérémie Donà, Jean-Yves Franceschi, Sylvain Lamprier, and Patrick Gallinari.*

1. **Disentangling physical dynamics from unknown factors for unsupervised video prediction.** CVPR , 2020. [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Le_Guen_Disentangling_Physical_Dynamics_From_Unknown_Factors_for_Unsupervised_Video_Prediction_CVPR_2020_paper.pdf)

   *Vincent Le Guen and Nicolas Thome.*

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

   *Yuyan Chen, Bin Dong, and Jinchao Xu.*

1. **Mosaic flows: A transferable deep learning framework for solving PDEs on unseen domains.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S004578252100668X)

   *Hengjie Wang, Robert Planas, Aparna Chandramowlishwaran, and Ramin Bostanabad.*
   
1. **Meta-learning PINN loss functions.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122001838)

   *Apostolos F Psaros,Kenji Kawaguchi, and George Em Karniadakis.*

1. **HyperPINN: Learning parameterized differential equations with physics-informed hypernetworks.** NIPS, 2021. [paper](https://openreview.net/pdf?id=LxUuRDUhRjM)

   *Filipe de Avila Belbute-Peres, Yi-fan Chen, and Fei Sha.*

1. **Adversarial multi-task learning enhanced physics-informed neural networks for solving partial differential equations.** IJCNN, 2022. [paper](https://ieeexplore.ieee.org/abstract/document/9533606)

   *Pongpisit Thanasutives, Masayuki Numao, and Ken-ichi Fukui.*

1. **Transfer physics informed neural network: A new framework for distributed physics informed neural networks via parameter sharing.** Engineering with Computers, 2022. [paper](https://link.springer.com/article/10.1007/s00366-022-01703-9)

   *Sreehari Manikkan and Balaji Srinivasan.*

1. **Meta-PDE: Learning to solve PDEs quickly without a mesh.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.01604)

   *Tian Qin, Alex Beatson, Deniz Oktay, Nick Mc Greivy, and Ryan P. Adams.*

1. **SVD-PINNs: Transfer learning of physics-informed neural networks via singular value decomposition.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.08760)

   *Yihang Gao, Ka Chun Cheung, and Michael K. Ng.*

1. **Physics-informed neural networks (PINNs) for parameterized PDEs: A meta-learning approach.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13361)

   *Michael Penwarden, Shandian Zhe, Akil Narayan, and Robert M. Kirby.*

1. **Data-driven initialization of deep learning solvers for Hamilton-Jacobi-Bellman PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.09299)

   *Anastasia Borovykh, Dante Kalise, Alexis Laignelet, and Panos Parpas.*

1. **Transfer learning based physics-informed neural networks for solving inverse problems in engineering structures under different loading scenarios.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.07731)

   *Chen Xu, Ba Trung Cao, Yong Yuan, and Günther Meschke.*

### [NAS](#content)
1. **Auto-PINN: Understanding and optimizing physics-informed neural architecture.** arXiv, 2022. [paper](https://arxiv.org/abs/2110.13361)

   *Yicheng Wang, Xiaotian Han, Chia-Yuan Chang, Daochen Zha, Ulisses Braga-Neto, and Xia Hu.*

1. **Building high accuracy emulators for scientific simulations with deep neural architecture search.** Machine Learning: Science and Technology, 2022. [paper](https://iopscience.iop.org/article/10.1088/2632-2153/ac3ffa)

   *M F Kasim, D Watson-Parris, L Deaconu, S Oliver, P Hatfield, D H Froula, G Gregori, M Jarvis, S Khatiwala, J Korenaga, J Topp-Mugglestone, E Viezzer, and S M Vinko.*

1. **Learning operations for neural PDE solvers.** ICLR, 2019. [paper](https://simdl.github.io/files/55.pdf)

   *Nicholas Roberts, Mikhail Khodak, Tri Dao, Liam Li, Christopher Re, and Ameet Talwalkar.*

1. **AutoPINN: When AutoML meets physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04058)

   *Xinle Wu, Dalin Zhang, Miao Zhang, Chenjuan Guo, Shuai Zhao, Yi Zhang, Huai Wang, and Bin Yang.*

### [Sampling](#content)
1. **DMIS: Dynamic mesh-based importance sampling for training physics-informed neural networks.** AAAI, 2023. [paper](https://arxiv.org/abs/2211.13944)

   *Zijiang Yang, Zhongwei Qiu, and Dongmei Fu.*

1. **A comprehensive study of non-adaptive and residual-based adaptive sampling for physics-informed neural networks.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522006260)

   *Chenxi Wua, Min Zhua, Qinyang Tan, YadhKartha, and Lu Lu.*

1. **Mitigating propagation failures in PINNs using evolutionary sampling.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.02338)

   *Arka Daw, Jie Bu, Sifan Wang, Paris Perdikaris, and Anuj Karpatne.*

1. **Residual-quantile adjustment for adaptive training of physics-informed neural network.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.05315)

   *Jiayue Han, Zhiqiang Cai, Zhiyou Wu, and Xiang Zhou.*

1. **Adversarial sampling for solving differential equations with neural networks.** NIPS, 2021. [paper](https://openreview.net/forum?id=EeBH6OZFFx)

   *Kshitij Parwani and Pavlos Protopapas.*

1. **A novel adaptive causal sampling method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.12914)

   *Jia Guo, Haifeng Wang, and Chenping Hou.*

### [Latent Space](#content)
1. **Multiscale simulations of complex systems by learning their effective dynamics.** NMI, 2022. [paper](https://www.nature.com/articles/s42256-022-00464-w)
   
   *Pantelis R. Vlachas, Georgios Arampatzis, Caroline Uhler, and Petros Koumoutsakos.*

1. **A latent space solver for PDE generalization.** ICLR, 2021. [paper](https://arxiv.org/abs/2104.02452)
   
   *Rishikesh Ranade, Chris Hill, Haiyang He, Amir Maleki, and Jay Pathak.*
   
1. **Approximate latent force model inference.** AAAI, 2021. [paper](https://ml4physicalsciences.github.io/2021/files/NeurIPS_ML4PS_2021_78.pdf)
   
   *Jacob D. Moss, Felix L. Opolka, Bianca Dumitrascu, and Pietro Lió.*
   
1. **Learning to accelerate partial differential equations via latent global evolution.** NIPS, 2022. [paper](https://arxiv.org/abs/2206.07681)
   
   *Tailin Wu, Takashi Maruyama, and Jure Leskovec.*
   
1. **Exploring physical latent spaces for deep learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.11298)
   
   *Chloe Paliard, Nils Thuerey, and Kiwon Um.*
   
1. **Certified data-driven physics-informed greedy auto-encoder simulator.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.13698)
   
   *Xiaolong He, Youngsoo Choi, William D. Fries, Jonathan L. Belof, and Jiun-Shyan Chen.*

### [Loss Function](#content)
1. **Adaptive activation functions accelerate convergence in deep and physics-informed neural networks.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119308411)

   *Ameya D.Jagtap, KenjiKawaguchi, and George Em Karniadakis.*

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

1. **Neural basis functions for accelerating solutions to high mach euler equations.** ICML, 2022. [paper](https://openreview.net/forum?id=dvqjD3peY5S)

   *David Witman, Alexander New, Hicham Alkandry, and Honest Mrema.*
   
1. **PFNN-2: A domain decomposed penalty-free neural network method for solving partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.00593)

   *Hailong Shen and Chao Yang.*

1. **Finite basis physics-informed neural networks (FBPINNs): A scalable domain decomposition approach for solving differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2107.07871)

   *Ben Moseley, Andrew Markham, and Tarje Nissen-Meyer.*

1. **Finite basis physics-informed neural networks as a Schwarz domain decomposition method.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.05560)

   *Victorita Dolean, Alexander Heinlein, Siddhartha Mishra, and Ben Moseley.*

1. **NeuralStagger: Accelerating physics constrained neural PDE solver with spatialtemporal decomposition.** ICLR, 2023. [paper](https://openreview.net/forum?id=pGR2gNO5c4p)

   *Anonymous Authors.*

1. **Augmenting physical models with deep networksfor complex dynamics forecasting.** Journal of Statistical Mechanics: Theory and Experiment, 2021. [paper](https://iopscience.iop.org/article/10.1088/1742-5468/ac3ae5/meta)

   *Yuan Yin, Vincent Le Guen, Jérémie Dona, Emmanuel de Bézenac, Ibrahim Ayed, Nicolas Thome, and Patrick Gallinari.*

1. **LordNet: Learning to solve parametric partial differential equations without simulated data.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.09418)

   *Wenlei Shi, Xinquan Huang, Xiaotian Gao, Xinran Wei, Jia Zhang, Jiang Bian, Mao Yang, and Tie-Yan Liu.*

1. **An optimisation–based domain–decomposition reduced order model for the incompressibleNavier-Stokes equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.14528)

   *Ivan Prusak, Monica Nonino, Davide Torlo, Francesco Ballarin, and Gianluigi Rozza.*

### [Mesh](#content)
1. **MeshingNet: A new mesh generation method based on deep learning.** ICCS, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-030-50420-5_14)

   *Zheyan Zhang, Yongxing Wang, Peter K. Jimack, and He Wang.*

1. **M2N: Mesh movement networks for PDE solvers.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.11188)

   *Wenbin Song, Mingrui Zhang, Joseph G. Wallwork, Junpeng Gao, Zheng Tian, Fanglei Sun, Matthew D. Piggott, Junqing Chen, Zuoqiang Shi, Xiang Chen, and Jun Wang.*

1. **RANG: A residual-based adaptive node generation method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.01051)

   *Wei Peng, Weien Zhou, Xiaoya Zhang, Wen Yao, and Zheliang Liu.*

1. **Learning a mesh motion technique with application to fluid-structure interaction and shape optimization.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.02217)

   *Johannes Haubne and Miroslav Kuchta.*

1. **Accelerated training of physics-informed neural networks (PINNs) using meshless discretizations.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.09332)

   *Ramansh Sharma and Varun Shankar.*

1. **An improved structured mesh generation method based on physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.09546)

   *Xinhai Chen, Jie Liu, Junjun Yan, Zhichao Wang, and Chunye Gong.*

1. **Mesh-free Eulerian physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01545)

   *Fabricio Arend Torres, Marcello Massimo Negri, Monika Nagy-Huber, Maxim Samarin, and Volker Roth.*

### [Generative Models](#content)
1. **A framework for data-driven solution and parameter estimation of PDEs using conditional generative adversarial networks.** NCS, 2021. [paper](https://www.nature.com/articles/s43588-021-00171-3)

   *Teeratorn Kadeethum, Daniel O’Malley, Jan Niklas Fuhg, Youngsoo Choi, Jonghyun Lee, Hari S. Viswanathan, and Nikolaos Bouklas.*

1. **Neural SDEs as infinite-dimensional GANs.** ICML, 2021. [paper](http://proceedings.mlr.press/v139/kidger21b.html)

   *Patrick Kidger, James Foster, Xuechen Li, and Terry J Lyons.*

1. **PID-GAN: A GAN framework based on a physics-informed discriminator for uncertainty quantification with physics.** KDD, 2021. [paper](https://dl.acm.org/doi/abs/10.1145/3447548.3467449)

   *Arka Daw, M. Maruf, and Anuj Karpatne.*

1. **Generative adversarial neural operators.** Transactions on Machine Learning Research, 2022. [paper](https://openreview.net/forum?id=X1VzbBU6xZ&referrer=%5BTMLR%5D(%2Fgroup%3Fid%3DTMLR))

   *Md Ashiqur Rahman, Manuel A Florez, Anima Anandkumar, Zachary E Ross, and Kamyar Azizzadenesheli.*

1. **Weak adversarial networks for high-dimensional partial differential equations.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120301832)

   *Yaohua Zang, Gang Bao, Xiaojing Ye, and Haomin Zhou.*

1. **Wasserstein generative adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003321)

   *Yihang Gao and Michael K. Ng.*

1. **Competitive physics informed networks.** ICLR, 2021. [paper](https://openreview.net/forum?id=rMz_scJ6lc)

   *Qi Zeng, Spencer H Bryngelson, and Florian Tobias Schaefer.*

1. **Learning generative neural networks with physics knowledge.** Research in the Mathematical Sciences, 2022. [paper](https://link.springer.com/article/10.1007/s40687-022-00329-z)

   *Kailai Xu, Weiqiang Zhu, and Eric Darve.*

1. **Diffusion generative models in infinite dimensions.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00886)

   *Gavin Kerrigan, Justin Ley, and Padhraic Smyth.*

1. **Revisiting PINNs: Generative adversarial physics-informed neural networks and point-weighting method.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.08754)

   *Wensheng Li, Chao Zhang, Chuncheng Wang, Hanting Guan, and Dacheng Tao.*

1. **PIAT: Physics informed adversarial training for solving partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.06647)

   *Simin Shekarpaz, Mohammad Azizmalayeri, and Mohammad Hossein Rohban.*

1. **Physics-constrained generative adversarial networks for 3D turbulence.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00217)

   *Dima Tretiak, Arvind T. Mohan, and Daniel Livescu.*

### [Gaussian Process](#content)
1. **PAGP: A physics-assisted Gaussian process framework with active learning for forward and inverse problems of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.02583)

   *Jiahao Zhang, Shiqi Zhang, and Guang Lin.*

1. **Solving and learning nonlinear PDEs with Gaussian processes.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005635)

   *Yifan Chen, Bamdad Hosseini, Houman Owhadi, and Andrew M.Stuart.*

1. **Neural-net-induced Gaussian process regression for function approximation and PDE solution.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119301032)

   *Guofei Pang, Liu Yang. and George Em Karniadakis.*

1. **Learning neural optimal interpolation models and solvers.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.07209)

   *Maxime Beauchamp, Joseph Thompson, Hugo Georgenthum, Quentin Febvre, and Ronan Fablet.*

### [Solver](#content)
1. **Solver-in-the-loop: Learning from differentiable physics to interact with iterative PDE-solvers.** NIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496237)

   *Kiwon Um, Robert Brand, Yun (Raymond) Fei, Philipp Holl, and Nils Thuerey.*
   
1. **Lie point symmetry data augmentation for neural PDE solvers.** ICML, 2022. [paper](https://arxiv.org/abs/2202.07643)

   *Johannes Brandstetter, Max Welling, and Daniel E. Worrall.*

1. **Incorporating symmetry into deep dynamics models for improved generalization.** ICLR, 2021. [paper](https://openreview.net/forum?id=wta_8Hx2KD)

   *Rui Wang, Robin Walters, and Rose Yu.*

1. **HyperSolvers: Toward fast continuous-depth models.** NIPS, 2020. [paper](http://www.robot.t.u-tokyo.ac.jp/~yamashita/paper/B/B268Final.pdf)

   *Michael Poli, Stefano Massaroli, Atsushi Yamashita, Hajime Asama, and Jinkyoo Park.*

1. **PIXEL: Physics-informed cell representations for fast and accurate PDE solvers.** NIPS, 2022. [paper](https://openreview.net/forum?id=t49TL3qzma)

   *Namgyu Kang, Byeonghyeon Lee, Youngjoon Hong, Seok-Bae Yun, and Eunbyung Park.*

1. **NeuralSim: Augmenting differentiable simulators with neural networks.** ICRA, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/9560935)

   *Eric Heiden, David Millard, Erwin Coumans, Yizhou Sheng, and Gaurav S. Sukhatme.*

### [Variation](#content) 
1. **PI-VAE: Physics-informed variational auto-encoder for stochastic differential equations.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522006193)

   *Weiheng Zhong and Hadi Meidani.*

1. **Robust SDE-based variational formulations for solving linear pdes via deep learning.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/richter22a.html)

   *Lorenz Richter and Julius Berner.*

1. **hp-VPINNs: Variational physics-informed neural networks with domain decomposition.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520307325)

   *Ehsan Kharazmi, Zhongqiang Zhang, and George Em Karniadakis.*

1. **Variational Onsager neural networks (VONNs): A thermodynamics-based variational learning strategy for non-equilibrium PDEs.** Journal of the Mechanics and Physics of Solids, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0022509622000692)

   *Shenglin Huang, Zequn He, Bryan Chem, and Celia Reina.*

1. **Solving PDEs by variational physics-informed neural networks: A posteriori error analysis.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.00786)

   *Stefano Berrone, Claudio Canuto, and Moreno Pintore.*

1. **Variational Monte Carlo approach to partial differential equations with neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01927)

   *Moritz Reh and Martin Gärttner.*

1. **Energetic variational neural network discretizations to gradient flows.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.07303)

   *Ziqing Hu, Chun Liu, Yiwei Wang, and Zhiliang Xu.*

1. **Variational Bayes deep operator network: A data-driven Bayesian solver for parametric differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.05655)

   *Shailesh Garg and Souvik Chakraborty.*

### [Bayesian](#content)
1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, and George Em Karniadakis.*

1. **Solving inverse problems in stochastic models using deep neural networks and adversarial training.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521003078)

   *Kailai Xu and Eric Darve.*

1. **Bayesian deep learning for partial differential equation parameter discovery with sparse and noisy data.** Journal of Computational Physics: X, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S2590055222000117?via%3Dihub)

   *Christophe Bonneville and Christopher Earls.*

1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, and George Em Karniadakis.*

1. **Approximate Bayesian neural operators: Uncertainty quantification for parametric PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.01565)

   *Emilia Magnani, Nicholas Krämer, Runa Eschenhagen, Lorenzo Rosasco, and Philipp Hennig.*

1. **Bayesian autoencoders for data-driven discovery of coordinates, governing equations and fundamental constants.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.10575)

   *L. Mars Gao and J. Nathan Kutz.*

1. **Bayesian physics informed neural networks for data assimilation and spatio-temporal modelling of wildfires.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00970)

   *Joel Janek Dabrowski, Daniel Edward Pagendam, James Hilton, Conrad Sanderson, Daniel MacKinlay, Carolyn Huston, Andrew Bolt, and Petra Kuhnert.*

### [Lagrangian](#content)
1. **Lagrangian PINNs: A causality–conforming solution to failure modes of physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.02902)

   *Rambod Mojgani, Maciej Balajewicz, and Pedram Hassanzadeh.*

1. **AL-PINNs: Augmented Lagrangian relaxation method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.01059)

   *Hwijae Son, Sung Woong Cho, and Hyung Ju Hwang.*

### [Uncertainty Quantification](#content)
1. **Quantifying total uncertainty in physics-informed neural networks for solving forward and inverse stochastic problems.** arXiv, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119305340)

   *Dongkun Zhang, Lu Lu, Ling Guo, and George Em Karniadakis.*

1. **Adversarial uncertainty quantification in physics-informed neural networks.** Journal of Computational Physics, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303584)

   *Yibo Yang and Paris Perdikaris.*

1. **Conditional Karhunen-Loève expansion for uncertainty quantification and active learning in partial differential equation models.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120303788)

   *Ramakrishna Tipireddy, David A.Barajas-Solano, and Alexandre M.Tartakovsky.*

1. **Physics-constrained deep learning for high-dimensional surrogate modeling and uncertainty quantification without labeled data.** Journal of Computational Physics, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303559)

   *Yinhao Zhu, Nicholas Zabarasa, Phaedon-Stelios Koutsourelakisb, and Paris Perdikaris.*

### [Active Learning](#content)
1. **Neural Galerkin scheme with active learning for high-dimensional evolution equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.01360)

   *Joan Bruna, Benjamin Peherstorfer, and Eric Vanden-Eijnden.*

1. **Discovering and forecasting extreme events via active learning in neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.02488)

   *Pickering, Ethan and Karniadakis, George Em and Sapsis, and Themistoklis P.*

### [Multi Scale](#content)
1. **Hierarchical deep learning of multiscale differential equation time-steppers.** Philosophical Transactions of the Royal Society A, 2022. [paper](https://royalsocietypublishing.org/doi/10.1098/rsta.2021.0200)

   *Yuying Liu, J. Nathan Kutz, and Steven L. Brunton.*

1. **NH-PINN: Neural homogenization-based physics-informed neural network for multiscale problems.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122006015)

   *Wing Tat Leung, Guang Lin, and Zecheng Zhang.*

1. **Deep multiscale model learning.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307764)

   *Yating Wang, Siu Wun Cheung, Eric T.Chung, Yalchin Efendiev, and Min Wang.*

1. **Multi-scale deep neural networks for solving high dimensional PDEs.** arXiv, 2019. [paper](https://www.science.org/doi/10.1126/sciadv.1602614)

   *Samuel H. Rudy, Steven L. Brunton, Joshua L. Proctor, and J. Nathan Kutz.*

1. **Towards multi-spatiotemporal-scale generalized PDE modeling.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.15616)

   *Jayesh K. Gupta and Johannes Brandstetter.*

### [Multi Fidelity](#content)
1. **Multifidelity deep operator networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.09157)

   *Amanda A. Howard, Mauro Perego, George Em Karniadakis, and Panos Stinis.*

1. **Physics and equality constrained artificial neural networks: Application to forward and inverse problems with multi-fidelity data fusion.** Journal of Computational Physics, 2022. [paper](https://dl.acm.org/doi/abs/10.1016/j.jcp.2022.111301)

   *Lulu Zhang, Tao Luo, Yaoyu Zhang, Weinan E, Zhi-Qin John Xu, and Zheng Ma.*

1. **A composite neural network that learns from multi-fidelity data: Application to function approximation and inverse PDE problems.** Journal of Computational Physics, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307260)

   *Xuhui Meng and George Em Karniadakis.*

1. **Multifidelity deep neural operators for efficient learning of partial differential equations with application to fast inverse design of nanoscale heat transport.** Physical Review Research, 2022. [paper](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.4.023210)

   *Lu Lu, Raphaël Pestourie, Steven G. Johnson, and Giuseppe Romano.*

### [Multi Grid](#content)

1. **Learning to optimize multigrid PDE solvers.** ICML, 2019. [paper](http://proceedings.mlr.press/v97/greenfeld19a.html)

   *Daniel Greenfeld, Meirav Galun, Ronen Basri, Irad Yavneh, and Ron Kimmel.*


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

1. **PDE-based optimal strategy for unconstrained online learning.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22d.html)

   *Zhiyu Zhang, Ashok Cutkosky, and Ioannis Paschalidis.*

1. **Control of partial differential equations via physics-informed neural networks.** Journal of Optimization Theory and Applications, 2022. [paper](https://link.springer.com/article/10.1007/s10957-022-02100-4)

   *Carlos J. García-Cervera, Mathieu Kessler, and Francisco Periago.*

1. **A machine learning framework for solving high-dimensional mean field game and mean field control problems.** PNAS, 2020. [paper](https://www.pnas.org/doi/abs/10.1073/pnas.1922204117)

   *Lars Ruthottoa, Stanley J. Osherc, Wuchen Lic, Levon Nurbekyanc, and Samy Wu Fung.*

1. **Bi-level physics-informed neural networks for PDE constrained optimization using Broyden's hypergradients.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.07075)

   *Zhongkai Hao, Chengyang Ying, Hang Su, Jun Zhu, Jian Song, and Ze Cheng.*

1. **A combination technique for optimal control problems constrained by random PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.00499)

   *Fabio Nobile and Tommaso Vanzan.*

1. **A multilevel reinforcement learning framework for PDE-based control.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.08400)

   *Atish Dixit and Ahmed H. Elsheikh.*

1. **Optimal learning of high-dimensional classification problems using deep neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2112.12555)

   *Philipp Petersen and Felix Voigtlaender.*

### [Fluid](#content)
1. **Physics-informed neural networks (PINNs) for fluid mechanics: A review.** Acta Mechanica Sinica, 2021. [paper](https://link.springer.com/article/10.1007/s10409-021-01148-1)

   *Shengze Cai, Zhiping Mao, Zhicheng Wang, Minglang Yin, and George Em Karniadakis.*

1. **Neural operator prediction of linear instability waves in high-speed boundary layers.** Journal of Computational Physics, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122008567)

   *Patricio Clark Di Leoni, Lu Lu, Charles Meneveau, George Karniadakis, and Tamer A. Zaki.*

1. **DiscretizationNet: A machine-learning based solver for Navier–Stokes equations using finite volume discretization.** Computer Methods in Applied Mechanics and Engineering, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S004578252100058X)

   *Rishikesh Ranade, Chris Hillb, and Jay Pathak.*

1. **Surrogate modeling for fluid flows based on physics-constrained deep learning without simulation data.** Computer Methods in Applied Mechanics and Engineering, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S004578251930622X)

   *Luning Sun, Han Gao, Shaowu Pan, and Jianxun Wang.*

1. **Towards physics-informed deep learning for turbulent flow prediction.** KDD, 2020. [paper](https://dl.acm.org/doi/10.1145/3394486.3403198)

   *Rui Wang, Karthik Kashinath, Mustafa Mustafa, Adrian Albert, and Rose Yu.*

1. **Learning to estimate and refine fluid motion with physical dynamics.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22ad/zhang22ad.pdf)

   *Mingrui Zhang, Jianhong Wang, James Tlhomole, and Matthew D. Piggott.*

1. **Physics informed neural fields for smoke reconstruction with sparse data.** ACM Transactions on Graphics, 2022. [paper](https://dl.acm.org/doi/10.1145/3528223.3530169)

   *Mengyu Chu, Lingjie Liu, Quan Zheng, Erik Franz, Hans-Peter Seidel, Christian Theobalt, and Rhaleb Zayer.*

1. **Physics-informed deep learning for traffic state estimation: A hybrid paradigm informed by second-order traffic models.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16132)

   *Rongye Shi, Zhaobin Mo, and Xuan Di.*

1. **Residual-based adaptivity for two-phase flow simulation in porous media using physics-informed neural networks.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S004578252200295X)

   *John M.Hanna, José V.Aguado, Sebastien Comas-Cardona, Ramz Askri, and Domenico Borzacchiello.*

1. **Learned turbulence modelling with differentiable fluid solvers: Physics-based loss-functions and optimisation horizons.** Journal of Fluid Mechanics, 2022. [paper](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/learned-turbulence-modelling-with-differentiable-fluid-solvers-physicsbased-loss-functions-and-optimisation-horizons/28D19239CEDB81A3DA58F32E0E8CB3B2)

   *Björn List, Li-Wei Chen, and Nils Thuerey.*

1. **Multi-scale digital twin: Developing a fast and physics-informed surrogate model for groundwater contamination with uncertain climate models.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.10884)

   *Lijing Wang, Takuya Kurihana, Aurelien Meray, Ilijana Mastilovic, Satyarth Praveen, Zexuan Xu, Milad Memarzadeh, Alexander Lavin, and Haruko Wainwright.*

### [Reconstruction](#content)
1. **Occupancy networks: Learning 3D reconstruction in function space.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mescheder_Occupancy_Networks_Learning_3D_Reconstruction_in_Function_Space_CVPR_2019_paper.pdf)

   *Lars Mescheder, Michael Oechsle, Michael Niemeyer, Sebastian Nowozin, and Andreas Geiger.*
   
1. **Transfer learning for flow reconstruction based on multifidelity data.** AIAA Journal, 2022. [paper](https://arc.aiaa.org/doi/abs/10.2514/1.J061647)

   *Jiaqing Kou , Chenjia Ning, and Weiwei Zhang.*

1. **Learning-based state reconstruction for a scalar hyperbolic PDE under noisy lagrangian sensing.** L4DC, 2022. [paper](http://proceedings.mlr.press/v144/barreau21a.html)

   *Matthieu Barreau, John Liu, and Karl Henrik Johansson.*

### [Physics](#content)
1. **FourCastNet: A global data-driven high-resolution weather model using adaptive Fourier neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.11214)

   *Jaideep Pathak, Shashank Subramanian, Peter Harrington, Sanjeev Raja, Ashesh Chattopadhyay, Morteza Mardani, Thorsten Kurth, David Hall, Zongyi Li, Kamyar Azizzadenesheli, Pedram Hassanzadeh, Karthik Kashinath, and Animashree Anandkumar.*

1. **Dynamic weights enabled physics-informed neural network for simulating the mobility of engineered nano-particles in a contaminated aquifer.** NIPS, 2022. [paper](https://arxiv.org/pdf/2211.03525.pdf)

   *Shikhar Nilabh and Fidel Grandia.*

1. **Spatiotemporal modeling of European paleoclimate using doubly sparse Gaussian processes.** NIPS, 2022. [paper](https://arxiv.org/abs/2211.08160)

   *Seth D. Axen, Alexandra Gessner, Christian Sommer, Nils Weitzel, and Álvaro Tejero-Cantero.*

1. **Learning two-phase microstructure evolution using neural operators and autoencoder architectures.** NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00876-7)

   *Vivek Oommen, Khemraj Shukla, Somdatta Goswami, Rémi Dingreville, and George Em Karniadakis.*

1. **Predicting glass structure by physics-informed machine learning.** NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00882-9)

   *Mikkel L. Bødker, Mathieu Bauchy, Tao Du, John C. Mauro, and Morten M. Smedskjaer.*

1. **Physics-informed deep learning for solving phonon Boltzmann transport equation with large temperature non-equilibrium.** NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00712-y)

   *Ruiyang Li, Jian-Xun Wang, Eungkyu Lee, and Tengfei Luo.*

1. **Bayesian inversion with neural operator (BINO) for modeling subdiffusion: Forward and inverse problems.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.11981)

   *Xiong-bin Yan, Zhi-Qin John Xu, and Zheng Ma.*

1. **Design of Turing systems with physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.13464)

   *Jordon Kho, Winston Koh, Jian Cheng Wong, Pao-Hsiung Chiu, and Chin Chun Ooi.*

1. **Spatio-temporal super-resolution of dynamical systems using physics-informed deep-learning.** AAAI, 2023. [paper](https://arxiv.org/abs/2212.04457)

   *Rajat Arora and Ankit Shrivastava.*

### [Image](#content)
1. **Learning to diffuse: A new perspective to design PDEs for visual analysis.** TPAMI, 2016. [paper](https://ieeexplore.ieee.org/document/7393839)

   *Risheng Liu, Guangyu Zhong, Junjie Cao, Zhouchen Lin, Shiguang Shan, and Zhongxuan Luo.*

1. **Reformulating optical flow to solve image-based inverse problems and quantify uncertainty.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9870569)

   *Aleix Boquet-Pujadas and Jean-Christophe Olivo-Marin.*

1. **WarpPINN: Cine-MR image registration with physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.12549)

   *Pablo Arratia Lopez, Hernan Mella, Sergio Uribe, Daniel E. Hurtado, and Francisco Sahli Costabal.*

1. **Approximating discontinuous Nash equilibria values of two-player general-sum differential games.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.01773)

   *Lei Zhang, Mukesh Ghimire, Wenlong Zhang, Zhe Xu, and Yi Ren.*

### [Mechanics](#content)
1. **Wavelet Neural Operator for solving parametric partial differential equations in computational mechanics problems.** Computer Methods in Applied Mechanics and Engineering, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522007393)

   *TapasTripura and Souvik Chakraborty.*

### [Robotics](#content)
1. **Hybrid learning of time-series inverse dynamics models for locally isotropic robot motion.** RAL, 2022. [paper](https://ieeexplore.ieee.org/document/9954138)

   *Tolga-Can Çallar and Sven Böttger.*

### [Cybernetics](#content)
1. **Machine learning accelerated PDE backstepping observers.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15044)

   *Yuanyuan Shi, Zongyi Li, Huan Yu, Drew Steeves, Anima Anandkumar, and Miroslav Krstic.*

1. **Neural solvers for fast and accurate numerical optimal control.** NIPS, 2021. [paper](https://openreview.net/forum?id=rwMWDGOjaQF)

   *Federico Berto, Stefano Massaroli, Michael Poli, and Jinkyoo Park.*

1. **Bellman neural networks for the class of optimal control problems with integral quadratic cost.** TAI, 2022. [paper](https://ieeexplore.ieee.org/document/9893345)

   *Enrico Schiassi, Andrea D'Ambrosio, and Roberto Furfaro.*

1. **Offline supervised learning vs online direct policy optimization: A comparative study and a unifie training paradigm for neural network-based optimal feedback control.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15930)

   *Yue Zhao and Jiequn Han.*

1. **Policy evaluation and temporal–difference learning in continuous time and space: A martingale approach.** JMLR, 2022. [paper](https://www.jmlr.org/papers/volume23/21-0947/21-0947.pdf)

   *Yanwei Jia and Xun Yu Zhou.*

### [Quantum](#content)
1. **Physics-informed neural networks for quantum eigenvalue problems.** IJCNN, 2022. [paper](https://ieeexplore.ieee.org/document/9891944)

   *Henry Jin, Marios Mattheakis, and Pavlos Protopapas.*

### [Nash Equilibria](#content)
1. **Approximating discontinuous Nash equilibria values of two-player general-sum differential games.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.01773)

   *Lei Zhang, Mukesh Ghimire, Wenlong Zhang, Zhe Xu, and Yi Ren.*

### [Manufacturing](#content)
1. **Physics-aware machine learning surrogates for real-time manufacturing digital twin.** Manufacturing Letters, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S2213846322001845)

   *Aditya Balu, Soumik Sarkar, Baskar Ganapathysubramanian, and Adarsh Krishnamurthy.*

1. **SciAI4Industry--Solving PDEs for industry-scale problems with deep learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.12709)

   *Philipp A. Witte, Russell J. Hewett, Kumar Saurabh, AmirHossein Sojoodi, and Ranveer Chandra.*
