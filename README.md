# Neural-PDE-Solver

PDE: Partial Differentiable Equation

Neural Operators: Learning nonlinear mappings between function spaces.

Contributed by Chunyang Zhang.

## [Content](#content)
<table>
<tr><td colspan="2"><a href="#survey-papers">1. Survey</a></td></tr> 
<tr><td colspan="2"><a href="#model">2. Model</a></td></tr>
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
    <td>&ensp;<a href="#convolution">2.7 Convolution</a></td>
    <td>&ensp;<a href="#autoencoder">2.8 AutoEncoder</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#neural-operator">2.9 Neural Operator</a></td>
	<td>&ensp;<a href="#machine-learning">2.10 Machine Learning</a></td>
<tr>
    <td>&ensp;<a href="#identification">2.11 Identification</a></td>
    <td>&ensp;<a href="#inverse-design">2.12 Inverse Design</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#neural-ode">2.13 Neural ODE</a></td>
    <td>&ensp;<a href="#large-model">2.14 Large Model</a></td>
</tr>
<tr><td colspan="2"><a href="#mechanism">3. Mechanism</a></td></tr>
<tr>
    <td>&ensp;<a href="#benchmark">3.1 Benchmark</a></td>
    <td>&ensp;<a href="#investigation">3.2 Investigation</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#domain-adaptation">3.3 Domain Adaptation</a></td>
    <td>&ensp;<a href="#loss-function">3.4 Loss Function</a></td>
</tr>
<tr> 
    <td>&ensp;<a href="#sampling">3.5 Sampling</a></td>
    <td>&ensp;<a href="#mesh">3.6 Mesh</a></td>
</tr>
<tr> 
    <td>&ensp;<a href="#decomposition">3.7 Decomposition</a></td>
    <td>&ensp;<a href="#disentangle">3.8 Disentangle</a></td>
</tr>
<tr> 
    <td>&ensp;<a href="#solver">3.9 Solver</a></td>
    <td>&ensp;<a href="#automl">3.10 AutoML</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#neural-implicit-flow">3.11 Neural Implicit Flow</a></td>
    <td>&ensp;<a href="#uncertainty-quantification">3.12 Uncertainty Quantification</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#generative-model">3.13 Generative Model</a></td>
    <td>&ensp;<a href="#transformer">3.14 Transformer</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#theory">3.15 Theory</a></td>
    <td>&ensp;<a href="#gaussian-process">3.16 Gaussian Process</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#variation">3.17 Variation</a></td>
    <td>&ensp;<a href="#bayesian">3.18 Bayesian</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#latent-space">3.19 Latent Space</a></td>
    <td>&ensp;<a href="#lagrangian">3.20 Lagrangian</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#multi-scale">3.21 Multi Scale</a></td>
    <td>&ensp;<a href="#multi-fidelity">3.22 Multi Fidelity</a></td>   
</tr>
<tr>
    <td>&ensp;<a href="#multi-grid">3.23 Multi Grid</a></td>
    <td>&ensp;<a href="#active-learning">3.24 Active Learning</a></td>
</tr>
<tr><td colspan="2"><a href="#applications">4. Applications</a></td></tr> 
<tr>
    <td>&ensp;<a href="#optimization">4.1 Optimization</a></td>
    <td>&ensp;<a href="#fluid">4.2 Fluid</a></td>
</tr>
<tr> 
    <td>&ensp;<a href="#cybernetics">4.3 Cybernetics</a></td>
    <td>&ensp;<a href="#climate">4.4 Climate</a></td>
</tr> 
<tr> 
    <td>&ensp;<a href="#mechanics">4.5 Mechanics</a></td>
    <td>&ensp;<a href="#robotics">4.6 Robotics</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#physics">4.7 Physics</a></td>
    <td>&ensp;<a href="#image">4.8 Image</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#chemistry">4.9 Chemistry</a></td>
    <td>&ensp;<a href="#materials">4.10 Materials</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#molecules">4.11 Molecules</a></td>
    <td>&ensp;<a href="#reconstruction">4.12 Reconstruction</a></td>
</tr>  
<tr>
    <td>&ensp;<a href="#quantum">4.13 Quantum</a></td>
    <td>&ensp;<a href="#game-theory">4.14 Game Theory</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#industry">4.15 Industry</a></td>
    <td>&ensp;<a href="#economics">4.16 Economics</a></td>
</tr> 
</table>


## [Survey Papers](#content)
1. **Physics-informed machine learning.** Nature Reviews Physics, 2021. [paper](https://www.nature.com/articles/s42254-021-00314-5)

   *George Em Karniadakis, Ioannis G. Kevrekidis, Lu Lu, Paris Perdikaris, Sifan Wang, and Liu Yang.*

1. **Neural operator: Learning maps between function spaces.** JMLR, 2023. [paper](https://www.jmlr.org/papers/v24/21-1524.html)

   *Nikola Kovachki, Zongyi Li, Burigede Liu, Kamyar Azizzadenesheli, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Physics-informed machine learning approach for augmenting turbulence models: A comprehensive framework.** Physical Review Fluids, 2018. [paper](https://journals.aps.org/prfluids/abstract/10.1103/PhysRevFluids.3.074602)

   *Jinlong Wu, Heng Xiao, and Eric Paterson.* 

1. **Integrating scientific knowledge with machine learning for engineering and environmental systems.** ACM Computing Surveys, 2023. [paper](https://dl.acm.org/doi/full/10.1145/3514228)

   *Jared Willard, Xiaowei Jia, Shaoming Xu, Michael Steinbach, and Vipin Kumar.* 

1. **Physical laws meet machine intelligence: Current developments and future directions.** Artificial Intelligence Review, 2022. [paper](https://link.springer.com/article/10.1007/s10462-022-10329-8)

   *Temoor Muther, Amirmasoud Kalantari Dahaghi, Fahad Iqbal Syed, and Vuong Van Pham.* 

1. **A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001207?via%3Dihub)

   *Lu Lu, Xuhui Meng, Shengze Cai, Zhiping Mao, Somdatta Goswami, Zhongqiang Zhang, and George Em Karniadakis.* 

1. **Scientific machine learning through physics–informed neural networks: Where we are and what’s next.** Beyond Traditional AI: The Impact of Machine Learning on Scientific Computing, 2022. [book](https://link.springer.com/article/10.1007/s10915-022-01939-z)

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

1. **Solving differential equations with deep learning: A beginner's guide.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.11237)

   *Luis Medrano Navarro, Luis Martín Moreno, and Sergio G Rodrigo.* 

1. **Deep learning algorithms for solving differential equations: A survey.** Journal of Experimental & Theoretical Artificial Intelligence, 2023. [paper](https://www.tandfonline.com/doi/abs/10.1080/0952813X.2023.2242356)

   *Harender Kumara and Neha Yadav.* 

1. **An expert's guide to training physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.08468)

   *Sifan Wang, Shyam Sankaran, Hanwen Wang, and Paris Perdikaris.* 

1. **A survey on physics informed reinforcement learning: Review and open problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.01909)

   *Chayan Banerjee, Kien Nguyen, Clinton Fookes, and Maziar Raissi.* 

1. **Machine learning and domain decomposition methods -- A survey.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.14050)

   *Axel Klawonn, Martin Lanser, and Janine Weber.* 

1. **The transformative potential of machine learning for experiments in fluid mechanics.** Nature Reviews Physics, 2023. [paper](https://www.nature.com/articles/s42254-023-00622-y)

   *Ricardo Vinuesa, Steven L. Brunton, and Beverley J. McKeon.* 

1. **Physics-informed machine learning for reliability and systems safety applications: State of the art and challenges.** Reliability Engineering & System Safety, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0951832022005154)

   *Yanwen Xu, Sara Kohtz, Jessica Boakye, Paolo Gardoni, and Pingfeng Wang.* 

1. **Operator learning: Algorithms and analysis.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15715)

   *Nikola B. Kovachki, Samuel Lanthaler, and Andrew M. Stuart.* 

1. **Neural operators for accelerating scientific simulations and design.** Nature Reviews Physics, 2024. [paper](https://www.nature.com/articles/s42254-024-00712-5)

   *Kamyar Azizzadenesheli, Nikola Kovachki, Zongyi Li, Miguel Liu-Schiaffini, Jean Kossaifi, and Anima Anandkumar.* 

1. **Learning dynamical systems from data: An introduction to physics-guided deep learning.** PNAS, 2024. [paper](https://www.pnas.org/doi/10.1073/pnas.2311808121)

   *Rose Yu and Rui Wang.* 


## [Model](#content) 
### [PINN](#content)
1. **Hidden fluid mechanics: Learning velocity and pressure fields from flow visualizations.** Science, 2020. [paper](https://www.science.org/doi/10.1126/science.aaw4741)

   *Raissi Maziar, Alireza Yazdani, and George Em Karniadakis.*

1. **Deep hidden physics models: Deep learning of nonlinear partial differential equations.** JMLR, 2018. [paper](https://www.jmlr.org/papers/volume19/18-046/18-046.pdf)

   *Maziar Raissi.*

1. **A universal PINNs method for solving partial differential equations with a point source.** IJCAI, 2022. [paper](https://www.ijcai.org/proceedings/2022/533)

   *Xiang Huang, Hongsheng Liu, Beiji Shi, Zidong Wang, Kang Yang, Yang Li, Min Wang, Haotian Chu, Jing Zhou, Fan Yu, Bei Hua, Bin Dong, and Lei Chen.*

1. **Parallel physics-informed neural networks via domain decomposition.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005787)

   *Khemraj Shukla, Ameya D.Jagtap, and George Em Karniadakis.*

1. **Kolmogorov n–width and Lagrangian physics-informed neural networks: A causality-conforming manifold for convection-dominated PDEs.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522007666)

   *Rambod Mojgani, Maciej Balajewicz, and Pedram Hassanzadeh.*

1. **Exact imposition of boundary conditions with distance functions in physics-informed deep neural networks.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521006186)

   *N.Sukumar and Ankit Srivastava.*

1. **Physics-informed multi-LSTM networks for meta-modeling of nonlinear structures.** CMAME, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520304114)

   *Ruiyang Zhang, Yang Liu, and Hao Sun.*

1. **Gradient-enhanced physics-informed neural networks for forward and inverse PDE problems.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522001438)

   *Jeremy Yu, Lu Lu, Xuhui Meng, and George Em Karniadakis.*

1. **Multi-output physics-informed neural networks for forward and inverse PDE problems with uncertainties.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522002602)

   *MingyuanYang and John T.Foster*

1. **PPINN: Parareal physics-informed neural network for time-dependent PDEs.** CMAME, 2020. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782520304357)

   *Xuhui Meng, Zhen Li, Dongkun Zhang, and George Em Karniadakis.*

1. **CAN-PINN: A fast physics-informed neural network based on coupled-automatic–numerical differentiation method.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522001906)

   *Pao-Hsiung Chiu, Jian Cheng Wong, Chinchun Ooi, My Ha Dao, and Yew-Soon Ong.*

1. **Derivative-informed projected neural networks for high-dimensional parametric maps governed by PDEs.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521005302)

   *Thomas O’Leary-Roseberry, Umberto Villa, Peng Chen, and Omar Ghattas.*

1. **Physics-augmented learning: A new paradigm beyond physics-informed learning.** NIPS, 2021. [paper](https://www.iamwawa.cn/daxiaoxie.html)

   *Ziming Liu, Yuanqi Du, Yunyue Chen, and Max Tegmark.*

1. **Data-driven vector soliton solutions of coupled nonlinear Schrödinger equation using a deep learning algorithm.** Physics Letters A, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0375960121006034)

   *Yifan Mo, Liming Ling, and Delu Zeng.*

1. **Solving Benjamin–Ono equation via gradient balanced PINNs approach.** The European Physical Journal Plus, 2022. [paper](https://link.springer.com/article/10.1140/epjp/s13360-022-03078-8)

   *Xiangyu Yang and Zhen Wang.*

1. **Robust learning of physics informed neural networks.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13330)

   *Chandrajit Bajaj, Luke McLennan, Timothy Andeen, and Avik Roy.*

1. **Learning physics-informed neural networks without stacked back-propagation.** AISTATS, 2023. [paper](https://proceedings.mlr.press/v206/he23a.html)

   *Di He, Wenlei Shi, Shanda Li, Xiaotian Gao, Jia Zhang, Jiang Bian, Liwei Wang, and Tieyan Liu.*

1. **NeuralPDE: Automating physics-informed neural networks (PINNs) with error approximations.** arXiv, 2021. [paper](https://arxiv.org/abs/2107.09443)

   *Kirill Zubov, Zoe McCarthy, Yingbo Ma, Francesco Calisto, Valerio Pagliarino, Simone Azeglio, Luca Bottero, Emmanuel Luján, Valentin Sulzer, Ashutosh Bharambe, Nand Vinchhi, Kaushik Balakrishnan, Devesh Upadhyay, and Chris Rackauckas.*

1. **Physics informed RNN-DCT networks for time-dependent partial differential equations.** ICCS, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-08754-7_45)

   *Benjamin Wu, Oliver Hennigh, Jan Kautz, Sanjay Choudhry, and Wonmin Byeon.*

1. **Theory-guided physics-informed neural networks for boundary layer problems with singular perturbation.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122008312)

   *Amirhossein Arzani, Kevin W.Cassel, and Roshan M.D'Souza.*

1. **A-PINN: Auxiliary physics informed neural networks for forward and inverse problems of nonlinear integro-differential equations.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003229)

   *Lei Yuan, Yiqing Ni, Xiangyun Deng, and Shuo Hao.*

1. **A mixed formulation for physics-informed neural networks as a potential solver for engineering problems in heterogeneous domains: Comparison with finite element method.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522005722)

   *Shahed Rezaei, Ali Harandi, Ahmad Moeineddin, Baixiang Xua, and Stefanie Reese.*

1. **Physics-informed neural networks combined with polynomial interpolation to solve nonlinear partial differential equations.** Computers & Mathematics with Applications, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0898122122005090)

   *Siping Tang, Xinlong Feng, Wei Wu, and Hui Xu.*

1. **A novel sequential method to train physics informed neural networks for Allen Cahn and Cahn Hilliard equations.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521006939)

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

1. **Physics-informed neural networks for operator equations with stochastic data.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.10344)

   *Paul Escapil-Inchauspé and Gonzalo A. Ruz.*

1. **Physics-informed neural networks with unknown measurement noise.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15498)

   *Philipp Pilar and Niklas Wahlstrom.*

1. **On the compatibility between a neural network and a partial differential equation for physics-informed learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00270)

   *Kuangdai Leng and Jeyan Thiyagalingam.*

1. **Pre-training strategy for solving evolution equations based on physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00798)

   *Jiawei Guo, Yanzhong Yao, Han Wang, and Tongxiang Gu.*

1. **L-HYDRA: Multi-head physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.02152)

   *Zongren Zou and George Em Karniadakis.*

1. **PINN for dynamical partial differential equations is not training deeper networks rather learning advection and time variance.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.04793)

   *Siddharth Rout.*

1. **Wavelets based physics informed neural networks to solve non-linear differential equations.** Scientific Reports, 2023. [paper](https://www.nature.com/articles/s41598-023-29806-3)

   *Ziya Uddin, Sai Ganga, Rishi Asthana, and Wubshet Ibrahim.*

1. **Improved training of physics-informed neural networks using energy-based priors: A study on electrical impedance tomography.** ICLR, 2023. [paper](https://openreview.net/forum?id=zqkfJA6R1-r)

   *Akarsh Pokkunuru, Pedram Rooshenas, Thilo Strauss, Anuj Abhishek, and Taufiquar Khan.*

1. **Adaptive weighting of Bayesian physics informed neural networks for multitask and multiscale forward and inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.12697)

   *Sarah Perez, Suryanarayana Maddu, Ivo F. Sbalzarini, and Philippe Poncet.*

1. **Efficient physics-informed neural networks using hash encoding.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.13397)

   *Xinquan Huang and Tariq Alkhalifah.*

1. **Ensemble learning for physics informed neural networks: A gradient boosting approach.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.13143)

   *Zhiwei Fang, Sifan Wang, and Paris Perdikaris.*

1. **On the limitations of physics-informed deep learning: Illustrations using first order hyperbolic conservation law-based traffic flow models.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.12337)

   *Archie J. Huang and Shaurya Agarwal.*

1. **Achieving high accuracy with PINNs via energy natural gradients.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.13163)

   *Johannes Müller and Marius Zeinhofer.*

1. **Implicit stochastic gradient descent for training physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.01767)

   *Ye Li, Songcan Chen, and Shengjun Huang.*

1. **NSGA-PINN: A multi-objective optimization method for physics-informed neural network training.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.02219)

   *Binghang Lu, Christian B. Moya, and Guang Lin.*

1. **Improving physics-informed neural networks with meta-learned optimization.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.07127)

   *Alex Bihlo.*

1. **MetaPhysiCa: OOD robustness in physics-informed machine learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.03181)

   *S Chandra Mouli, Muhammad Ashraful Alam, and Bruno Ribeiro.*

1. **HomPINNs: Homotopy physics-informed neural networks for solving the inverse problems of nonlinear differential equations with multiple solutions.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.02811)

   *Haoyang Zheng, Yao Huang, Ziyang Huang, Wenrui Hao, and Guang Lin.*

1. **iPINNs: Incremental learning for physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.04854)

   *Aleksandr Dekhovich, Marcel H.F. Sluiter, David M.J. Tax, and Miguel A. Bessa.*

1. **Global convergence of deep Galerkin and PINNs methods for solving partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.06000)

   *Francisco Eiras, Adel Bibi, Rudy Bunel, Krishnamurthy Dj Dvijotham, Philip Torr, and M. Pawan Kumar.*

1. **Provably correct physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.10157)

   *Deqing Jiang, Justin Sirignano, and Samuel N. Cohen.*

1. **Predictive limitations of physics-informed neural networks in vortex shedding.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.00230)

   *Pi-Yueh Chuang and Lorena A. Barba.*

1. **Residual-based error bound for physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.03786)

   *Shuheng Liu, Xiyue Huang, and Pavlos Protopapas.*

1. **Automatic boundary fitting framework of boundary dependent physics-informed neural network solving partial differential equation with complex boundary conditions.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523002633)

   *Yuchen Xie, Yu Ma, and Yahui Wang.*

1. **Solving a class of multi-scale elliptic PDEs by means of Fourier-based mixed physics informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.13385)

   *Xi'an Li, Jinran Wu, Zhi-Qin John Xu, and You-Gan Wang.*

1. **Separable physics informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.15969)

   *Junwoo Cho, Seungtae Nam, Hyunmo Yang, Seok-Bae Yun, Youngjoon Hong, and Eunbyung Park.*

1. **Achieving high accuracy with PINNs via energy natural gradient descent.** ICML, 2023. [paper](https://openreview.net/forum?id=y6sCx3eJpw)

   *Johannes Müller and Marius Zeinhofer.*

1. **Gradient descent finds the global optima of two-layer physics-informed neural networks.** ICML, 2023. [paper](https://openreview.net/forum?id=DRMh8mVEav)

   *Yihang Gao, Yiqi Gu, and Michael Ng.*

1. **Residual-based attention in physics-informed neural networks.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524000616)

   *Sokratis J. Anagnostopoulos, Juan Diego Toscano, Nikolaos Stergiopulos, and George Em Karniadakis.*

1. **Auxiliary-tasks learning for physics-informed neural network-based partial differential equations solving.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.06167)

   *Junjun Yan, Xinhai Chen, Zhichao Wang, Enqiang Zhou, and Jie Liu.*

1. **Tackling the curse of dimensionality with physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.12306)

   *Zheyuan Hu, Khemraj Shukla, George Em Karniadakis, and Kenji Kawaguchi.*

1. **Solving PDEs on spheres with physics-informed convolutional neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.09605)

   *Guanhang Lei, Zhen Lei, Lei Shi, Chenyu Zeng, and Dingxuan Zhou.*

1. **Solving PDEs on spheres with physics-informed convolutional neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.09605)

   *Guanhang Lei, Zhen Lei, Lei Shi, Chenyu Zeng, and Dingxuan Zhou.*

1. **Tensor-compressed back-propagation-free training for (physics-informed) neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.09858)

   *Yequan Zhao, Xinling Yu, Zhixiong Chen, Ziyue Liu, Sijia Liu, and Zheng Zhang.*

1. **How to select physics-informed neural networks in the absence of ground truth: A pareto front-based strategy.** ICML, 2023. [paper](https://openreview.net/pdf?id=i3Hjq9Wcvq)

   *Zhao Wei, Jian Cheng Wong, Nicholas Wei Yong Sung, Abhishek Gupta, Chin Chun Ooi, Pao-Hsiung Chiu, My Ha Dao, and Yew-Soon Ong.*

1. **A gradient-enhanced physics-informed neural network (gPINN) scheme for the coupled non-fickian/non-fourierian diffusion-thermoelasticity analysis: A novel gPINN structure.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623010928)

   *Katayoun Eshkofti and Seyed Mahmoud Hosseini.*

1. **Learning only on boundaries: A physics-informed neural operator for solving parametric partial differential equations in complex geometries.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.12939)

   *Zhiwei Fang, Sifan Wang, and Paris Perdikaris.*

1. **Exact and soft boundary conditions in physics-informed neural networks for the variable coefficient poisson equation.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.02548)

   *Sebastian Barschkis.*

1. **Investigating the ability of PINNs to solve burgers’ PDE near finite-time blowup.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.05169)

   *Dibyakanti Kumar and Anirbit Mukherjee.*

1. **Correcting model misspecification in physics-informed neural networks (PINNs).** arXiv, 2023. [paper](https://arxiv.org/abs/2310.10776)

   *Zongren Zou, Xuhui Meng, and George Em Karniadakis.*

1. **On residual minimization for PDEs: Failure of PINN, modified equation, and implicit bias.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.18201)

   *Tao Luo and Qixuan Zhou.*

1. **Operator learning enhanced physics-informed neural networks for solving partial differential equations characterized by sharp solutions.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.19590)

   *Bin Lin, Zhiping Mao, Zhicheng Wang, and George Em Karniadakis.*

1. **PINNs-TF2: Fast and user-friendly physics-informed neural networks in TensorFlow V2.** NIPS, 2023. [paper](https://arxiv.org/abs/2311.03626)

   *Reza Akbarian Bafghi and Maziar Raissi.*

1. **Filtered partial differential equations: A robust surrogate constraint in physics-informed deep learning framework.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.03776)

   *Dashan Zhang, Yuntian Chen, and Shiyi Chen.*

1. **Enhanced physics-informed neural networks with domain scaling and residual correction methods for multi-frequency elliptic problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.03746)

   *Deok-Kyu Jang, Hyea Hyun Kim, and Kyungsoo Kim.*

1. **Physics-informed neural networks for transformed geometries and manifolds.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.15940)

   *Samuel Burbulla.*

   *Zheyuan Hu, Zhouhao Yang, Yezhen Wang, George Em Karniadakis, and Kenji Kawaguchi.*

1. **Neuro-PINN: A hybrid framework for efficient nonlinear projection equation solutions.** The International Journal for Numerical Methods in Engineering, 2023. [paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/nme.7377)

   *Dawen Wu and Abdel Lisser.*

1. **Exactly conservative physics-informed neural networks and deep operator networks for dynamical systems.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.14131)

   *Elsa Cardoso-Bihlo and Alex Bihlo.*

1. **Semi-analytic PINN methods for boundary layer problems in a rectangular domain.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.06278)

   *Gungmin Gie, Youngjoon Hong, Chang-Yeol Jung, and Tselmuun Munkhjin.*

1. **PICL: Physics informed contrastive learning for partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.16327)

   *Cooper Lorsung and Amir Barati Farimani.*

1. **Fourier warm start for physics-informed neural networks.** EAAI, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197624000459)

   *Ge Jin, Jian Cheng Wong, Abhishek Gupta, Shipeng Li, and Yew-Soon Ong.*

1. **Preconditioning for physics-informed neural networks.** ICML, 2024. [paper](https://openreview.net/forum?id=2C3CWCPxNS)

   *Songming Liu, Chang Su, Jiachen Yao, Zhongkai Hao, Hang Su, Youjia Wu, and Jun Zhu.*

1. **RBF-PINN: Non-Fourier positional embedding in physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.08367)

   *Chengxi Zeng, Tilo Burghardt, and Alberto M Gambaruto.*

1. **Training dynamics in physics-informed neural networks with feature mapping.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.06955)

   *Chengxi Zeng, Tilo Burghardt, and Alberto M Gambaruto.*

1. **Score-based physics-informed neural networks for high-dimensional Fokker-Planck equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.07465)

   *Zheyuan Hu, Zhongqiang Zhang, George Em Karniadakis, and Kenji Kawaguchi.*

1. **Investigation of compressor cascade flow using physics-informed neural networks with adaptive learning strategy.** AIAA Journal, 2024. [paper](https://arc.aiaa.org/doi/full/10.2514/1.J063562)

   *Zhihui Li, Francesco Montomoli, and Sanjiv Sharma.*

1. **Exact enforcement of temporal continuity in sequential physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.03223)

   *Pratanu Roy and Stephen Castonguay.*

1. **Multiple scattering simulation via physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.04094v1)

   *Siddharth Nair, Timothy F. Walsh, Greg Pickrell, and Fabio Semperlotti.*

1. **Toward a better understanding of Fourier neural operators: Analysis and improvement from a spectral perspective.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.07200)

   *Shaoxiang Qin, Fuyuan Lyu, Wenhui Peng, Dingyang Geng, Ju Wang, Naiping Gao, Xue Liu, and Liangzhu Leon Wang.*

1. **Anti-derivatives approximator for enhancing physics-informed neural networks.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524002561)

   *Jeongsu Lee.*

1. **GMC-PINNs: A new general Monte Carlo PINNs methodfor solving fractional partial differential equations on irregular domains.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.00217)

   *Shupeng Wang and George Em Karniadakis.*

1. **CEENs: Causality-enforced evolutional networks for solving time-dependent partial differential equations.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524002925)

   *Jeahan Jung, Heechang Kim, Hyomin Shin, and Minseok Choi.*

1. **PTPI-DL-ROMs: Pre-trained physics-informed deep learning-based reduced order models for nonlinear parametrized PDEs.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.08558)

   *Simone Brivio, Stefania Fresca, and Andrea Manzoni.*

1. **Closed-form symbolic solutions: A new perspective on solving partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.14620)

   *Shu Wei, Yanjie Li, Lina Yu, Min Wu, Weijun Li, Meilan Hao, Wenqiang Li, Jingyi Liu, and Yusong Deng.*

1. **RoPINN: Region optimized physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.14369)

   *Haixu Wu, Huakun Luo, Yuezhou Ma, Jianmin Wang, and Mingsheng Long.*

1. **Interface PINNs (I-PINNs): A physics-informed neural networks framework for interface problems.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S0045782524003918)

   *Antareep Kumar Sarma, Sumanta Roy, Chandrasekhar Annavarapu, Pratanu Roy, and Shriram Jagannathan.*

1. **Parameterized physics-informed neural networks for parameterized PDEs.** ICML, 2024. [paper](https://openreview.net/forum?id=n3yYrtt9U7)

   *Woojin Cho, Minju Jo, Haksoo Lim, Kookjin Lee, Dongeun Lee, Sanghyun Hong, and Noseong Park.*

### [DeepONet](#content)
1. **Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators.** NMI, 2021. [paper](https://www.nature.com/articles/s42256-021-00302-5)

   *Lu Lu, Pengzhan Jin, Guofei Pang, Zhongqiang Zhang, and George Em Karniadakis.*

1. **Learning the solution operator of parametric partial differential equations with physics-informed DeepONets.** SA, 2021. [paper](https://www.science.org/doi/10.1126/sciadv.abi8605)

   *Wang Sifan, Hanwen Wang, and Paris Perdikaris.*

1. **Deep transfer operator learning for partial differential equations under conditional shift.** NMI, 2022. [paper](https://www.nature.com/articles/s42256-022-00569-2) 

   *Somdatta Goswami, Katiana Kontolati, Michael D. Shields, and George Em Karniadakis.*

1. **Variable-input deep operator networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.11404)

   *Michael Prasthofer, Tim De Ryck, and Siddhartha Mishra.*

1. **MIONet: Learning multiple-input operators via tensor product.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.06137)

   *Jeremy Yu, Lu Lu, Xuhui Meng, and George Em Karniadakis.*

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

1. **MultiAuto-DeepONet: A multi-resolution autoencoder DeepONet for nonlinear dimension reduction, uncertainty quantification and operator learning of forward and inverse stochastic problems.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.03193)

   *Jiahao Zhang, Shiqi Zhang, and Guang Lin.*

1. **Transfer learning enhanced DeepONet for long-time prediction of evolution equations.** AAAI, 2023. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/26262)

   *Wuzhe Xu, Yulong Lu, and Li Wang.*

1. **B-DeepONet: An enhanced Bayesian DeepONet for solving noisy parametric PDEs using accelerated replica exchange SGLD.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122007768)

   *Guang Lin, Christian Moy, and Zecheng Zhang.*

1. **VB-DeepONet: A Bayesian operator learning framework for uncertainty quantification.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0952197622006753)

   *Shailesh Garg and Souvik Chakraborty.*

1. **Sequential deep learning operator network (S-DeepONet) for time-dependent loads.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.08218)

   *Jaewan Park, Shashank Kushwaha, Junyan He, Seid Koric, Diab Abueidda, and Iwona Jasiuk.*

1. **Asymptotic-preserving convolutional DeepONets capture the diffusive behavior of the multiscale linear transport equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.15891)

   *Keke Wu, Xiong-bin Yan, Shi Jin, and Zheng Ma.*

1. **A hybrid decoder-DeepONet operator regression framework for unaligned observation data.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.09274)

   *Bo Chen, Chenyu Wang, Weipeng Li, and Haiyang Fu.*

1. **Improving physics-informed DeepONets with hard constraints.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.07899)

   *Rüdiger Brecht, Dmytro R. Popovych, Alex Bihlo, and Roman O. Popovych.*

1. **Capturing the diffusive behavior of the multiscale linear transport equations by asymptotic-preserving convolutional DeepONets.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782523006552)

   *Keke Wu, Xiong-Bin Yan, Shi Jin, and Zheng Ma.*

1. **DON-LSTM: Multi-resolution learning with DeepONets and long short-term memory neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.02491)

   *Katarzyna Michałowska, Somdatta Goswami, George Em Karniadakis, and Signe Riemer-Sørensen.*

1. **DeepOnet based preconditioning strategies for solving parametric linear systems of equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.02016)

   *Alena Kopaničáková and George Em Karniadakis.*

1. **Derivative-enhanced deep operator network.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.19242)

   *Yuan Qiu, Nolan Bridges, and Peng Chen.*

1. **Ensemble and mixture-of-experts DeepONets for operator learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.11907)

   *Ramansh Sharma and Varun Shankar.*

1. **Learning nonlinear operators in latent spaces for real-time predictions of complex dynamics in physical systems.** NC, 2024. [paper](https://www.nature.com/articles/s41467-024-49411-w)

   *Katiana Kontolati, Somdatta Goswami, George Em Karniadakis, and Michael D. Shields.*

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

1. **Multipole graph neural operator for parametric partial differential equations.** NIPS, 2020. [paper](https://dl.acm.org/doi/abs/10.5555/3495724.3496291)

   *Zongyi Li, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar.*

1. **Fast sampling of diffusion models via operator learning.** ICML, 2023. [paper](https://proceedings.mlr.press/v202/zheng23d.html)

   *Hongkai Zheng, Weili Nie, Arash Vahdat, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Factorized Fourier neural operators.** ICLR, 2023. [paper](https://openreview.net/forum?id=tmIiMPl4IPa)

   *Alasdair Tran, Alexander Mathews, Lexing Xie, and Cheng Soon Ong.*

1. **Model inversion for spatio-temporal processes using the Fourier neural operator.** NIPS, 2023. [paper](https://ml4physicalsciences.github.io/2021/files/NeurIPS_ML4PS_2021_8.pdf)

   *Dan MacKinlay, Dan Pagendam, Petra M. Kuhnert, Tao Cui, David Robertson, and Sreekanth Janardhanan.*

1. **Learning deep implicit Fourier neural operators (IFNOs) with applications to heterogeneous material modeling.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522004078)

   *Huaiqian You, Quinn Zhang, Colton J. Ross, Chung-Hao Lee, and Yue Yu.*

1. **On the eigenvector bias of Fourier feature networks: From regression to solving multi-scale PDEs with physics-informed neural networks.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521002759)

   *Sifan Wang, Hanwen Wang, and Paris Perdikaris.*

1. **Semi-supervised learning of partial differential operators and dynamical flows.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.14366)

   *Michael Rotman, Amit Dekel, Ran Ilan Ber, Lior Wolf, and Yaron Oz.*

1. **Non-equispaced Fourier neural solvers for PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04689)

   *Haitao Lin, Lirong Wu, Yongjie Xu, Yufei Huang, Siyuan Li, Guojiang Zhao, Stan Z, and Li Cari.*

1. **Incremental spectral learning Fourier neural operator.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15188)

   *Jiawei Zhao, Robert Joseph George, Yifei Zhang, Zongyi Li, and Anima Anandkumar.*

1. **Fourier continuation for exact derivative computation in physics-informed neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.15960)

   *Haydn Maust, Zongyi Li, Yixuan Wang, Daniel Leibovici, Oscar Bruno, Thomas Hou, and Anima Anandkumar.*

1. **Non-equispaced Fourier neural solvers for PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2212.04689)

   *Haitao Lin, Lirong Wu, Yongjie Xu, Yufei Huang, Siyuan Li, Guojiang Zhao, Stan Z, and Li Cari.*

1. **Learning-based solutions to nonlinear hyperbolic PDEs: Empirical insights on generalization errors.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.08144)

   *Bilal Thonnam Thodi, Sai Venkata Ramana Ambadipudi, and Saif Eddin Jabari.*

1. **Domain agnostic Fourier neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.00478)

   *Ning Liu, Siavash Jafarzadeh, and Yue Yu.*

1. **Spherical Fourier neural operators: Learning stable dynamics on the sphere.** ICML, 2023. [paper](https://arxiv.org/abs/2306.03838)

   *Boris Bonev, Thorsten Kurth, Christian Hundt, Jaideep Pathak, Maximilian Baust, Karthik Kashinath, and Anima Anandkumar.*

1. **Group equivariant Fourier neural operators for partial differential equations.** ICML, 2023. [paper](https://openreview.net/forum?id=kgAOY5x4fi)

   *Jacob Helwig, Xuan Zhang, Cong Fu, Jerry Kurtin, Stephan Wojtowytsch, and Shuiwang Ji.*

1. **Speeding up Fourier neural operators via mixed precision.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.15034)

   *Colin White, Renbo Tu, Jean Kossaifi, Gennady Pekhimenko, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Geometry-informed neural operator for large-scale 3D PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.00583)

   *Zongyi Li, Nikola Borislavov Kovachki, Chris Choy, Boyi Li, Jean Kossaifi, Shourya Prakash Otta, Mohammad Amin Nabian, Maximilian Stadler, Christian Hundt, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Deep equilibrium based neural operators for steady-state PDEs.** NIPS, 2023. [paper](https://openreview.net/forum?id=FzXsSCF50t)

   *Tanya Marwah, Ashwini Pokle, J Zico Kolter, Zachary Chase Lipton, Jianfeng Lu, and Andrej Risteski.*

1. **A born fourier neural operator for solving Poisson’s equation with limited data and arbitrary domain deformation.** TAP, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10352090)

   *Zheng Zong, Yusong Wang, Siyuan He, and Zhun Wei.*

1. **Approximating numerical flux by Fourier neural operators for the hyperbolic conservation laws.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.01783)

   *Taeyoung Kim and Myungjoo Sang.*

1. **Invertible Fourier neural operators for tackling both forward and inverse problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.11722)

   *Da Long and Shandian Zhe.*

1. **An operator learning perspective on parameter-to-observable maps.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.06031v1)

   *Daniel Zhengyu Huang, Nicholas H. Nelsen, and Margaret Trautner.*

1. **Learning the boundary-to-domain mapping using lifting product Fourier neural operators for partial differential equations.** ICML, 2024. [paper](https://arxiv.org/abs/2406.16740)

   *Aditya Kashi, Arka Daw, Muralikrishnan Gopalakrishnan Meena, and Hao Lu.*

1. **Accelerating phase field simulations through a hybrid adaptive fourier neural operator with U-net backbone.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.17119)

   *Christophe Bonneville, Nathan Bieberdorf, Arun Hegde, Mark Asta, Habib N. Najm, Laurent Capolungo, and Cosmin Safta.*

1. **Gabor-filtered Fourier neural operator for solving partial differential equations.** Computers & Fluids, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045793024000719)

   *Kai Qi and Jian Sun.*

1. **Component Fourier neural operator for singularly perturbed differential equations.** AAAI, 2024. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/29274)

   *Ye Li, Ting Du, Yiwen Pang, and Zhongyi Huang.*

### [Graph Network](#content)
1. **Message passing neural PDE solvers.** ICLR, 2022. [paper](https://openreview.net/forum?id=vSix3HPYKSU)

   *Johannes Brandstetter, Daniel E. Worrall, and Max Welling.*

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR, 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP)

   *Xu Han, Han Gao, Tobias Pfaff, Jianxun Wang, and Liping Liu.*

1. **Learning mesh-based simulation with graph networks.** ICLR, 2021. [paper](https://openreview.net/forum?id=roNqYL0_XP)

   *Tobias Pfaff, Meire Fortunato, Alvaro Sanchez-Gonzalez, and Peter Battaglia.*

1. **Learning large-scale subsurface simulations with a hybrid graph network simulator.** KDD, 2022. [paper](https://arxiv.org/abs/2206.07680)

   *Tailin Wu, Qinchen Wang, Yinan Zhang, Rex Ying, Kaidi Cao, Rok Sosič, Ridwan Jalali, Hassan Hamam, Marko Maucec, and Jure Leskovec.*

1. **Unravelling the performance of physics-informed graph neural networks for dynamical systems.** NIPS, 2022. [paper](https://openreview.net/forum?id=tXEe-Ew_ikh)

   *Abishek Thangamuthu, Gunjan Kumar, Suresh Bishnoi, Ravinder Bhattoo, N M Anoop Krishnan, and Sayan Ranu.*

1. **Learning the solution operator of boundary value problems using graph neural networks.** ICML, 2022. [paper](https://arxiv.org/abs/2206.14092)

   *Winfried Lötzsch, Simon Ohler, and Johannes S. Otterbach.*

1. **Physics-informed graph neural Galerkin networks: A unified framework for solving PDE-governed forward and inverse problems.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521007076)

   *Han Gao, Matthew J.Zahr, and Jianxun Wang.*

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

1. **DS-GPS: A deep statistical graph Poisson solver (for faster CFD simulations).** NIPS, 2022. [paper](https://arxiv.org/abs/2211.11763)

   *Matthieu Nastorg, Marc Schoenauer, Guillaume Charpiat, Thibault Faney, Jean-Marc Gratien, and Michele-Alessandro Bucci.*

1. **PF-GNN: Differentiable particle filtering based approximation of universal graph representations.** ICLR, 2022. [paper](https://openreview.net/forum?id=oh4TirnfSem)

   *Mohammed Haroon Dupty, Yanfei Dong, and Wee Sun Lee.*

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

1. **MG-GNN: Multigrid graph neural networks for learning multilevel domain decomposition methods.** ICML, 2023. [paper](https://openreview.net/forum?id=bkRrdYhd7U)

   *Ali Taghibakhshi, Nicolas Nytko, Tareq Uz Zaman, Scott MacLachlan, Luke Olson, and Matthew West.*

1. **Multi-scale message passing neural PDE solvers.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.03580)

   *Léonard Equer, T. Konstantin Rusch, and Siddhartha Mishra.*

1. **An implicit GNN solver for Poisson-like problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.10891)

   *Matthieu Nastorg, Michele-Alessandro Bucci, Thibault Faney, Jean-Marc Gratien, Guillaume Charpiat, and Marc Schoenauer.*

1. **GNN-based physics solver for time-independent PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.15681)

   *Rini Jasmine Gladstone, Helia Rahmani, Vishvas Suryakumar, Hadi Meidani, Marta D'Elia, and Ahmad Zareei.*

1. **E(3) equivariant graph neural networks for particle-based fluid mechanics.** ICLR, 2023. [paper](https://arxiv.org/abs/2304.00150)

   *Artur P. Toshev, Gianluca Galletti, Johannes Brandstetter, Stefan Adami, and Nikolaus A. Adams.*

1. **Long-short-range message-passing: A physics-informed framework to capture non-local interaction for scalable molecular dynamics simulation.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.13542)

   *Yunyang Li, Yusong Wang, Lin Huang, Han Yang, Xinran Wei, Jia Zhang, Tong Wang, Zun Wang, Bin Shao, and Tieyan Liu.*

1. **A graph convolutional autoencoder approach to model order reduction for parametrized PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.08573)

   *Federico Pichi, Beatriz Moya, and Jan S. Hesthaven.*

1. **GAD-NR: Graph anomaly detection via neighborhood reconstruction.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.01951)

   *Amit Roy, Juan Shu, Jia Li, Carl Yang, Olivier Elshocht, Jeroen Smeets, and Pan Li.*

1. **GPINN: Physics-informed neural network with graph embedding.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.09792)

   *Yuyang Miao and Haolin Li.*

1. **GNRK: Graph Neural Runge-Kutta method for solving partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.00618)

   *Hoyun Choi, Sungyeop Lee, B. Kahng, and Junghyo Jo.*

1. **Equivariant graph neural operator for modeling 3D dynamics.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.11037)

   *Minkai Xu, Jiaqi Han, Aaron Lou, Jean Kossaifi, Arvind Ramanathan, Kamyar Azizzadenesheli, Jure Leskovec, Stefano Ermon, and Anima Anandkumar.*

1. **HAMLET: Graph transformer neural operator for partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.03541)

   *Andrey Bryutkin, Jiahao Huang, Zhongying Deng, Guang Yang, Carola-Bibiane Schönlieb, and Angelica Aviles-Rivero.*

1. **Learning time-dependent PDE via graph neural networks and deep operator network for robust accuracy on irregular grids.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.08187)

   *Sung Woong Cho, Jae Yong Lee, and Hyung Ju Hwang.*

1. **Towards general neural surrogate solvers with specialized neural accelerators.** ICML, 2024. [paper](https://arxiv.org/abs/2405.02351)

   *Chenkai Mao, Robert Lupoiu, Tianxiang Dai, Mingkun Chen, and Jonathan A. Fan.*

1. **Graph neural PDE solvers with conservation and similarity-equivariance.** ICML, 2024. [paper](https://openreview.net/forum?id=WajJf47TUi)

   *Masanobu Horie and Naoto Mitsume.*

1. **Spectral-refiner: Fine-tuning of accurate spatiotemporal neural operator for turbulent flows.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.17211)

   *Shuhao Cao, Francesco Brarda, Ruipeng Li, and Yuanzhe Xi.*

1. **Accelerating simulation of two-phase flows with neural PDE surrogates.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.17260)

   *Yoeri Poels, Koen Minartz, Harshit Bansal, and Vlado Menkovski.*

### [Green Function](#content)
1. **Learning Green's functions associated with time-dependent partial differential equations.** JMLR, 2022. [paper](https://www.jmlr.org/papers/volume23/22-0433/22-0433.pdf)

   *Nicolas Boullé, Seick Kim, Tianyi Shi, and Alex Townsend.*

1. **BI-GreenNet: Learning Green's functions by boundary integral network.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.13247)

   *Guochang Lin, Fukai Chen, Pipi Hu, Xiang Chen, Junqing Chen, Jun Wang, and Zuoqiang Shi.*

1. **DeepGreen: Deep learning of Green’s functions for nonlinear boundary value problems.** Scientific Reports, 2021. [paper](https://www.nature.com/articles/s41598-021-00773-x)

   *Craig R. Gin, Daniel E. Shea, Steven L. Brunton, and J. Nathan Kutz.*

1. **Data-driven discovery of Green’s functions with human-understandable deep learning.** Scientific Reports, 2022. [paper](https://www.nature.com/articles/s41598-022-08745-5)

   *Nicolas Boullé, Christopher J. Earls, and Alex Townsend.*

1. **Data-driven discovery of Green's functions.** Doctoral Dissertation, 2022. [Ph.D.](https://arxiv.org/abs/2210.16016)

   *Nicolas Boullé.*

1. **Principled interpolation of Green's functions learned from data.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.06299)

   *Harshwardhan Praveen, Nicolas Boulle, and Christopher Earls.*

1. **Deep generalized Green's functions.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.02925)

   *Rixi Peng, Juncheng Dong, Jordan Malof, Willie J. Padilla, Vahid Tarokh.*

1. **Operator approximation of the wave equation based on deep learning of Green’s function.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.13902)

   *Ziad Aldirany, R´egis Cottereau, Marc Laforest, and Serge Prudhomme.*

1. **Deep surrogate model for learning Green's function associated with linear reaction-diffusion operator.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.03642)

   *Junqing Ji, Lili Ju, and Xiaoping Zhang.*

1. **Numerical solutions of boundary problems in partial differential equations: A deep learning framework with Green's function.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S002199912400370X)

   *Yuanjun Dai, Zhi Li, Yiran An, and Wanru Deng.*

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

1. **Integration of physics-informed operator learning and finite element method for parametric learning of partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.02363)

   *Shahed Rezaei, Ahmad Moeineddin, Michael Kaliske, and Markus Apel.*

1. **Error assessment of an adaptive finite elements—neural networks method for an elliptic parametric PDE.** CMAME, 2024. [paper](https://arxiv.org/abs/2401.02363)

   *Alexandre Caboussat, Maude Girardin, and Marco Picasso.*

1. **Predicting unsteady incompressible fluid dynamics with finite volume informed neural network.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/4/043601/3280514)

   *Tianyu Li, Shufan Zou, Xinghua Chang, Laiping Zhang, and Xiaogang Deng.*

1. **Unified finite-volume physics informed neural networks to solve the heterogeneous partial differential equations.** KBS, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0950705124004659)

   *Di Mei, Kangcheng Zhou, and Chun-Ho Liu.*

### [Convolution](#content)
1. **PDE-Net: Learning PDEs from data.** ICML, 2018. [paper](https://proceedings.mlr.press/v80/long18a.html)

   *Zichao Long, Yiping Lu, Xianzhong Ma, and Bin Dong.*

1. **PDE-Net 2.0: Learning PDEs from data with a numeric-symbolic hybrid deep network.** JCP, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119306308)

   *Zichao Long, Yiping Lu, and Bin Dong.*

1. **Physics-informed CNNs for super-resolution of sparse observations on dynamical systems.** NIPS, 2022. [paper](https://arxiv.org/abs/2210.17319)

   *Daniel Kelshaw, Georgios Rigas, and Luca Magri.*

1. **Deep-pretrained-FWI: Combining supervised learning with physics-informed neural network.** NIPS, 2022. [paper](https://arxiv.org/abs/2212.02338)

   *Ana Paula O. Muller, Clecio R. Bom, Jessé C. Costa, Matheus Klatt, Elisângela L. Faria, Marcelo P. de Albuquerque, and Márcio P. de Albuquerque.*

1. **Learning time-dependent PDEs with a linear and nonlinear separate convolutional neural network.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121008238)

   *Jiagang Qu, Weihua Cai, and YijunZhao.*

1. **PhyCRNet: Physics-informed convolutional-recurrent network for solving spatiotemporal PDEs.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521006514)

   *Pu Ren, Chengping Rao, Yang Liu, Jianxun Wang, and Hao Sun.*

1. **Spline-PINN: Approaching PDEs without data using fast, physics-informed Hermite-Spline CNNs.** AAAI, 2019. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/20830/20589)

   *Nils Wandel, Michael Weinmann, Michael Neidlin, and Reinhard Klein.*

1. **Deep convolutional Ritz method: Parametric PDE surrogates without labeled data.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.04675)

   *Jan Niklas Fuhg, Arnav Karmarkar, Teeratorn Kadeethum, Hongkyu Yoon, and Nikolaos Bouklas.*

1. **Deep convolutional architectures for extrapolative forecasts in time-dependent flow problems.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.09651)

   *Pratyush Bhatt, Yash Kumar, and Azzeddine Soulaimani.*

1. **Phase2Vec: Dynamical systems embedding with a physics-informed convolutional network.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.03857)

   *Matthew Ricci, Noa Moriel, Zoe Piran, and Mor Nitzan.*

1. **Numerical approximation based on deep convolutional neural network for high-dimensional fully nonlinear merged PDEs and 2BSDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.04997)

   *Xu Xiao and Wenlin Qiu.*

1. **SplineCNN: Fast geometric deep learning with continuous B-spline kernels.** CVPR, 2018. [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Fey_SplineCNN_Fast_Geometric_CVPR_2018_paper.pdf)

   *Matthias Fey, Jan Eric Lenssen, Frank Weichert, and Heinrich Muller.*

1. **Physics-informed deep super-resolution for spatiotemporal data.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.01462)

   *Pu Ren, Chengping Rao, Yang Liu, Zihan Ma, Qi Wang, Jianxun Wang, and Hao Sun.*

1. **MeshFreeFLowNet: A physics-constrained deep continuous space-time super-resolution framework.** SC20, 2020. [paper](https://ieeexplore.ieee.org/document/9355293)

   *Chiyu Max Jiang, Soheil Esmaeilzadeh, Kamyar Azizzadenesheli, Karthik Kashinath, Mustafa Mustafa, Hamdi A. Tchelepi, Philip Marcus Prabhat, and Anima Anandkumar.*

1. **Convolutional neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.01178)

   *Bogdan Raonić, Roberto Molinaro, Tobias Rohner, Siddhartha Mishra, and Emmanuel de Bezenac.*

1. **An unsupervised latent/output physics-informed convolutional-LSTM network for solving partial differential equations using peridynamic differential operator.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782523000671)

   *Arda Mavi, Ali Can Bekar, Ehsan Haghigh, and Erdogan Madenci.*

1. **Clifford neural layers for PDE modeling.** ICLR, 2023. [paper](https://openreview.net/forum?id=okwxL_c4x84)

   *Johannes Brandstetter, Rianne van den Berg, Max Welling, and Jayesh K Gupta.*

1. **Neural partial differential equations with functional convolution.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.07194)

   *Ziqian Wu, Xingzhe He, Yijun Li, Cheng Yang, Rui Liu, Shiying Xiong, and Bo Zhu.*

1. **Multilevel CNNs for parametric PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.00388v2)

   *Cosmas Heiß, Ingo Gühring, and Martin Eigel.*

1. **Encoding physics to learn reaction–diffusion processes.** NMI, 2023. [paper](https://www.nature.com/articles/s42256-023-00685-7)

   *Chengping Rao, Pu Ren, Qi Wang, Oral Buyukozturk, Hao Sun, and Yang Liu.*

1. **PhySR: Physics-informed deep super-resolution for spatiotemporal data.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123005338)

   *Pu Ren, Chengping Rao, Yang Liu, Zihan Ma, Qi Wang, Jianxun Wang, and Hao Sun.*

1. **Local convolution enhanced global Fourier neural operator for multiscale dynamic spaces prediction.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.12902)

   *Xuanle Zhao, Yue Sun, Tielin Zhang, and Bo Xu.*

1. **A practical existence theorem for reduced order models based on convolutional autoencoders.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.00435)

   *Nicola Rares Franco and Simone Brugiapaglia.*

1. **Closure discovery for coarse-grained partial differential equations using multi-agent reinforcement learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.00972)

   *Jan-Philipp von Bassewitz, Sebastian Kaltenbach, and Petros Koumoutsakos.*

1. **PARCv2: Physics-aware recurrent convolutional neural networks for spatiotemporal dynamics modeling.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.12503)

   *Phong C.H. Nguyen, Xinlun Cheng, Shahab Arfaza, Pradeep Seshadri, Yen T. Nguyen, Munho Kim, Sanghun Choi, H.S. Udaykumar, and Stephen Baek.*

1. **Neural operators with localized integral and differential kernels.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.16845)

   *Miguel Liu-Schiaffini, Julius Berner, Boris Bonev, Thorsten Kurth, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **PDE-CNNs: Axiomatic derivations and applications.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.15182)

   *Gijs Bellaard, Sei Sakata, Bart M. N. Smets, and Remco Duits.*

1. **Symmetric basis convolutions for learning Lagrangian fluid mechanics.** ICLR, 2024. [paper](https://openreview.net/forum?id=HKgRwNhI9R)

   *Rene Winchenbach and Nils Thuerey.*

1. **Fully differentiable Lagrangian convolutional neural network for continuity-consistent physics-informed precipitation nowcasting.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.10747)

   *Peter Pavlík, Martin Výboh, Anna Bou Ezzeddine, and Viera Rozinajová.*

1. **Theory guided Lagrange programming neural network for subsurface flow problems.** EAAI, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197624008145)

   *Jian Wang, Xiaofeng Xue, Zhixue Sun, Jun Yao, El-Sayed M. El-Alfy, Kai Zhang, Witold Pedrycz, and Jacek Mańdziuk.*

1. **Physics-aware recurrent convolutional neural networks for modeling multiphase compressible flows.** International Journal of Multiphase Flow, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S030193222400154X)

   *Xinlun Cheng, Phong C.H. Nguyen, Pradeep K. Seshadri, Mayank Verma, Zoë J. Gray, Jack T. Beerman, H.S. Udaykumar, and Stephen S. Baek.*

### [AutoEncoder](#content)
1. **Integral autoencoder network for discretization-invariant learning.** JMLR, 2022. [paper](https://www.jmlr.org/papers/v23/22-0297.html)

   *Yong Zheng Ong, Zuowei Shen, and Haizhao Yang.*

1. **Variational autoencoding neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.10351)

   *Jacob H. Seidman, Georgios Kissas, George J. Pappas, and Paris Perdikaris.*

1. **PI-VEGAN: Physics informed variational embedding generative adversarial networks for stochastic differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.10351)

   *Ruisong Gao, Yufeng Wang, Min Yang, and Chuanjun Chen.*

1. **On the latent dimension of deep autoencoders for reduced order modeling of PDEs parametrized by random fields.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.12095)

   *Nicola Rares Franco, Daniel Fraulin, Andrea Manzoni, and Paolo Zunino.*

1. **Modeling unknown stochastic dynamical system via Autoencoder.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.10001)

   *Zhongshu Xu, Yuan Chen, Qifan Chen, and Dongbin Xiu.*

1. **Parameterized physics-informed neural networks for parameterized PDEs.** ICML, 2024. [paper](https://openreview.net/forum?id=n3yYrtt9U7)

   *Woojin Cho, Minju Jo, Haksoo Lim, Kookjin Lee, Dongeun Lee, Sanghyun Hong, and Noseong Park.*

### [Neural Operator](#content)
1. **Multiwavelet-based operator learning for differential equations.** NIPS, 2021. [paper](https://openreview.net/forum?id=LZDiWaC9CGL)

   *Gaurav Gupta, Xiongye Xiao, and Paul Bogdan.*

1. **On the representation of solutions to elliptic PDEs in Barron space.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/32cfdce9631d8c7906e8e9d6e68b514b-Abstract.html)

   *Ziang Chen, Jianfeng Lu, and Yulong Lu.*

1. **Low-rank registration based manifolds for convection-dominated PDEs.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16116)

   *Rambod Mojgani and Maciej Balajewicz.*

1. **Isogeometric neural networks: A new deep learning approach for solving parameterized partial differential equations.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522007952)

   *Joshua Gasick and Xiaoping Qian.*

1. **A nonlocal physics-informed deep learning framework using the peridynamic differential operator.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521003431)

   *Ehsan Haghighat, Ali CanBekar, Erdogan Madenci, and Ruben Juanes.*

1. **Kernel flows: From learning kernels from data into the abyss.** JCP, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119302232)

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

1. **Guiding continuous operator learning through physics-based boundary constraints.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.07477)

   *Nadim Saad, Gaurav Gupta, Shima Alizadeh, and Danielle C. Maddix.*

1. **BelNet: Basis enhanced learning, a mesh-free neural operator.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.07336)

   *Zecheng Zhang, Wing Tat Leung, and Hayden Schaeffer.*

1. **INO: Invariant neural operators for learning complex physical systems with momentum conservation.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.14365)

   *Ning Liu, Yue Yu, Huaiqian You, and Neeraj Tatikola.*

1. **BINN: A deep learning approach for computational mechanics problems based on boundary integral equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.04480)

   *Jia Sun, Yinghua Liu, Yizheng Wang, Zhenhan Yao, and Xiaoping Zheng.*

1. **Koopman neural operator as a mesh-free solver of non-linear partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.10022)

   *Wei Xiong, Xiaomeng Huang, Ziyang Zhang, Ruixuan Deng, Pei Sun, and Yang Tian.*

1. **Physics-informed Koopman network.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.09419)

   *Yuying Liu, Aleksei Sholokhov, Hassan Mansour, and Saleh Nabi.*

1. **Deep operator learning lessens the curse of dimensionality for PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.10022)

   *Ke Chen, Chunmei Wang, and Haizhao Yang.*

1. **Algorithmically designed artificial neural networks (ADANNs): Higher order deep operator learning for parametric partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.03286)

   *Arnulf Jentzen, Adrian Riekert, and Philippe von Wurstemberger.*

1. **Entropy-dissipation informed neural network for McKean-Vlasov type.** arXiv, 2023. [paper](http://faculty.bicmr.pku.edu.cn/~zhenfuwang/Entropy_Dissipation.pdf)

   *Zebang Shen and Zhenfu Wang.*

1. **A neural PDE solver with temporal stencil modeling.** ICML, 2023. [paper](https://openreview.net/forum?id=ghdyH3u8y3)

   *Zhiqing Sun, Yiming Yang, and Shinjae Yoo.*

1. **Neural operator learning for long-time integration in dynamical systems with recurrent neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.02243)

   *Katarzyna Michałowska, Somdatta Goswami, George Em Karniadakis, and Signe Riemer-Sørensen.*

1. **Coupled multiwavelet operator learning for coupled differential equations.** ICLR, 2023. [paper](https://openreview.net/forum?id=kIo_C6QmMOM)

   *Xiongye Xiao, Defu Cao, Ruochen Yang, Gaurav Gupta, Chenzhong Yin, Gengshuo Liu, Radu Balan, and Paul Bogdan.*

1. **Vandermonde neural operator.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.19663)

   *Levi Lingsch, Mike Michelis, Sirani M. Perera, Robert K. Katzschmann, and Siddartha Mishra.*

1. **Energy-dissipative evolutionary deep operator neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.06281)

   *Jiahao Zhang, Shiheng Zhang, Jie Shen, and Guang Lin.*

1. **Physics informed WNO.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.05925)

   *Navaneeth N, Tapas Tripura, and Souvik Chakraborty.*

1. **Corrector operator to enhance accuracy and reliability of neural operator surrogates of nonlinear variational boundary-value problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.12047v2)

   *Prashant K. Jha and J. Tinsley Oden.*

1. **HNO: Hyena neural operator for solving PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.16524)

   *Saurabh Patil, Zijie Li, and Amir Barati Farimani.*

1. **Finite element operator network for solving parametric PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.04690)

   *Jae Yong Lee, Seungchan Ko, and Youngjoon Hong.*

1. **PDE-Refiner: Achieving accurate long rollouts with neural PDE solvers.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.05732)

   *Phillip Lippe, Bastiaan S. Veeling, Paris Perdikaris, Richard E. Turner, and Johannes Brandstetter.*

1. **Online infinite-dimensional regression: Learning linear operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.06548)

   *Vinod Raman, Unique Subedi, and Ambuj Tewari.*

1. **Online infinite-dimensional regression: Learning linear operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.06548)

   *Vinod Raman, Unique Subedi, and Ambuj Tewari.*

1. **Deep-OSG: Deep learning of operators in semigroup.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123005934)

   *Junfeng Chen and Kailiang Wu.*

1. **D2NO: Efficient handling of heterogeneous input function spaces with distributed deep neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.18888)

   *Zecheng Zhang, Christian Moya, Lu Lu, Guang Lin, and Hayden Schaeffer.*

1. **Physics informed WNO.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523006709)

   *Navaneeth N., Tapas Tripura, and Souvik Chakraborty.*

1. **Neural oscillators for generalizing parametric PDEs.** NIPS, 2023. [paper](https://nips.cc/virtual/2023/75490)

   *Taniya Kapoor, Abhishek Chandra, and Daniel M. Tartakovsky.*

1. **B-LSTM-MIONet: Bayesian LSTM-based neural operators for learning the response of complex dynamical systems to length-variant multiple input functions.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.16519)

   *Zhihao Kong, Amirhossein Mollaali, Christian Moya, Na Lu, and Guang Lin.*

1. **GIT-Net: Generalized integral transform for operator learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.02450)

   *Chao Wang and Alexandre Hoang Thiery.*

1. **Neural spectral methods: Self-supervised learning in the spectral domain.** ICLR, 2024. [paper](https://openreview.net/forum?id=2DbVeuoa6a)

   *Yiheng Du, Nithin Chalapathi, and Aditi S. Krishnapriyan.*

1. **A nonlinear-manifold reduced-order model and operator learning for partial differential equations with sharp solution gradients.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523008071)

   *Peiyi Chen, Tianchen Hu, and Johann Guilleminot.*

1. **Operator-learning-inspired modeling of neural ordinary differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.10274)

   *Woojin Cho, Seunghyeon Cho, Hyundong Jin, Jinsung Jeon, Kookjin Lee, Sanghyun Hong, Dongeun Lee, Jonghyun Choi, and Noseong Park.*

1. **Operator learning for hyperbolic partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.17489)

   *Christopher Wang and Alex Townsend.*

1. **BENO: Boundary-embedded neural operators for elliptic PDEs.** ICLR, 2024. [paper](https://openreview.net/forum?id=ZZTkLDRmkg)

   *Haixin Wang, Jiaxin Li, Anubhav Dwivedi, Kentaro Hara, and Tailin Wu.*

1. **Koopman operator learning using invertible neural networks.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999124000445)

   *Yuhuang Meng, Jianguo Huang, and Yue Qiu.*

1. **Operator learning without the adjoint.** arXiv, 2024. [paper](https://.arxiv.org/abs/2401.17739)

   *Nicolas Boullé, Diana Halikias, Samuel E. Otto, and Alex Townsend.*

1. **Neural operators meet energy-based theory: Operator learning for Hamiltonian and dissipative PDEs.** arXiv, 2024. [paper](https://.arxiv.org/abs/2402.09018)

   *Yusuke Tanaka, Takaharu Yaguchi, Tomoharu Iwata, and Naonori Ueda.*

1. **Learning solution operators of PDEs defined on varying domains via MIONet.** arXiv, 2024. [paper](https://.arxiv.org/abs/2402.15097)

   *Shanshan Xiao, Pengzhan Jin, and Yifa Tang.*

1. **Neural operators with localized integral and differential kernels.** arXiv, 2024. [paper](https://.arxiv.org/abs/2402.16845)

   *Miguel Liu-Schiaffini, Julius Berner, Boris Bonev, Thorsten Kurth, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **Data scoping: Effectively learning the evolution of generic transport PDEs.** arXiv, 2024. [paper](https://.arxiv.org/abs/2405.01319)

   *Jiangce Chen, Wenzhuo Xu, Zeda Xu, Noelia Grande Gutiérrez, Sneha Prabha Narra, and Christopher McComb.*

1. **Newton informed neural operator for computing multiple solutions of nonlinear partials differential equations.** arXiv, 2024. [paper](https://.arxiv.org/abs/2405.14096)

   *Wenrui Hao, Xinliang Liu, and Yahong Yang.*

1. **FUSE: Fast unified simulation and estimation for PDEs.** arXiv, 2024. [paper](https://.arxiv.org/abs/2405.14558)

   *Levi E. Lingsch, Dana Grund, Siddhartha Mishra, and Georgios Kissas.*

1. **Reference neural operators: Learning the smooth dependence of solutions of PDEs on geometric deformations.** ICML, 2024. [paper](https://openreview.net/forum?id=CecY6XiUfu)

   *Ze Cheng, Zhongkai Hao, Xiaoqiang Wang, Jianing Huang, Youjia Wu, Xudan Liu, Yiru Zhao, Songming Liu, and Hang Su.*

1. **Variational operator learning: A unified paradigm marrying training neural operators and solving partial differential equations.** Journal of the Mechanics and Physics of Solids, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0022509624001807)

   *Tengfei Xu, Dachuan Liu, Peng Hao, and Bo Wang.*

1. **Laplace neural operator for solving differential equations.** NMI, 2024. [paper](https://www.nature.com/articles/s42256-024-00844-4)

   *Qianying Cao, Somdatta Goswami, and George Em Karniadakis.*

### [Machine Learning](#content)
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

1. **Nonlocal kernel network (NKN): A stable and resolution-independent deep neural network.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122005988)

   *Huaiqian You, Yue Yu, Marta D'Elia, Tian Gao, and Stewart Silling.*

1. **On computing the hyperparameter of extreme learning machines: Algorithm and application to computational PDEs, and comparison with classical and high-order finite elements.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003527#!)

   *Suchuan Dong and Jielin Yang.*

1. **Int-Deep: A deep learning initialized iterative method for nonlinear problems.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120304496)

   *Jianguo Huang, Haoqin Wang, and Haizhao Yang.*

1. **DeLISA: Deep learning based iteration scheme approximation for solving PDEs.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121007798)

   *Ying Li, Zuojia Zhou, and Shihui Ying.*

1. **Physics-informed machine learning for reduced-order modeling of nonlinear problems.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005611)

   *Wenqian Chen, Qian Wang, Jan S.Hesthaven, and Chuhua Zhang.*

1. **SelectNet: Self-paced learning for high-dimensional partial differential equations.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121003399)

   *Yiqi Gu, Haizhao Yang, and Chao Zhou.*

1. **Deep least-squares methods: An unsupervised learning-based numerical method for solving elliptic PDEs.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120304812)

   *Zhiqiang Cai, Jingshuang Chen, Min Liu, and Xinyu Liu.*

1. **Local extreme learning machines and domain decomposition for solving linear and nonlinear partial differential equations.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521004606)

   *Suchuan Dong and Zongwei Li.*

1. **Iterative surrogate model optimization (ISMO): An active learning algorithm for PDE constrained optimization with deep neural networks.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S004578252030760X)

   *Kjetil O.Lye, Siddhartha Mishra, Deep Ray, and Praveen Chandrashekar.*

1. **Probabilistic learning on manifolds constrained by nonlinear partial differential equations for small datasets.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521001134)

   *C. Soize and R. Ghanem.*

1. **An energy approach to the solution of partial differential equations in computational mechanics via machine learning: Concepts, implementation and applications.** CMAME, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0045782519306826)

   *E. Samaniego, C. Anitescu, S.Goswami, V.M.Nguyen-Thanh, H.Guo, K.Hamdia, X.Zhuang, and T.Rabczuk.*

1. **Reduced order modeling for parameterized time-dependent PDEs using spatially and memory aware deep learning.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S1877750321000934)

   *Nikolaj T.Mücke, Sander M.Bohté, and Cornelis W.Oosterlee.*

1. **GCN-FFNN: A two-stream deep model for learning solution to partial differential equations.** Neurocomputing, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0925231222011511?dgcid=rss_sd_all)

   *Onur Bilgin, Thomas Vergutz, Siamak Mehrkanoon.*

1. **Deep-HyROMnet: A deep learning-based operator approximation for hyper-reduction of nonlinear parametrized PDEs.** Journal of Scientific Computing, 2021. [paper](https://link.springer.com/article/10.1007/s10915-022-02001-8)

   *Ludovica Cicci, Stefania Fresca, and Andrea Manzoni.*

1. **HybridNet: Integrating model-based and data-driven learning to predict evolution of dynamical systems.** CoRL, 2018. [paper](https://proceedings.mlr.press/v87/long18a.html)

   *Yun Long, Xueyuan She, and Saibal Mukhopadhyay.*

1. **A model-constrained tangent slope learning approach for dynamical systems.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.04995)

   *Hai V. Nguyen and Tan Bui-Thanh.*

1. **Solving PDEs on unknown manifolds with machine learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2106.06682)

   *Senwei Liang, Shixiao W. Jiang, John Harlim, and Haizhao Yang.*

1. **Model reduction and neural networks for parametric PDEs.** SIAM Journal of Computational Mathematics, 2021. [paper](https://smai-jcm.centre-mersenne.org/item/SMAI-JCM_2021__7__121_0/)

   *Kaushik Bhattacharya, Bamdad Hosseini, Nikola B. Kovachki, and Andrew M. Stuart.*

1. **MOD-Net: A machine learning approach via model-operator-data network for solving PDEs.** Communications in Computational Physics, 2022. [paper](https://global-sci.org/intro/article_detail/cicp/20860.html#)

   *Shamsulhaq Basir and Inanc Senocak.*

1. **A deep double Ritz method (D^2RM) for solving partial differential equations using neural networks.** CMAME, 2023. [paper](https://global-sci.org/intro/article_detail/cicp/20860.html#)

   *Carlos Uriarte, David Pardo, Ignacio Muga, and Judit Muñoz-Matute.*

1. **Data- and theory-guided learning of partial differential equations using simultaneous basis function approximation and parameter estimation (SNAPE).** MSSP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S088832702201127X)

   *Sutanu Bhowmick, Satish Nagarajaiah, and Anastasios Kyrillidis.*

1. **Invariant preservation in machine learned PDE solvers via error correction.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.16110)

   *Nick McGreivy and Ammar Hakim.*

1. **Operator learning with PCA-Net: upper and lower complexity bounds.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.16317v2)

   *Samuel Lanthaler.*

1. **Multiscale attention via wavelet neural operators for vision Transformers.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.12398)

   *Anahita Nekoozadeh, Mohammad Reza Ahmadzadeh, Zahra Mardani, and Morteza Mardani.*

1. **Pseudo-Hamiltonian neural networks for learning partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.14374)

   *Sølve Eidnes and Kjetil Olsen Lye.*

1. **SHoP: A deep learning framework for solving high-order partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.10033)

   *Tingxiong Xiao, Runzhao Yang, Yuxiao Cheng, Jinli Suo, and Qionghai Dai.*

1. **A Neural RDE-based model for solving path-dependent PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.01123)

   *Bowen Fang, Hao Ni, and Yue Wu.*

1. **Global universal approximation of functional input maps on weighted spaces.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.03303)

   *Christa Cuchiero, Philipp Schmocker, and Josef Teichmann.*

1. **Accelerating explicit time-stepping with spatially variable time steps through machine learning.** Journal of Scientific Computing, 2023. [paper](https://link.springer.com/article/10.1007/s10915-023-02260-z)

   *Kiera van der Sande, Natasha Flyer, and Bengt Fornberg.*

1. **Learning elliptic partial differential equations with randomized linear algebra.** Foundations of Computational Mathematics, 2023. [paper](https://link.springer.com/article/10.1007/s10208-022-09556-w)

   *Nicolas Boullé and Alex Townsend .*

1. **A deep double Ritz method (D^2RM) for solving partial differential equations using neural networks.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782523000154)

   *Carlos Uriarte, David Pardo, Ignacio Mug, and Judit Muñoz-Matute.*

1. **A deep learning framework for solving hyperbolic partial differential equations: Part I.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.04121)

   *Rajat Arora.*

1. **Fully probabilistic deep models for forward and inverse problems in parametric PDEs.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123004643)

   *Arnaud Vadeboncoeur, Ömer Deniz Akyildiz, Ieva Kazlauskaite, Mark Girolami, and Fehmi Cirak.*

1. **An axiomatized PDE model of deep neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.12333)

   *Tangjun Wang, Wenqi Tao, Chenglong Bao, and Zuoqiang Shi.*

1. **Element learning: A systematic approach of accelerating finite element-type methods via machine learning, with applications to radiative transfer.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.02467)

   *Shukai Du and Samuel N. Stechmann.*

1. **Deep multi-step mixed algorithm for high dimensional non-linear PDEs and associated BSDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.14487)

   *Daniel Bussell and Camilo Andrés García-Trillos.*

1. **Artificial to spiking neural networks conversion for scientific machine learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.16372)

   *Qian Zhang, Chenxi Wu, Adar Kahana, Youngeun Kim, Yuhang Li, George Em Karniadakis, and Priyadarshini Panda.*

1. **Data generation-based operator learning for solving partial differential equations on unbounded domains.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.02446)

   *Jihong Wang, Xin Wang, Jing Li, and Bin Liu.*

1. **Slow invariant manifolds of singularly perturbed systems via physics-informed machine learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.07946)

   *Dimitrios G. Patsatzis, Gianluca Fabiani, Lucia Russo, and Constantinos Siettos.*

1. **Spectral operator learning for parametric PDEs without data reliance.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.02013)

   *Junho Choi, Taehyun Yun, Namjung Kim, and Youngjoon Hong.*

1. **The deep minimizing movement scheme.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123006137)

   *Min Sue Park, Cheolhyeong Kim, Hwijae Son, and Hyung Ju Hwang .*

1. **Learning nonlinear integral operators via recurrent neural networks and its application in solving integro-differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.09434)

   *Hardeep Bassi, Yuanran Zhu, Senwei Liang, Jia Yin, Cian C. Reeves, Vojtech Vlcek, and Chao Yang.*

1. **Adaptive deep neural networks for solving corner singular problems.** Engineering Analysis with Boundary Elements, 2023. [paper](https://arxiv.org/abs/2310.09434)

   *Shaojie Zeng, Yijie Liang, and Qinghui Zhang.*

1. **FastSVD-ML–ROM: A reduced-order modeling framework based on machine learning for real-time applications.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523002797)

   *G.I. Drakoulas, T.V. Gortsas, G.C. Bourantas, V.N. Burganos, and D. Polyzos.*

1. **Nonintrusive reduced-order models for parametric partial differential equations via data-driven operator inference.** SIAM Journal on Scientific Computing, 2023. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1452810)

   *Shane A. McQuarrie, Parisa Khodabakhshi, and Karen E. Willcox.*

1. **Deep learning approximations for non-local nonlinear PDEs with Neumann boundary conditions.** Partial Differential Equations and Applications, 2023. [paper](https://link.springer.com/article/10.1007/s42985-023-00244-0)

   *Victor Boussange, Sebastian Becker, Arnulf Jentzen, Benno Kuckuck, and Loïc Pellissier.*

1. **Neural networks with kernel-weighted corrective residuals for solving partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.03492)

   *Carlos Mora, Amin Yousefpour, Shirin Hosseinmardi, and Ramin Bostanabad.*

1. **Spectral integrated neural networks (SINNs) for solving forward and inverse dynamic problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.03643)

   *Lin Qiu, Fajie Wang, Wenzhen Qu, Yan Gu, and Qinghua Qin.*

1. **Deep FBSDE neural networks for solving incompressible Navier-Stokes equation and Cahn-Hilliard equation.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.03427)

   *Yangtao Deng and Qiaolin He.*

1. **Modeling spatio-temporal dynamical systems with neural discrete learning and levels-of-experts.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.05970)

   *Kun Wang, Hao Wu, Guibin Zhang, Junfeng Fang, Yuxuan Liang, Yuankai Wu, Roger Zimmermann, and Yang Wang.*

1. **Solving Euler equations with gradient-weighted multi-input high-dimensional feature neural network.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/3/035150/3272548)

   *Jiebin Zhao, Wei Wu, Xinlong Feng, and Hui Xu.*

1. **TENG: Time-evolving natural gradient for solving PDEs with deep neural net.** ICML, 2024. [paper](https://openreview.net/forum?id=v1I4zRAjMb)

   *Zhuo Chen, Jacob McCarran, Esteban Vizcaino, Marin Soljačić, and Di Luo.*

1. **A hybrid kernel-free boundary integral method with operator learning for solving parametric partial differential equations in complex domains.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.15242)

   *Shuo Ling, Liwei Tan, and Wenjun Ying.*

1. **Full error analysis of the random deep splitting method for nonlinear parabolic PDEs and PIDEs with infinite activity.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.05192)

   *Ariel Neufeld, Philipp Schmocker, and Sizhou Wu.*

1. **Multiple wavefield solutions in physics-informed neural networks using latent representation.** IEEE Geoscience and Remote Sensing Letters, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10521697)

   *Mohammad H. Taufik, Xinquan Huang, and Tariq Alkhalifah.*

1. **Solving Poisson equations using neural walk-on-spheres.** ICML, 2024. [paper](https://arxiv.org/abs/2406.03494)

   *Hong Chul Nam, Julius Berner, and Anima Anandkumar.*

### [Identification](#content)
1. **Data-driven discovery of partial differential equations.** SA, 2017. [paper](https://arxiv.org/abs/1910.11710)

   *Wei Cai and Zhiqin John Xu.*

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

1. **Machine learning hidden symmetries.** PRL, 2022. [paper](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.128.180201)

   *Ziming Liu and Max Tegmark.*

1. **Efficient learning of sparse and decomposable PDEs using random projection.** UAI, 2022. [paper](https://openreview.net/forum?id=SCg9JDUscgq)

   *Md Nasim, Xinghang Zhang, Anter El-Azab, and Yexiang Xue.*

1. **Data-driven discovery of partial differential equation models with latent variables.** Physical Review E, 2019. [paper](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.100.022219)

   *Patrick A. K. Reinbold and Roman O. Grigoriev.*

1. **Physics constrained learning for data-driven inverse modeling from sparse observations.** Physical Review E, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121008330)

   *Kailai Xua and Eric Darve.*

1. **Deep neural network modeling of unknown partial differential equations in nodal space.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100677X)

   *Zhen Chen, and Victor Churchill, Kailiang Wu, and Dongbin Xiu.*

1. **DeepMOD: Deep learning for model discovery in noisy data.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120307592)

   *Gert-Jan Both, Subham Choudhury, Pierre Sens, and Remy Kusters.*

1. **Theory-guided hard constraint projection (HCP): A knowledge-based data-driven scientific machine learning method.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005192)

   *Yuntian Chen, Dou Huang, Dongxiao Zhang, Junsheng Zeng, Nanzhe Wang, Haoran Zhang, and Jinyue Yan.*

1. **Deep-learning based discovery of partial differential equations in integral form from sparse and noisy data.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121004873)

   *Hao Xua, Dongxiao Zhang, and Nanzhe Wang.*

1. **Peridynamics enabled learning partial differential equations.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121000887)

   *Ali C.Bekar and Erdogan Madenci.*

1. **Data-driven deep learning of partial differential equations in modal space.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120300814)

   *Kailiang Wu and Dongbin Xiu.*

1. **DLGA-PDE: Discovery of PDEs with incomplete candidate library via combination of deep learning and genetic algorithm.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120303582)

   *Hao Xu, Haibin Chang, and Dongxiao Zhang.*

1. **Learning nonlocal constitutive models with neural networks.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782521002644)

   *Xuhui Zhou, Jiequn Han, and Heng Xiao.*

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

1. **Modeling the dynamics of PDE systems with physics-constrained deep auto-regressive networks.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307612)

   *Nicholas Geneva and Nicholas Zabaras.*

1. **Deep learning and inverse discovery of polymer self-consistent field theory inspired by physics-informed neural networks.** Physical Review E, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307612)

   *Danny Lin and Hsiu-Yu Yu.*

1. **Data-driven solutions and parameter discovery of the Sasa–Satsuma equation via the physics-informed neural networks method.** Physica D, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0167278922002044)

   *Haotian Luo, Lei Wang, Yabin Zhang, Gui Lu, Jingjing Su, and Yinchuan Zhao.*

1. **Reliable extrapolation of deep neural operators informed by physics or sparse observations.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/ab)

   *Min Zhu, Handi Zhang, Anran Jiao, George Em Karniadakis, and Lu Lu.*

1. **Neural operator with regularity structure for modeling dynamics driven by SPDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.06255)

   *Peiyan Hu, Qi Meng, Bingguang Chen, Shiqi Gong, Yue Wang, Wei Chen, Rongchan Zhu, Zhiming Ma, and Tieyan Liu.*

1. **A PINN approach to symbolic differential operator discovery with sparse data.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04630)

   *Lena Podina, Brydon Eastman, and Mohammad Kohandel.*

1. **WeakIdent: Weak formulation for identifying differential equations using narrow-fit and trimming.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.03134)

   *Mengyi Tang, Wenjing Liao, Rachel Kuske, and Sung Ha Kang.*

1. **Predicting parametric spatiotemporal dynamics by multi-resolution PDE structure-preserved deep learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.03990)

   *Xinyang Liu, Hao Sun, and Jianxun Wang.*

1. **Data-driven modeling of Landau damping by physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.01021)

   *Yilan Qin, Jiayu Ma, Mingle Jiang, Chuanfei Dong, Haiyang Fu, Liang Wang, Wenjie Cheng, and Yaqiu Jin.*

1. **Discovering governing equations in discrete systems using PINNs.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00971)

   *Sheikh Saqlain, Wei Zhu, Efstathios G. Charalampidis, and Panayotis G. Kevrekidis.*

1. **Physics-guided generative adversarial network to learn physical models.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.11488)

   *Kazuo Yonekura.*

1. **PDE-Learn: Using deep learning to discover partial differential equations from noisy, limited data.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04971)

   *Robert Stephany and Christopher Earls.*

1. **PiSL: Physics-informed Spline Learning for data-driven identification of nonlinear dynamical systems.** MSSP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0888327023000729)

   *Fangzheng Sun, Yang Liu, Qi Wang, Hao Sun.*

1. **Learning physical models that can respect conservation laws.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.11002)

   *Derek Hansen, Danielle C. Maddix, Shima Alizadeh, Gaurav Gupta, and Michael W. Mahoney.*

1. **Data-driven discovery of intrinsic dynamics.** NMI, 2022. [paper](https://www.nature.com/articles/s42256-022-00575-4)

   *Daniel Floryan and Michael D. Graham.*

1. **Symbolic regression for PDEs using pruned differentiable programs.** ICLR, 2023. [paper](https://arxiv.org/abs/2303.07009)

   *Ritam Majumdar, Vishal Jadhav, Anirudh Deodhar, Shirish Karande, Lovekesh Vig, and Venkataramana Runkana.*

1. **Symbolic physics learner: Discovering governing equations via Monte Carlo tree search.** ICLR, 2023. [paper](https://openreview.net/forum?id=ZTK3SefE8_Z)

   *Fangzheng Sun, Yang Liu, Jianxun Wang, Hao Sun.*

1. **Learning neural constitutive laws from motion observations for generalizable PDE dynamics.** ICML, 2023. [paper](https://openreview.net/forum?id=7GD5BMI3km)

   *Pingchuan Ma, Peter Yichen Chen, Bolei Deng, Joshua B. Tenenbaum, Tao Du, Chuang Gan, and Wojciech Matusik.*

1. **Learning partial differential equations in reproducing kernel Hilbert spaces.** JMLR, 2023. [paper](https://www.jmlr.org/papers/volume24/21-1363/21-1363.pdf)

   *George Stepaniants.*

1. **Finite expression methods for discovering physical laws from data.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.08342)

   *Zhongyi Jiang, Chunmei Wang, and Haizhao Yang.*

1. **Physics-informed representation learning for emergent organization in complex dynamical systems.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.12586)

   *Adam Rupe, Karthik Kashinath, Nalini Kumar, and James P. Crutchfield.*

1. **TaylorPDENet: Learning PDEs from non-grid data.** arXiv, 2023. [paper](https://arxiv.org/abs/:2306.14511)

   *Paul Heinisch, Andrzej Dulny, Anna Krause, and Andreas Hotho.*

1. **Learning of discrete models of variational PDEs from data.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.05082)

   *Christian Offen and Sina Ober-Blöbaum.*

1. **Towards true discovery of the differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.04901)

   *Alexander Hvatov and Roman Titov.*

1. **Adaptive uncertainty-guided model selection for data-driven PDE discovery.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.04901)

   *Pongpisit Thanasutives, Takashi Morita, Masayuki Numao, and Ken-ichi Fukui.*

1. **Weak-PDE-LEARN: A weak form based approach to discovering pdes from noisy, limited data.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.04699)

   *Robert Stephany and Christopher Earls.*

1. **Physics-constrained robust learning of open-form PDEs from limited and noisy data.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.07672)

   *Mengge Du, Longfeng Nie, Siyu Lou, Yuntian Chenc, and Dongxiao Zhang.*

1. **Equation discovery with bayesian spike-and-slab priors and efficient kernels.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.05387)

   *Da Long, Wei W. Xing, Aditi S. Krishnapriyan, Robert M. Kirby, Shandian Zhe, and Michael W. Mahoney.*

1. **A Bayesian framework for discovering interpretable Lagrangian of dynamical systems from data.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.06241)

   *Tapas Tripura and Souvik Chakraborty.*

1. **HyperSINDy: Deep generative modeling of nonlinear stochastic governing equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.04832)

   *Mozes Jacobs, Bingni W. Brunton, Steven L. Brunton, J. Nathan Kutz, and Ryan V. Raut.*

1. **Sparse Bayesian machine learning for the interpretable identification of nonlinear structural dynamics: Towards the experimental data-driven discovery of a quasi zero stiffness device.** MSSP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0888327023007665)

   *Tanmoy Chatterjee, Alexander D. Shaw, Michael I. Friswell, and Hamed Haddad Khodaparast.*

1. **SD-PINN: Deep learning based spatially dependent PDEs recovery.** IEEE Access, 2023. [paper](https://arxiv.org/abs/2310.10970)

   *Ruixian Liu and Peter Gerstoft.*

1. **PROSE: Predicting operators and symbolic expressions using multimodal transformers.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.16816)

   *Yuxuan Liu, Zecheng Zhang, and Hayden Schaeffer.*

1. **AI-Aristotle: A physics-informed framework for systems biology gray-box identification.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.01433)

   *Nazanin Ahmadi Daryakenari, Mario De Florio, Khemraj Shukla, and George Em Karniadakis.*

1. **Learning-informed parameter identification in nonlinear time-dependent PDEs.** Applied Mathematics & Optimization, 2023. [paper](https://link.springer.com/article/10.1007/s00245-023-10044-y)

   *Christian Aarset, Martin Holler, and Tram Thi Ngoc Nguyen.*

1. **Data-driven discovery of PDEs via the adjoint method.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.17177)

   *Mohsen Sadr, Tony Tohme, and Kamal Youcef-Toumi.*

1. **Learning the dynamics for unknown hyperbolic conservation laws using deep neural networks.** SIAM Journal on Scientific Computing, 2024. [paper](https://epubs.siam.org/doi/abs/10.1137/22M1537333)

   *Zhen Chen, Anne Gelb, and Yoonsang Lee.*

1. **OptPDE: Discovering novel integrable systems via AI-human collaboration.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.04484)

   *Subhash Kantamneni, Ziming Liu, and Max Tegmark.*

1. **Learning PDEs from data on closed surfaces with sparse optimization.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.06199)

   *Zhengjie Sun, Leevan Ling, and an Zhang.*

1. **Physics-informed parallel neural networks with self-adaptive loss weighting for the identification of continuous structural systems.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524002986)

   *Rui Zhang, Gordon P. Warn, and Aleksandra Radlińska.*

### [Inverse Design](#content)
1. **DPM: Physics-informed Karhunen-Loéve and neural network approximations for solving inverse differential equation problems.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16992/16799)

   *Jungeun Kim, Kookjin Lee, Dongeun Lee, Sheo Yon Jin, and Noseong Park.*

1. **Neural inverse operators for solving PDE inverse problems.** ICML, 2023. [paper](https://arxiv.org/abs/2301.11167)

   *Roberto Molinaro, Yunan Yang, Björn Engquist, and Siddhartha Mishra.*

1. **Physics-informed Karhunen-Loéve and neural network approximations for solving inverse differential equation problems.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122002923)

   *Jing Li and Alexandre M.Tartakovsky.*

1. **Solving inverse problems in stochastic models using deep neural networks and adversarial training.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782521003078)

   *Kailai Xu and Eric Darve.*

1. **Physics-informed neural networks with hard constraints for inverse design.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/21M1397908)

   *Lu Lu, Raphaël Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson.*

1. **Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations.** JCP, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999118307125)

   *M.Raissia, P.Perdikarisb, and George Em Karniadakis.*

1. **GRIDS-Net: Inverse shape design and identification of scatterers via geometric regularization and physics-embedded deep learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.07504)

   *Siddharth Nair, Timothy F. Walsh, Greg Pickrell, and Fabio Semperlotti.*

1. **Bayesian inversion with neural operator (BINO) for modeling subdiffusion: Forward and inverse problems.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.11981)

   *Xiongbin Yan, Zhiqin John Xu, and Zheng Ma.*

1. **Maximum-likelihood estimators in physics-informed neural networks for high-dimensional inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.05991)

   *Gabriel S. Gusmão and Andrew J. Medford.*

1. **Solution of physics-based inverse problems using conditional generative adversarial networks with full gradient penalty.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.04895)

   *Deep Ray, Javier Murgoitio-Esandi, Agnimitra Dasgupta, and Assad A. Oberai.*

1. **Entropy structure informed learning for inverse XDE problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.08241)

   *Yan Jiang, Wuyue Yang, Yi Zhu, and Liu Hong.*

1. **Solving multiphysics-based inverse problems with learned surrogates and constraints.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.11099)

   *Ziyi Yin, Rafael Orozco, Mathias Louboutin, and Felix J. Herrmann.*

1. **Enforcing continuous symmetries in physics-informed neural network for solving forward and inverse problems of partial differential equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123005107)

   *Zhiyong Zhang Hui Zhang, Lisheng Zhang, and Leilei Guo.*

1. **Learning prediction function of prior measures for statistical inverse problems of partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.12436)

   *Junxiong Jia, Deyu Meng, Zongben Xu, and Fang Yao.*

1. **Let data talk: Data-regularized operator learning theory for inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.09854)

   *Ke Chen, Chunmei Wang, and Haizhao Yang.*

1. **Pseudo-differential integral autoencoder network for inverse PDE operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.09856)

   *Ke Chen, Jasen Lai, and Chunmei Wang.*

1. **Adaptive operator learning for infinite-dimensional Bayesian inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.17844)

   *Zhiwei Gao, Liang Yan, and Tao Zhou.*

1. **Variational formulations of the strong formulation -- Forward and inverse modeling using isogeometric analysis and physics-informed networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.03496)

   *Kent-Andre Mardal, Jarle Sogn, and Marius Zeinhofer.*

1. **A method for computing inverse parametric PDE problems with random-weight neural networks.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123003583)

   *Suchuan Dong and Yiran Wang.*

1. **ODE-DPS: ODE-based diffusion posterior sampling for inverse problems in partial differential equation.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.13496)

   *Enze Jiang, Jishen Peng, Zheng Ma, and Xiongbin Yan.*

1. **BiLO: Bilevel local operator learning for PDE inverse problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.17789)

   *Ray Zirui Zhang, Xiaohui Xie, and John Lowengrub.*

1. **Taming score-based diffusion priors for infinite-dimensional nonlinear inverse problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.15676)

   *Lorenzo Baldassari, Ali Siahkoohi, Josselin Garnier, Knut Solna, and Maarten V. de Hoop.*

1. **On the estimation rate of Bayesian PINN for inverse problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.14808)

   *Yi Sun, Debarghya Mukherjee, and Yves Atchade.*

### [Neural ODE](#content)
1. **Neural rough differential equations for long time series.** ICML, 2021. [paper](http://proceedings.mlr.press/v139/morrill21b.html)

   *James Morrill, Cristopher Salvi, Patrick Kidger, and James Foster.*

1. **LEADS: Learning dynamical systems that generalize across environments.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/3df1d4b96d8976ff5986393e8767f5b2-Abstract.html)

   *Yuan Yin, Ibrahim Ayed, Emmanuel de Bézenac, and Nicolas Baskiotis, and Patrick Gallinari.*

1. **A neural ODE interpretation of transformer layers.** NIPS, 2022. [paper](https://arxiv.org/abs/2212.06011)

   *Yuan Yin, Ibrahim Ayed, Emmanuel de Bézenac, Nicolas Baskiotis, and Patrick Gallinari.*

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

   *Marios Mattheaki, David Sondak, Akshunna S. Dogra, and Pavlos Protopapas.*

1. **Deep learning for universal linear embeddings of nonlinear dynamics.** NC, 2018. [paper](https://www.nature.com/articles/s41467-018-07210-0)

   *Bethany Lusch, J. Nathan Kutz, and Steven L. Brunton.*

1. **Stochastic physics-informed neural ordinary differential equations.** arXiv, 2021. [paper](https://arxiv.org/abs/2109.01621)

   *Jared O'Leary, Joel A. Paulson, and Ali Mesbah.*

1. **A stable and scalable method for solving initial value PDEs with neural networks.** ICLR, 2023. [paper](https://openreview.net/forum?id=vsMyHUq_C1c)

   *Marc Anton Finzi, Andres Potapczynski, Matthew Choptuik, and Andrew Gordon Wilson.*

1. **Characteristic neural ordinary differential equation.** ICLR, 2023. [paper](https://openreview.net/forum?id=loIfC8WHevK)

   *Xingzi Xu, Ali Hasan, Khalil Elkhalil, Jie Ding, and Vahid Tarokh.*

1. **Efficient certified training and robustness verification of neural ODEs.** ICLR, 2023. [paper](https://openreview.net/forum?id=KyoVpYvWWnK)

   *Mustafa Zeqiri, Mark Niklas Mueller, Marc Fischer, and Martin Vechev.*

1. **Efficient certified training and robustness verification of neural ODEs.** ICLR, 2023. [paper](https://openreview.net/forum?id=KyoVpYvWWnK)

   *Mustafa Zeqiri, Mark Niklas Mueller, Marc Fischer, and Martin Vechev.*

1. **Physics-informed neural ODE (PINODE): embedding physics into models using collocation points.** Scientific Reports, 2023. [paper](https://www.nature.com/articles/s41598-023-36799-6)

   *Aleksei Sholokhov, Yuying Liu, Hassan Mansour, and Saleh Nabi.*

1. **Data-adaptive probabilistic likelihood approximation for ordinary differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.05566)

   *Mohan Wu and Martin Lysy.*

1. **Neural signature kernels as infinite-width-depth-limits of controlled ResNets.** ICML, 2023. [paper](https://openreview.net/forum?id=0rnA1l6WAc)

   *Nicola Muca Cirone, Maud Lemercier, and Cristopher Salvi.*

1. **AbODE: Ab initio antibody design using conjoined ODEs.** ICML, 2023. [paper](https://openreview.net/forum?id=EB5unD2ojL)

   *Yogesh Verma, Markus Heinonen, and Vikas Garg.*

1. **On the forward invariance of neural ODEs.** ICML, 2023. [paper](https://openreview.net/forum?id=jSkV9aP1Mi)

   *Wei Xiao, Tsun-Hsuan Wang, Ramin Hasani, Mathias Lechner, Yutong Ban, Chuang Gan, and Daniela Rus.*

1. **Predicting ordinary differential equations with Transformers.** ICML, 2023. [paper](https://openreview.net/forum?id=LztkK0UZxS)

   *Sören Becker, Michal Klein, Alexander Neitz, Giambattista Parascandolo, and Niki Kilbertus.*

1. **Elucidating the solution space of extended reverse-time SDE for diffusion models.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.06169)

   *Qinpeng Cui, Xinyi Zhang, Zongqing Lu, and Qingmin Liao.*

1. **ODE-based recurrent model-free reinforcement learning for POMDPs.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.14078)

   *Xuanle Zhao, Duzhen Zhang, Liyuan Han, Tielin Zhang, and Bo Xu.*

1. **A spectral approach for learning spatiotemporal neural differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.16131)

   *Mingtao Xia, Xiangting Li, Qijing Shen, and Tom Chou.*

1. **Invariant physics-informed neural networks for ordinary differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.17053)

   *Shivam Arora, Alex Bihlo, and Francis Valiquette.*

1. **Stability-informed initialization of neural ordinary differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.15890)

   *Theodor Westny, Arman Mohammadi, Daniel Jung, and Erik Frisk.*

1. **U^p-Net: a generic deep learning-based time stepper for parameterized spatio-temporal dynamics.** Computational Mechanics, 2023. [paper](https://link.springer.com/article/10.1007/s00466-023-02295-x)

   *Merten Stender, Jakob Ohlsen, Hendrik Geisler, Amin Chabchoub, Norbert Hoffmann, and Alexander Schlaefer.*

1. **Implicit regularization of deep residual networks towards neural ODEs.** ICLR, 2024. [paper](https://openreview.net/forum?id=AbXGwqb5Ht)

   *Pierre Marion, Yuhan Wu, Michael E. Sander, and Gérard Biau.*

1. **Stable neural stochastic differential equations in analyzing irregular time series data.** ICLR, 2024. [paper](https://openreview.net/forum?id=4VIgNuQ1pY)

   *YongKyung Oh, Dongyoung Lim, and Sungil Kim.*

1. **From Fourier to neural ODEs: Flow matching for modeling complex systems.** ICML, 2024. [paper](https://arxiv.org/abs/2405.11542)

   *Xin Li, Jingdong Zhang, Qunxi Zhu, Chengli Zhao, Xue Zhang, Xiaojun Duan, and Wei Lin.*

### [Large Model](#content)
1. **Prompting in-context operator learning with sensor data, equations, and natural language.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.05061)

   *Liu Yang, Tingwei Meng, Siting Liu, and Stanley J. Osher.*

1. **CrunchGPT: A chatGPT assisted framework for scientific machine learning.** Journal of Machine Learning for Modeling and Computing, 2023. [paper](https://arxiv.org/abs/2306.15551)

   *Varun Kumar, Leonard Gleyzer, Adar Kahana, Khemraj Shukla, and George Em Karniadakis.*

1. **Data-efficient operator learning via unsupervised pretraining and in-context learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15734)

   *Wuyang Chen, Jialin Song, Pu Ren, Shashank Subramanian, Dmitriy Morozov, and Michael W. Mahoney.*

1. **UPS: Towards foundation models for PDE solving via cross-modal adaptation.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.07187)

   *Junhong Shen, Tanya Marwah, and Ameet Talwalkar.*

1. **Towards a foundation model for partial differential equation: Multi-operator learning and extrapolation.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.12355)

   *Jingmin Sun, Yuxuan Liu, Zecheng Zhang, and Hayden Schaeffer.*

1. **Poseidon: Efficient foundation models for PDEs.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.19101)

   *Maximilian Herde, Bogdan Raonić, Tobias Rohner, Roger Käppeli, Roberto Molinaro, Emmanuel de Bézenac, and Siddhartha Mishra.*

1. **PStrategies for pretraining neural operators.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.08473)

   *Anthony Zhou, Cooper Lorsung, AmirPouya Hemmasian, and Amir Barati Farimani.*


## [Mechanism](#content)
### [Benchmark](#content)
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

1. **KoopmanLab: A PyTorch module of Koopman neural operator family for solving partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.01104)

   *Wei Xiong, Muyuan Ma, Pei Sun, and Yang Tian.*

1. **Physics-driven machine learning models coupling PyTorch and Firedrake.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.06871)

   *Nacime Bouziani and David A. Ham.*

1. **BubbleML: A multi-physics dataset and benchmarks for machine learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.14623)

   *Sheikh Md Shakeel Hassan, Arthur Feeney, Akash Dhruv, Jihoon Kim, Youngjoon Suh, Jaiyoung Ryu, Yoonjin Won, and Aparna Chandramowlishwaran.*

1. **LagrangeBench: A Lagrangian fluid nechanics benchmarking suite.** NIPS, 2023. [paper](https://arxiv.org/abs/2309.16342)

   *Artur P. Toshev, Gianluca Galletti, Fabian Fritz, Stefan Adami, and Nikolaus A. Adams.*

1. **Zero coordinate shift: Whetted automatic differentiation for physics-informed operator learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.00860)

   *Kuangdai Leng, Mallikarjun Shankar, and Jeyan Thiyagalingam.*

1. **CFDBench: A comprehensive benchmark for machine learning methods in fluid dynamics.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.05963)

   *Yining Luo, Yingfa Chen, and Zhen Zhang.*

1. **An operator learning framework for spatiotemporal super-resolution of scientific simulations.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.02328)

   *Valentin Duruisseaux and Amit Chakraborty.*

1. **ClimSim: A large multi-scale dataset for hybrid physics-ML climate emulation.** NIPS, 2023. [paper](https://arxiv.org/abs/2306.08754)

   *Busecke, Nora Loose, Charles I Stern, Tom Beucler, Bryce Harrop, Benjamin R Hillman, Andrea Jenney, Savannah Ferretti, Nana Liu, Anima Anandkumar, Noah D Brenowitz, Veronika Eyring, Nicholas Geneva, Pierre Gentine, Stephan Mandt, Jaideep Pathak, Akshay Subramaniam, Carl Vondrick, Rose Yu, Laure Zanna, Tian Zheng, Ryan Abernathey, Fiaz Ahmed, David C Bader, Pierre Baldi, Elizabeth Barnes, Christopher Bretherton, Peter Caldwell, Wayne Chuang, Yilun Han, Yu Huang, Fernando Iglesias-Suarez, Sanket Jantre, Karthik Kashinath, Marat Khairoutdinov, Thorsten Kurth, Nicholas Lutsko, Po-Lun Ma, Griffin Mooers, J. David Neelin, David Randall, Sara Shamekh, Mark A Taylor, Nathan Urban, Janni Yuval, Guang Zhang, and Michael Pritchard.*

1. **Benchmarking the robustness of neural network-based partial differential equation solvers.** ICCAD, 2023. [paper](https://fastmachinelearning.org/iccad2023/file/fastml-iccad-23-final5.pdf)

   *Jiaqi Gu, Mohit Dighamber, Zhengqi Gao, and Duane S. Boning.*

1. **Physics-informed neural networks for advanced modeling.** Journal of Open Source Software, 2024. [paper](https://joss.theoj.org/papers/10.21105/joss.05352)/[Github](https://github.com/mathLab/PINA)

   *Dario Coscia, Anna Ivagnes, Nicola Demo, and Gianluigi Rozza.*

1. **A novel A.I enhanced reservoir characterization with a combined mixture of experts -- NVIDIA modulus based physics informed neural operator forward model.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.14447)

   *Clement Etienam, Yang Juntao, Issam Said, Oleg Ovcharenko, Kaustubh Tangsali, Pavel Dimitrov, and Ken Hester.*

1. **An advanced physics-informed neural operator for comprehensive design optimization of highly-nonlinear systems: An aerospace composites processing case study.** ICML, 2024. [paper](https://openreview.net/forum?id=7eqJypc7RK)

   *Milad Ramezankhani, Anirudh Deodhar, Rishi Yash Parekh, and Dagnachew Birru.*

### [Investigation](#content)
1. **Characterizing possible failure modes in physics-informed neural networks.** NIPS, 2021. [paper](https://openreview.net/forum?id=a2Gr9gNFD-J)

   *Aditi Krishnapriyan, Amir Gholami, Shandian Zhe, Robert Kirby, and Michael W. Mahoney.*

1. **Understanding and mitigating gradient flow pathologies in physics-informed neural networks.** SIAM Journal on Scientific Computing, 2021. [paper](https://epubs.siam.org/doi/10.1137/20M1318043)

   *Sifan Wang, Yujun Teng, and Paris Perdikaris.*

1. **When and why PINNs fail to train: A neural tangent kernel perspective.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S002199912100663X)

   *SifanWang, XinlingYu, and Paris Perdikaris.*

1. **When do extended physics-informed neural networks (XPINNs) improve generalization?** SIAM Journal on Scientific Computing, 2022. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1447039)

   *Zheyuan Hu, Ameya D. Jagtap, George Em Karniadakis, and Kenji Kawaguchi.*

1. **MARS: A method for the adaptive removal of stiffness in PDEs.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122006878#!)

   *Laurent Duchemin and Jen Eggers.*

1. **Learning similarity metrics for numerical simulations.** ICML, 2020. [paper](https://proceedings.mlr.press/v119/kohl20a.html)

   *Georg Kohl, Kiwon Um, and Nils Thuerey.*

1. **A curriculum-training-based strategy for distributing collocation points during physics-informed neural network training.** NIPS, 2021. [paper](https://arxiv.org/abs/2211.11396)

   *Marcus Münzer and Chris Bard.*

1. **Parametric complexity bounds for approximating PDEs with neural networks.** NIPS, 2021. [paper](https://proceedings.neurips.cc/paper/2021/hash/7edccc661418aeb5761dbcdc06ad490c-Abstract.html)

   *Tanya Marwah, Zachary Lipton, and Andrej Risteski.*

1. **Respecting causality for training physics-informed neural networks.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524000690)

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

1. **Separable PINN: Mitigating the curse of dimensionality in physics-informed neural networks.** NIPS, 2022. [paper](https://openreview.net/forum?id=jGk3DgkHB_)

   *Junwoo Cho, Seungtae Nam, Hyunmo Yang, Seok-Bae Yun, Youngjoon Hong, and Eunbyung Park.*

1. **A curriculum-training-based strategy for distributing collocation points during physics-informed neural network training.** NIPS, 2022. [paper](https://arxiv.org/pdf/2211.11396.pdf)

   *Marcus Münzer and Chris Bard.*

1. **Robustness of physics-informed neural networks to noise in sensor data.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.12042)

   *Jian Cheng Wong, Pao-Hsiung Chiu, Chin Chun Ooi, and My Ha Da.* 

1. **Investigations on convergence behaviour of physics informed neural networks across spectral ranges and derivative orders.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.02790)

   *Mayank Deshpande, Siddharth Agarwal, Vukka Snigdha, and Arya Kumar Bhattacharya.* 

1. **Stochastic projection based approach for gradient free physics informed learning.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522007988)

   *Navaneeth N. and Souvik Chakraborty.* 

1. **Temporal consistency loss for physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.13262)

   *Sukirt Thakur, Maziar Raissi, Harsa Mitra, and Arezoo Ardekani.* 

1. **Can physics-informed neural networks beat the finite element method?** arXiv, 2023. [paper](https://arxiv.org/abs/2302.04107)

   *Tamara G. Grossmann, Urszula Julia Komorowska, Jonas Latz, and Carola-Bibiane Schönlieb.* 

1. **LSA-PINN: Linear boundary connectivity loss for solving PDEs on complex geometry.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.01518)

   *Jian Cheng Wong, Pao-Hsiung Chiu, Chinchun Ooi, and My Ha Dao, and Yew-Soon Ong.* 

1. **On the Hyperparameters influencing a PINN’s generalization beyond the training domain.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.07557)

   *Andrea Bonfanti, Roberto Santana, Marco Ellero, and Babak Gholami.* 

1. **DPM: A novel training method for physics-informed neural networks in extrapolation.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16992)

   *Jungeun Kim, Kookjin Lee, Dongeun Lee, Sheo Yon Jhin, and Noseong Park.* 

1. **Guiding continuous operator learning through physics-based boundary constraints.** ICLR, 2023. [paper](https://openreview.net/forum?id=gfWNItGOES6)

   *Nadim Saad, Gaurav Gupta, Shima Alizadeh, and Danielle C. Maddix.* 

1. **Probing optimisation in physics-informed neural networks.** ICLR, 2023. [paper](https://arxiv.org/abs/2303.15196)

   *Nayara Fonseca, Veronica Guidetti, and Will Trojak.*

1. **Nearly optimal VC-dimension and Pseudo-dimension bounds for deep neural network derivatives.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.08466)

   *Yahong Yang, Haizhao Yang, and Yang Xiang.*

1. **PDE+: Enhancing generalization via PDE with adaptive distributional diffusion.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.15835)

   *Yige Yuan, Bingbing Xu, Bo Lin, Liang Hou, Fei Sun, Huawei Shen, and Xueqi Cheng.*

1. **Towards foundation models for scientific machine learning: Characterizing scaling and transfer behavior.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.00258)

   *Shashank Subramanian, Peter Harrington, Kurt Keutzer, Wahid Bhimji, Dmitriy Morozov, Michael Mahoney, and Amir Gholami.*

1. **Understanding and mitigating extrapolation failures in physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.09478)

   *Lukas Fesser, Richard Qiu, and Luca D'Amico-Wong.*

1. **Physics-informed neural network based on a new adaptive gradient descent algorithm for solving partial differential equations of flow problems.** Physics of Fluids, 2023. [paper](https://pubs.aip.org/aip/pof/article/35/6/063608/2899773)

   *Xiaojian Li, Yuhao Liu, and Zhengxian Liu.*

1. **The curse of dimensionality in operator learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.15924v1)

   *Samuel Lanthaler and Andrew M. Stuart.*

1. **Inverse evolution layers: Physics-informed regularizers for deep neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.07344)

   *Chaoyu Liu, Zhonghua Qiao, Chao Li, and Carola-Bibiane Schönlieb.*

1. **Positional embeddings for solving PDEs with evolutional deep neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.03461)

   *Mariella Kast and Jan S Hesthaven.*

1. **Learning specialized activation functions for physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.04073)

   *Honghui Wang, Lu Lu, Shiji Song, and Gao Huang.*

1. **Size lowerbounds for deep operator networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.06338)

   *Anirbit Mukherjee and Amartya Roy.*

1. **How important are specialized transforms in neural operators?** arXiv, 2023. [paper](https://arxiv.org/abs/2308.09293)

   *Ritam Majumdar, Shirish Karande, and Lovekesh Vig.*

1. **Neural oscillators for generalization of physics-informed machine learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.08989)

   *Taniya Kapoor, Abhishek Chandra, Daniel M. Tartakovsky, Hongrui Wang, Alfredo Nunez, and Rolf Dollevoet.*

1. **Deep neural networks with ReLU, leaky ReLU, and softplus activation provably overcome the curse of dimensionality for Kolmogorov partial differential equations with Lipschitz nonlinearities in the L^p-sense.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.13722)

   *Julia Ackermann, Arnulf Jentzen, Thomas Kruse, Benno Kuckuck, and Joshua Lee Padgett.*

1. **An operator preconditioning perspective on training in physics-informed machine learning.** ICLR, 2024. [paper](https://openreview.net/forum?id=WWlxFtR5sV)

   *Tim De Ryck, Florent Bonnet, Siddhartha Mishra, and Emmanuel de Bézenac.*

1. **A trial solution for imposing boundary conditions of partial differential equations in physics-informed neural networks.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623014203)

   *Seyedalborz Manavi, Ehsan Fattahi, and Thomas Becker.*

1. **Multiple physics pretraining for physical surrogate models.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.02994)

   *Michael McCabe, Bruno Régaldo-Saint Blancard, Liam Holden Parker, Ruben Ohana, Miles Cranmer, Alberto Bietti, Michael Eickenberg, Siavash Golkar, Geraud Krawezik, Francois Lanusse, Mariel Pettee, Tiberiu Tesileanu, Kyunghyun Cho, and Shirley Ho.*

1. **Lie point symmetry and physics informed networks.** NIPS, 2023. [paper](https://openreview.net/forum?id=VlUf77e9cR)

   *Tara Akhound-Sadegh, Laurence Perreault-Levasseur, Johannes Brandstetter, Max Welling, and Siamak Ravanbakhsh.*

1. **Stacked networks improve physics-informed training: Applications to neural networks and deep operator networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.06483)

   *Amanda A Howard, Sarah H Murphy, Shady E Ahmed, and Panos Stinis.*

1. **Is the neural tangent kernel of PINNs deep learning general partial differential equations always convergent?** Physica D: Nonlinear Phenomena, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S016727892300341X)

   *Zijian Zhou and Zhenya Yan.*

1. **Can physics informed neural operators self improve?** NIPS, 2023. [paper](https://openreview.net/forum?id=Lhm15nDeGH)

   *Ritam Majumdar, Ritam_Majumdar, Amey Varhade, Shirish Karande, and Lovekesh Vig.*

1. **Bias-variance trade-off in physics-informed neural networks with randomized smoothing for high-dimensional PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.15283)

   *Zheyuan Hu, Zhouhao Yang, Yezhen Wang, George Em Karniadakis, and Kenji Kawaguchi.*

1. **From plateaus to progress: Unveiling training dynamics of PINNs.** NIPS, 2023. [paper](https://ml4physicalsciences.github.io/2023/files/NeurIPS_ML4PS_2023_187.pdf)

   *Rahil Pandya, Panos Parpas, and Daniel Lengyel.*

1. **An integrated framework for accelerating reactive flow simulation using GPU and machine learning models.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.13513)

   *Runze Mao, Yingrui Wang, Min Zhang, Han Li, Jiayang Xu, Xinyu Dong, Yan Zhang, and Zhi X. Chen.*

1. **Greedy training algorithms for neural networks and applications to PDEs.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123001791)

   *Jonathan W. Siegel, Qingguo Hong, Xianlin Jin, Wenrui Hao, and Jinchao Xu.*

1. **How much can one learn a partial differential equation from its solution?** Foundations of Computational Mathematics, 2023. [paper](https://link.springer.com/article/10.1007/s10208-023-09620-z)

   *Yuchen He, Hongkai Zhao, and Yimin Zhong.*

1. **Random feature neural networks learn black-Scholes type PDEs without curse of dimensionality,** JMLR, 2023. [paper](https://www.jmlr.org/papers/v24/21-0987.html)

   *Lukas Gonon.*

1. **Generalizable neural physics solvers by baldwinian evolution.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.03243)

   *Jian Cheng Wong, Chin Chun Ooi, Abhishek Gupta, Pao-Hsiung Chiu, Joshua Shao Zheng Low, My Ha Dao, and Yew-Soon Ong.*

1. **Mind the gap: Constraining physics-informed neural operators to improve the quality of auto-regressive predictions.** AIAA, 2024. [paper](https://arc.aiaa.org/doi/abs/10.2514/6.2024-0772)

   *Sean F. Current, Vilas J. Shinde, Saket Gurukar, Datta V. Gaitonde, and Srinivasan Parthasarathy.*

1. **Refined generalization analysis of the deep Ritz method and physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.12526)

   *Xianliang Xu and Zhongyi Huang.*

1. **PirateNets: Physics-informed deep learning with residual adaptive networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.00326)

   *Sifan Wang, Bowen Li, Yuhan Chen, and Paris Perdikaris.*

1. **An operator learning perspective on parameter-to-observable maps.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.06031)

   *Daniel Zhengyu Huang, Nicholas H. Nelsen, and Margaret Trautner.*

1. **Architectural strategies for the optimization of physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.02711)

   *Hemanth Saratchandran, Shin-Fang Chng, and Simon Lucey.*

1. **Closure discovery for coarse-grained partial differential equations using multi-agent reinforcement learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.00972)

   *Jan-Philipp von Bassewitz, Sebastian Kaltenbach, and Petros Koumoutsakos.*

1. **Kolmogorov n-widths for multitask physics-informed machine learning (PIML) methods: Towards robust metrics.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.11126v1)

   *Michael Penwarden, Houman Owhadi, and Robert M. Kirby.*

1. **Parametric encoding with attention and convolution mitigate spectral bias of neural partial differential equation solvers.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.15652)

   *Mehdi Shishehbor, Shirin Hosseinmardi, and Ramin Bostanabad.*

1. **Physics-informed neural networks: Minimizing residual loss with wide networks and effective activations.** IJCAI, 2024. [paper](https://arxiv.org/abs/2405.01680)

   *Nima Hosseini Dashtbayaz, Ghazal Farhani, Boyu Wang, and Charles X. Ling.*

1. **Unveiling the optimization process of physics informed neural networks: How accurate and competitive can pinns be?** arXiv, 2024. [paper](https://arxiv.org/abs/2403.15652)

   *Jorge F. Urbán, Petros Stefanou, and José A. Pons.*

1. **Loss jump during loss switch in solving PDEs with neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.03095)

   *Zhiwei Wang, Lulu Zhang, Zhongwang Zhang, and Zhi-Qin John Xu.*

1. **CEENs: Causality-enforced evolutional networks for solving time-dependent partial differential equations.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524002925)

   *Jeahan Jung, Heechang Kim, Hyomin Shin, and Minseok Choi.*

1. **Deep neural networks with ReLU, leaky ReLU, and softplus activation provably overcome the curse of dimensionality for space-time solutions of semilinear partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.10876)

   *Julia Ackermann, Arnulf Jentzen, Benno Kuckuck, and Joshua Lee Padgett.*

### [Domain Adaptation](#content)
1. **Meta-auto-decoder for solving parametric partial differential equations.** NIPS, 2022. [paper](https://openreview.net/pdf?id=PwlW5Jri1Xt) 

   *Xiang Huang, Zhanhong Ye, Hongsheng Liu, Beiji Shi, Zidong Wang, Kang Yang, Yang Li, Bingya Weng, Min Wang, Haotian Chu, Jing Zhou, Fan Yu, Bei Hua, Lei Chen, and Bin Dong.*

1. **Transfer learning with physics-informed neural networks for efficient simulation of branched flows.** NIPS, 2022. [paper](https://arxiv.org/abs/2211.00214) 

   *Raphaël Pellegrin, Blake Bullwinkel, Marios Mattheakis, and Pavlos Protopapas.*

1. **Identifying physical law of hamiltonian systems via meta-learning.** ICLR, 2021. [paper](https://openreview.net/pdf?id=45NZvF1UHam) 

   *Seungjun Lee, Haesang Yang, and Woojae Seong.*

1. **One-shot learning for solution operators of partial differential equations.** ICLR, 2021. [paper](https://arxiv.org/abs/2104.05512) 

   *Lu Lu, Haiyang He, Priya Kasimbeg, Rishikesh Ranade, and Jay Pathak.*

1. **A metalearning approach for physics-informed neural networks (PINNs): Application to parameterized PDEs.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123000074)

   *Michael Penwarden, Shandian Zhe, Akil Narayan, and Robert M.Kirby.*

1. **Meta-MgNet: Meta multigrid networks for solving parameterized partial differential equations.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122000584)

   *Yuyan Chen, Bin Dong, and Jinchao Xu.*

1. **Mosaic flows: A transferable deep learning framework for solving PDEs on unseen domains.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S004578252100668X)

   *Hengjie Wang, Robert Planas, Aparna Chandramowlishwaran, and Ramin Bostanabad.*

1. **Meta-learning PINN loss functions.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122001838)

   *Apostolos F Psaros,Kenji Kawaguchi, and George Em Karniadakis.*

1. **HyperPINN: Learning parameterized differential equations with physics-informed hypernetworks.** NIPS, 2021. [paper](https://openreview.net/pdf?id=LxUuRDUhRjM)

   *Filipe de Avila Belbute-Peres, Yifan Chen, and Fei Sha.*

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

1. **Transfer learning based physics-informed neural networks for solving inverse problems in engineering structures under different loading scenarios.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522008088)

   *Chen Xu, Ba Trung Cao, Yong Yuan, and Günther Meschke.*

1. **TransNet: Transferable neural networks for partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.11701)

   *Zezhong Zhang, Feng Bao, Lili Ju, and Guannan Zhang.*

1. **Adaptive weighting of Bayesian physics informed neural networks for multitask and multiscale forward and inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.12697)

   *Sarah Perez, Suryanarayana Maddu, Ivo F. Sbalzarini, and Philippe Poncet.*

1. **GPT-PINN: Generative pre-trained physics-informed neural networks toward non-intrusive meta-learning of parametric PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.14878)

   *Yanlai Chen and Shawn Koohy.*

1. **Gradient-enhanced physics-informed neural networks based on transfer learning for inverse problems of the variable coefficient differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.08310)

   *Shuning Lin and Yong Chen.*

1. **Towards foundation models for scientific machine learning: Characterizing scaling and transfer behavior.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.00258)

   *Shashank Subramanian, Peter Harrington, Kurt Keutzer, Wahid Bhimji, Dmitriy Morozov, Michael Mahoney, and Amir Gholami.*

1. **Adaptive transfer learning for PINN.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123003868)

   *Yang Liu, Wen Liu, Xunshi Yan, Shuaiqi Guo, and Chen-an Zhang.*

1. **Meta learning of interface conditions for multi-domain physics-informed neural networks.** ICML, 2023. [paper](https://openreview.net/forum?id=e694Xvz6Q6)

   *Shibo Li, Michael Penwarden, Yiming Xu, Conor Tillinghast, Akil Narayan, Robert Kirby, and Shandian Zhe.*

1. **A sequential meta-transfer (SMT) learning to combat complexities of physics-informed neural networks: Application to composites autoclave processing.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.06447)

   *Milad Ramezankhani and Abbas S. Milani.*

1. **HyperLoRA for PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.09290)

   *Ritam Majumdar, Vishal Jadhav, Anirudh Deodhar, Shirish Karande, Lovekesh Vig, and Venkataramana Runkana.*

1. **In-context operator learning with data prompts for differential equation problems.** PNAS, 2023. [paper](https://www.pnas.org/doi/abs/10.1073/pnas.2310142120)

   *Liu Yang, Siting Liu, Tingwei Meng, and Stanley J. Osher.*

1. **SONets: Sub-operator learning enhanced neural networks for solving parametric partial differential equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123006319)

   *Xiaowei Jin and Hui Li.*

1. **Hypernetwork-based meta-learning for low-rank physics-informed neural networks.** NIPS, 2023. [paper](https://arxiv.org/abs/2310.09528)

   *Woojin Cho, Kookjin Lee, Donsub Rim, and Noseong Park.*

1. **Meta-learning of physics-informed neural networks for efficiently solving newly given PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.13270)

   *Tomoharu Iwata, Yusuke Tanaka, and Naonori Ueda.*

1. **Generalized one-shot transfer learning of linear ordinary and partial differential equations.** NIPS, 2023. [paper](https://openreview.net/pdf?id=x2Mscu1b7H)

   *Tomoharu Iwata, Yusuke Tanaka, and Naonori Ueda.*

1. **One-shot transfer learning for nonlinear ODEs.** NIPS, 2023. [paper](https://openreview.net/forum?id=mcIbqPMKCU)

   *Wanzhou Lei, Pavlos Protopapas, and Joy Parikh.*

1. **PDE generalization of in-context operator networks: A study on 1D scalar nonlinear conservation laws.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.07364)

   *Liu Yang and Stanley J. Osher.*

1. **DIMON: Learning solution operators of partial differential equations on a diffeomorphic family of domains.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.07250)

   *Minglang Yin, Nicolas Charon, Ryan Brody, Lu Lu, Natalia Trayanova, and Mauro Maggioni.*

1. **Transferable neural networks for partial differential equations.** Journal of Scientific Computing, 2024. [paper](https://link.springer.com/article/10.1007/s10915-024-02463-y)

   *Zezhong Zhang, Feng Bao, Lili Ju, and Guannan Zhang.*

1. **Using uncertainty quantification to characterize and improve out-of-domain learning for PDEs.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.10642)

   *S. Chandra Mouli, Danielle C. Maddix, Shima Alizadeh, Gaurav Gupta, Andrew Stuart, Michael W. Mahoney, and Yuyang Wang.*

1. **Neural parameter regression for explicit representations of PDE solution operators.** ICLR, 2024. [paper](https://arxiv.org/abs/2403.12764)

   *Konrad Mundinger, Max Zimmer, and Sebastian Pokutta.*

1. **Deep operator networks for bioheat transfer problems with parameterized laser source functions.**  International Journal of Heat and Mass Transfe, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0017931024004903)

   *Aditya Roy, Andrew DuPlissis, Biswajit Mishra, and Adela Ben-Yakar.*

1. **Vectorized conditional neural fields: A framework for solving time-dependent parametric partial differential equations.** ICML, 2024. [paper](https://arxiv.org/abs/2406.03919)

   *Jan Hagnberger, Marimuthu Kalimuthu, Daniel Musekamp, and Mathias Niepert.*

1. **Base models for parabolic partial differential equations.** UAI, 2024. [paper](https://openreview.net/forum?id=TLYNkysFB3)

   *Xingzi Xu, Ali Hasan, Jie Ding, and Vahid Tarokh.*

1. **DeltaPhi: Learning physical trajectory residual for PDE solving.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.09795)

   *Xihang Yue, Linchao Zhu, and Yi Yang.*

1. **DATS: Difficulty-aware task sampler for meta-learning physics-informed neural networks.** ICLR, 2024. [paper](https://openreview.net/forum?id=EvyYFSxdgB)

   *Maryam Toloubidokhti, Yubo Ye, Ryan Missel, Xiajun Jiang, Nilesh Kumar, Ruby Shrestha, and Linwei Wang.*

1. **Using uncertainty quantification to characterize and improve out-of-domain learning for PDEs.** ICML, 2024. [paper](https://openreview.net/forum?id=Y50K6DSrWo)

   *S Chandra Mouli, Danielle C. Maddix, Shima Alizadeh, Gaurav Gupta, Andrew Stuart, Michael W. Mahoney, and Bernie Wang.*

1. **Base models for parabolic partial differential equations.** UAI, 2024. [paper](https://openreview.net/forum?id=TLYNkysFB3)

   *Xingzi Xu, Ali Hasan, Jie Ding, and Vahid Tarokh.*

### [Loss Function](#content)
1. **Adaptive activation functions accelerate convergence in deep and physics-informed neural networks.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119308411)

   *Ameya D.Jagtap, KenjiKawaguchi, and George Em Karniadakis.*

1. **Adaptive deep neural networks methods for high-dimensional partial differential equations.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122002947#)

   *Shaojie Zeng, Zong Zhang, and Qingsong Zou.*

1. **Self-adaptive loss balanced Physics-informed neural networks.** Neurocomputing, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S092523122200546X)

   *Zixue Xiang, Wei Peng, Xu Liu, and Wen Yao.*

1. **Multi-objective loss balancing for physics-informed deep learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.09813)

   *Rafael Bischof and Michael Kraus.*

1. **Self-scalable Tanh (Stan): Faster convergence and better generalization in physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.12589)

   *Raghav Gnanasambandam, Bo Shen, Jihoon Chung, Xubo Yue, and Zhenyu (James) Kong.*

1. **Is L2 physics-informed loss always suitable for training physics-informed neural network?** arXiv, 2022. [paper](https://arxiv.org/abs/2206.02016)

   *Chuwei Wang, Shanda Li, Di He, and Liwei Wang.*

1. **Loss landscape engineering via data regulation on PINNs.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.07843)

   *Vignesh Gopakumar, Stanislas Pamela, and Debasmita Samaddar.*

1. **Implicit stochastic gradient descent for training physics-informed neural networks.** AAAI, 2023. [paper](https://arxiv.org/abs/2303.01767)

   *Ye Li, Songcan Chen, and Shengjun Huang.*

1. **About optimal loss function for training physics-informed neural networks under respecting causality.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.02282)

   *Vasiliy A. Es'kin, Danil V. Davydov, Ekaterina D. Egorova, Alexey O. Malkhanov, Mikhail A. Akhukov, and Mikhail E. Smorkalov.*

1. **Fourier-MIONet: Fourier-enhanced multiple-input neural operators for multiphase modeling of geological carbon sequestration.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.04778)

   *Zhongyi Jiang, Min Zhu, Dongzhuo Li, Qiuzi Li, Yanhua O. Yuan, and Lu Lu.*

1. **Learning from integral losses in physics informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.17387)

   *Ehsan Saleh, Saba Ghaffari, Timothy Bretl, Luke Olson, and Matthew West.*

1. **A symmetry group based supervised learning method for solving partial differential equations.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523003055)

   *Zhiyong Zhang, Shengjie Cai, and Hui Zhang.*

1. **Loss jump during loss switch in solving PDEs with neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.03095)

   *Zhiwei Wang, Lulu Zhang, Zhongwang Zhang, and Zhi-Qin John Xu.*

1. **Godunov loss functions for modelling of hyperbolic conservation laws.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.11674)

   *R. G. Cassia and R. R. Kerswell.*

1. **Kronecker-factored approximate curvature for physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.15603)

   *Felix Dangel, Johannes Müller, and Marius Zeinhofer.*

1. **Astral: Training physics-informed neural networks with error majorants.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.02645)

   *Vladimir Fanaskov, Tianchi Yu, Alexander Rudikov, and Ivan Oseledets.*

1. **Physics-Informed Parallel Neural Networks with self-adaptive loss weighting for the identification of continuous structural systems.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524002986)

   *Rui Zhang, Gordon P. Warn, and Aleksandra Radlińska.*

1. **A practical PINN framework for multi-scale problems with multi-magnitude loss terms.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999124003619)

   *Yong Wang, Yanzhong Yao, Jiawei Guo, and Zhiming Gao.*

1. **Neural operators meet conjugate gradients: The FCG-NO method for efficient PDE solving.** ICML, 2024. [paper](https://openreview.net/forum?id=J0ty1o7nCj)

   *Alexander Rudikov, Vladimir Fanaskov, Ekaterina Muravleva, Yuri M. Laevsky, and Ivan Oseledets.*

### [Sampling](#content)
1. **ADLGM: An efficient adaptive sampling deep learning Galerkin method.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123000396)

   *Andreas C.Aristotelous, Edward C.Mitchell, and Vasileios Maroulasb.*

1. **DMIS: Dynamic mesh-based importance sampling for training physics-informed neural networks.** AAAI, 2023. [paper](https://arxiv.org/abs/2211.13944)

   *Zijiang Yang, Zhongwei Qiu, and Dongmei Fu.*

1. **A comprehensive study of non-adaptive and residual-based adaptive sampling for physics-informed neural networks.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782522006260)

   *Chenxi Wua, Min Zhua, Qinyang Tan, YadhKartha, and Lu Lu.*

1. **Mitigating propagation failures in PINNs using evolutionary sampling.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.02338)

   *Arka Daw, Jie Bu, Sifan Wang, Paris Perdikaris, and Anuj Karpatne.*

1. **Residual-quantile adjustment for adaptive training of physics-informed neural network.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.05315)

   *Jiayue Han, Zhiqiang Cai, Zhiyou Wu, and Xiang Zhou.*

1. **Adversarial sampling for solving differential equations with neural networks.** NIPS, 2021. [paper](https://openreview.net/forum?id=EeBH6OZFFx)

   *Kshitij Parwani and Pavlos Protopapas.*

1. **A novel adaptive causal sampling method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.12914)

   *Jia Guo, Haifeng Wang, and Chenping Hou.*

1. **Physics-informed neural networks with residual/gradient-based adaptive sampling methods for solving PDEs with sharp solutions.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.08035)

   *Zhiping Mao and Xuhui Meng.*

1. **Active learning based sampling for high-dimensional nonlinear partial differential equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122009111)

   *Wenhan Gao and Chunmei Wang.*

1. **Adversarial adaptive sampling: Unify PINN and optimal yransport for the approximation of PDEs.** ICLR, 2024. [paper](https://openreview.net/forum?id=7QI7tVrh2c)

   *Kejun Tang, Jiayu Zhai, Xiaoliang Wan, and Chao Yang.*

1. **Coupling parameter and particle dynamics for adaptive sampling in neural Galerkin schemes.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.15630)

   *Yuxiao Wen, Eric Vanden-Eijnden, and Benjamin Peherstorfer.*

1. **Mitigating propagation failures in physics-informed neural networks using retain-resample-release (R3) sampling.** ICML, 2023. [paper](https://openreview.net/forum?id=rhvb4kprWB)

   *Arka Daw, Jie Bu, Sifan Wang, Paris Perdikaris, and Anuj Karpatne.*

1. **Good lattice training: Physics-informed neural networks accelerated by number theory.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.13869)

   *Takashi Matsubara and Takaharu Yaguchi.*

1. **Adaptive importance sampling for Deep Ritz.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.17185)

   *Xiaoliang Wan, Tao Zhou, and Yuancheng Zhou.*

1. **Adversarial adaptive sampling: Unify PINN and optimal transport for the approximation of PDEs.** ICLR, 2024. [paper](https://openreview.net/forum?id=7QI7tVrh2c)

   *Kejun Tang, Jiayu Zhai, Xiaoliang Wan, and Chao Yang.*

1. **DAS-PINNs: A deep adaptive sampling method for solving high-dimensional partial differential equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999122009317)

   *Kejun Tang, Xiaoliang Wan, and Chao Yang.*

1. **Deep adaptive sampling for surrogate modeling without labeled data.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.11283)

   *Xili Wang, Kejun Tang, Jiayu Zhai, Xiaoliang Wan, and Chao Yang.*

1. **Physics-informed neural networks for sampling.** ICLR, 2024. [paper](https://openreview.net/forum?id=KwHPBIGkET)

   *Jingtong Sun, Julius Berner, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **PINNACLE: PINN adaptive collocation and experimental points selection.** ICLR, 2024. [paper](https://openreview.net/forum?id=GzNaCp6Vcg)

   *Gregory Kang Ruey Lau, Apivich Hemachandra, See-Kiong Ng, and Bryan Kian Hsiang Low.*

1. **Annealed adaptive importance sampling method in PINNs for solving high dimensional partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.03433)

   *Zhengqi Zhang, Jing Li, and Bin Liu.*

1. **Solving partial differential equations with sampled neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.20836)

   *Chinmay Datar, Taniya Kapoor, Abhishek Chandra, Qing Sun, Iryna Burak, Erik Lien Bolager, Anna Veselovska, Massimo Fornasier, and Felix Dietrich.*

1. **A Gaussian mixture distribution-based adaptive sampling method for physics-informed neural networks.** EAAI, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S095219762400928X)

   *Yuling Jiao, Di Li, Xiliang Lu, Jerry Zhijian Yang, and Cheng Yuan.*

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

1. **Fixed-budget online adaptive mesh learning for physics-informed neural networks. Towards parameterized problem inference.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.11776)

   *Thi Nguyen Khoa Nguyen, Thibault Dairay, Raphaël Meunier, Christophe Millet, and Mathilde Mougeot.*

1. **Learning controllable adaptive simulation for multi-resolution physics.** ICLR, 2023. [paper](https://openreview.net/forum?id=PbfgkZ2HdbE)

   *Tailin Wu, Takashi Maruyama, Qingqing Zhao, Gordon Wetzstein, and Jure Leskovec.*

1. **A closest point method for surface PDEs with interior boundary conditions for geometry processing.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.04711)

   *Nathan King, Haozhe Su, Mridul Aanjaneya, Steven Ruuth, and Christopher Batty.*

1. **Efficient training of physics-informed neural networks with direct grid refinement algorithm.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.08293)

   *Shikhar Nilabh and Fidel Grandia.*

1. **Redefining Super-Resolution: Fine-mesh PDE predictions without classical simulations.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.09740)

   *Rajat Kumar Sarkar, Ritam Majumdar, Vishal Jadhav, Sagar Srinivas Sakhinana, and Venkataramana Runkana.*

1. **MMPDE-Net and moving sampling physics-informed neural networks based on moving mesh method.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.16167)

   *Yu Yang, Qihong Yang, Yangtao Deng, and Qiaolin He.*

1. **Reinforcement learning for adaptive mesh refinement.** AISTATS, 2023. [paper](https://proceedings.mlr.press/v206/yang23e.html)

   *Jiachen Yang, Tarik Dzanic, Brenden Petersen, Jun Kudo, Ketan Mittal, Vladimir Tomov, Jean-Sylvain Camier, Tuo Zhao, Hongyuan Zha, Tzanio Kolev, Robert Anderson, and Daniel Faissol.*

1. **Multiscale graph neural networks with adaptive mesh refinement for accelerating mesh-based simulations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.08863)

   *Roberto Perera and Vinamra Agrawal.*

1. **Learning mesh motion techniques with application to fluid–structure interaction.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S0045782524001464)

   *Johannes Haubner, Ottar Hellan, Marius Zeinhofer, and Miroslav Kuchta.*

1. **Learning time-dependent PDE via graph neural networks and deep operator network for robust accuracy on irregular grids.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.08187v1)

   *Sung Woong Cho, Jae Yong Lee, and Hyung Ju Hwang.*

1. **Physics-informed mesh-independent deep compositional operator network.** arXiv, 2024. [paper](https://.arxiv.org/abs/2404.13646)

   *Weiheng Zhong and Hadi Meidani.*

1. **End-to-end mesh optimization of a hybrid deep learning black-box PDE solver.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.11766)

   *Shaocong Ma, James Diffenderfer, Bhavya Kailkhura, and Yi Zhou.*

1. **RoPINN: Region optimized physics-informed neural networks.** arXiv, 2024. [paper](https://.arxiv.org/abs/2405.14369)

   *Haixu Wu, Huakun Luo, Yuezhou Ma, Jianmin Wang, and Mingsheng Long.*

1. **UM2N: Towards universal mesh movement networks.** arXiv, 2024. [paper](https://.arxiv.org/abs/2407.00382)

   *Mingrui Zhang, Chunyang Wang, Stephan Kramer, Joseph G. Wallwork, Siyi Li, Jiancheng Liu, Xiang Chen, and Matthew D. Piggott.*

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

1. **NeuralStagger: Accelerating physics constrained neural PDE solver with spatial-temporal decomposition.** ICML, 2023. [paper](https://openreview.net/forum?id=YeDBpVhq4M)

   *Xinquan Huang, Wenlei Shi, Qi Meng, Yue Wang, Xiaotian Gao, Jia Zhang, and Tieyan Liu.*

1. **Augmenting physical models with deep networksfor complex dynamics forecasting.** Journal of Statistical Mechanics: Theory and Experiment, 2021. [paper](https://iopscience.iop.org/article/10.1088/1742-5468/ac3ae5/meta)

   *Yuan Yin, Vincent Le Guen, Jérémie Dona, Emmanuel de Bézenac, Ibrahim Ayed, Nicolas Thome, and Patrick Gallinari.*

1. **LordNet: Learning to solve parametric partial differential equations without simulated data.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.09418)

   *Wenlei Shi, Xinquan Huang, Xiaotian Gao, Xinran Wei, Jia Zhang, Jiang Bian, Mao Yang, and Tieyan Liu.*

1. **An optimisation–based domain–decomposition reduced order model for the incompressible Navier-Stokes equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.14528)

   *Ivan Prusak, Monica Nonino, Davide Torlo, Francesco Ballarin, and Gianluigi Rozza.*

1. **NUNO: A general gramework for learning parametric PDEs with non-uniform data.** ICML, 2023. [paper](https://arxiv.org/abs/2305.18694v2)

   *Songming Liu, Zhongkai Hao, Chengyang Ying, Hang Su, Ze Cheng, and Jun Zhu.*

1. **Enhancing training of physics-informed neural networks using domain-decomposition based preconditioning strategies.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.17648)

   *Alena Kopaničáková, Hardik Kothari, George Em Karniadakis, and Rolf Krause.*

1. **Multilevel domain decomposition-based architectures for physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.05486)

   *Victorita Dolean, Alexander Heinlein, Siddhartha Mishra, and Ben Moseley.*

1. **Friedrichs' systems discretized with the Discontinuous Galerkin method: Domain decomposable model order reduction and Graph Neural Networks approximating vanishing viscosity solutions.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.03378)

   *Francesco Romor, Davide Torlo, and Gianluigi Rozza.*

1. **A deep domain decomposition method based on Fourier features.** Journal of Computational and Applied Mathematics, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0377042722005611)

   *Sen Li, Yingzhi Xia, Yu Liu, and Qifeng Liao.*

1. **A unified scalable framework for causal sweeping strategies for physics-informed neural networks (PINNs) and their temporal decompositions.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.14227)

   *Michael Penwarden, Ameya D. Jagtap, Shandian Zhe, George Em Karniadakis, and Robert M. Kirby.* 

1. **A generalized Schwarz-type non-overlapping domain decomposition method using physics-constrained neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.12435)

   *Shamsulhaq Basir and Inanc Senocak.*

1. **Breaking boundaries: Distributed domain decomposition with scalable physics-informed neural PDE solvers.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.14258)

   *Arthur Feeney, Zitong Li, Ramin Bostanabad, and Aparna Chandramowlishwaran.*

1. **Efficient learning of PDEs via Taylor expansion and sparse decomposition into value and Fourier domains.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.07344)

   *Md Nasim and Yexiang Xue.*

1. **Adaptive task decomposition physics-informed neural networks.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523006850)

   *Jianchuan Yang, Xuanqi Liu, Yu Diao, Xi Chen, and Haikuo Hu.*

1. **PF-DMD: Physics-fusion dynamic mode decomposition for accurate and robust forecasting of dynamical systems with imperfect data and physics.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.15604)

   *Yuhui Yin, Chenhui Kou, Shengkun Jia, Lu Lu, Xigang Yuan, and Yiqing Luo.*

1. **Subspace decomposition based DNN algorithm for elliptic type multi-scale PDEs.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123003376)

   *Xian Li, Zhiqin John Xu, and Lei Zhang.*

1. **Adaptive deep Fourier residual method via overlapping domain decomposition.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.04663)

   *Jamie M. Taylor, Manuela Bastidas, Victor M. Calo, and David Pardo.*

### [Disentangle](#content)
1. **PDE-driven spatiotemporal disentanglement.** ICLR, 2021. [paper](https://openreview.net/forum?id=vLaHRtHvfFp)

   *Jérémie Donà, Jean-Yves Franceschi, Sylvain Lamprier, and Patrick Gallinari.*

1. **Disentangling physical dynamics from unknown factors for unsupervised video prediction.** CVPR, 2020. [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Le_Guen_Disentangling_Physical_Dynamics_From_Unknown_Factors_for_Unsupervised_Video_Prediction_CVPR_2020_paper.pdf)

   *Vincent Le Guen and Nicolas Thome.*

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

1. **DPM: A deep learning PDE augmentation method with application to large-eddy simulation.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120305854)

   *Justin Sirignano, Jonathan F.MacArt, and Jonathan B.Freund.*

1. **General covariance data augmentation for neural PDE solvers.** ICML, 2023. [paper](https://openreview.net/forum?id=glID3Vsmc0)

   *Vladimir Fanaskov, Tianchi Yu, Alexander Rudikov, and Ivan Oseledets.* 

1. **Learning preconditioners for conjugate gradient PDE solvers.** ICML, 2023. [paper](https://arxiv.org/abs/2305.16432)

   *Yichen Li, Peter Yichen Chen, Tao Du, and Wojciech Matusik.* 

1. **Autoregressive Renaissance in neural PDE solvers.** ICLR, 2023. [paper](https://arxiv.org/abs/2310.19763)

   *Yolanne Yi Ran Lee.*

1. **Stability of implicit neural networks for long-term forecasting in dynamical systems.** ICLR, 2023. [paper](https://arxiv.org/abs/2305.17155)

   *Leon Migus, Julien Salomon, and Patrick Gallinari.* 

1. **Training deep surrogate models with large scale online learning.** ICML, 2023. [paper](https://openreview.net/forum?id=WT70GgYdLI)

   *Lucas Meyer, Marc Schouler, Robert A. Caulk, Alejandro Ribes, and Bruno Raffin.* 

1. **Self-supervised learning with Lie symmetries for partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.05432)

   *Grégoire Mialon, Quentin Garrido, Hannah Lawrence, Danyal Rehman, Yann LeCun, and Bobak T. Kiani.*

1. **Interpretable neural PDE solvers using symbolic frameworks.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.20463)

   *Yolanne Yi Ran Lee.*

1. **Modeling accurate long rollouts with temporal neural PDE solvers.** ICML, 2023. [paper](https://openreview.net/pdf?id=EGTY6V76b3)

   *Phillip Lippe, Bastiaan S. Veeling, Paris Perdikaris, Richard E. Turner, and Johannes Brandstetter.*

1. **Neural-integrated meshfree (NIM) method: A differentiable programming-based hybrid solver for computational mechanics.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.12915)

   *Honghui Du and Qizhi He.*

1. **A deep-genetic algorithm (deep-GA) approach for high-dimensional nonlinear parabolic partial differential equations.** Computers & Mathematics with Applications, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0898122123005126)

   *Endah R.M. Putri, Muhammad L. Shahab, Mohammad Iqbal, Imam Mukhlash, Amirul Hakam, Lutfi Mardianto, and Hadi Susanto.*

1. **Physics-enhanced deep surrogates for partial differential equations.** NMI, 2023. [paper](https://www.nature.com/articles/s42256-023-00761-y)

   *Raphaël Pestourie, Youssef Mroueh, Chris Rackauckas, Payel Das, and Steven G. Johnson .*

1. **Better neural PDE solvers through data-free mesh movers.** ICLR, 2024. [paper](https://openreview.net/forum?id=hj9ZuNimRl)

   *Peiyan Hu, Yue Wang, and Zhiming Ma.*

1. **Generating synthetic data for neural operators.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.02398)

   *Erisa Hasani and Rachel A. Ward.*

1. **A deep branching solver for fully nonlinear partial differential equations.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123008070)

   *Jiang Yu Nguwi, Guillaume Penent, and Nicolas Privault.*

1. **Accelerating data generation for neural operators via Krylov subspace recycling.** ICLR, 2024. [paper](https://openreview.net/forum?id=UpgRVWexaD)

   *Hong Wang, Zhongkai Hao, Jie Wang, Zijie Geng, Zhen Wang, Bin Li, and Feng Wu.*

1. **Space and time continuous physics simulation from partial observations.** ICLR, 2024. [paper](https://openreview.net/forum?id=4yaFQ7181M)

   *Janny Steeven, Nadri Madiha, Digne Julie, and Wolf Christian.*

1. **Speeding up and reducing memory usage for scientific machine learning via mixed precision.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.16645)

   *Joel Hayford, Jacob Goldman-Wetzler, Eric Wang, and Lu Lu.*

1. **Neural operators meet conjugate gradients: The FCG-NO method for efficient PDE solving.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.05598)

   *Alexander Rudikov, Vladimir Fanaskov, Ekaterina Muravleva, Yuri M. Laevsky, and Ivan Oseledets.*

1. **Learning operators with stochastic gradient descent in general Hilbert spaces.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.04691)

   *Lei Shi and Jiaqi Yang.*

1. **Accelerating PDE data generation via differential operator action in solution space.** ICML, 2024. [paper](https://openreview.net/forum?id=Fv9GLw0LkO)

   *Huanshuo Dong, Hong Wang, Haoyang Liu, Jian Luo, and Jie Wang.*

1. **Correctness verification of neural networks approximating differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.07621)

   *Petros Ellinas, Rahul Nellikath, Ignasi Ventura, Jochen Stiasny, and Spyros Chatzivasileiadis.*

1. **DOF: Accelerating high-order differential operators with forward propagation.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.09730)

   *Ruichen Li, Chuwei Wang, Haotian Ye, Di He, and Liwei Wang.*

1. **Sobolev training for operator learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.09084)

   *Namkyeong Cho, Junseung Ryu, and Hyung Ju Hwang.*

1. **Scaling physics-informed hard constraints with mixture-of-experts.** ICLR, 2024. [paper](https://openreview.net/forum?id=u3dX2CEIZb)

   *Nithin Chalapathi, Yiheng Du, and Aditi Krishnapriyan.*

1. **Learning semilinear neural operators: A unified recursive framework for prediction and data assimilation.** ICLR, 2024. [paper](https://openreview.net/forum?id=ZMv6zKYYUs&noteId=EhSvltJICs)

   *Ashutosh Singh, Ricardo Augusto Borsoi, Deniz Erdogmus, and Tales Imbiriba.*

1. **Efficient and stable SAV-based methods for gradient flows arising from deep learning.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999124001608)

   *Ziqi Ma, Zhiping Mao, and Jie Shen.*

1. **Generative downscaling of PDE solvers with physics-guided diffusion models.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.05009v1)

   *Yulong Lu and Wuzhe Xu.*

1. **Nearest neighbors GParareal: Improving scalability of Gaussian processes for parallel-in-Time solvers.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.12182)

   *Guglielmo Gattiglio, Lyudmila Grigoryeva, and Massimiliano Tamborrino.*

1. **Large scale scattering using fast solvers based on neural operators.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.12380)

   *Zongren Zou, Adar Kahana, Enrui Zhang, Eli Turkel, Rishikesh Ranade, Jay Pathak, and George Em Karniadakis.*

1. **Position: Optimization in SciML should employ the function space geometry.** ICML, 2024. [paper](https://openreview.net/forum?id=MOrvoYrlOg)

   *Johannes Müller and Marius Zeinhofer.*

1. **Scaling physics-informed hard constraints with mixture-of-experts.** ICLR, 2024. [paper](https://openreview.net/forum?id=u3dX2CEIZb)

   *Nithin Chalapathi, Yiheng Du, and Aditi S. Krishnapriyan.*

### [AutoML](#content)
1. **Auto-PINN: Understanding and optimizing physics-informed neural architecture.** arXiv, 2022. [paper](https://arxiv.org/abs/2110.13361)

   *Yicheng Wang, Xiaotian Han, Chiayuan Chang, Daochen Zha, Ulisses Braga-Neto, and Xia Hu.*

1. **Building high accuracy emulators for scientific simulations with deep neural architecture search.** Machine Learning: Science and Technology, 2022. [paper](https://iopscience.iop.org/article/10.1088/2632-2153/ac3ffa)

   *M F Kasim, D Watson-Parris, L Deaconu, S Oliver, P Hatfield, D H Froula, G Gregori, M Jarvis, S Khatiwala, J Korenaga, J Topp-Mugglestone, E Viezzer, and S M Vinko.*

1. **Learning operations for neural PDE solvers.** ICLR, 2019. [paper](https://simdl.github.io/files/55.pdf)

   *Nicholas Roberts, Mikhail Khodak, Tri Dao, Liam Li, Christopher Re, and Ameet Talwalkar.*

1. **AutoPINN: When AutoML meets physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.04058)

   *Xinle Wu, Dalin Zhang, Miao Zhang, Chenjuan Guo, Shuai Zhao, Yi Zhang, Huai Wang, and Bin Yang.*

1. **NAS-PINN: Neural architecture search-guided physics-informed neural network for solving PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.10127)

   *Yifan Wang and Linlin Zhong.*

### [Neural Implicit Flow](#content)
1. **Neural implicit flow: A mesh-agnostic dimensionality reduction paradigm of spatio-temporal data.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.03216) 

   *Shaowu Pan, Steven L. Brunton, and J. Nathan Kutz.*

1. **CROM: Continuous reduced-order modeling of PDEs using implicit neural representations.** ICLR, 2023. [paper](https://openreview.net/forum?id=FUORz1tG8Og) 

   *Peter Yichen Chen, Jinxu Xiang, Dong Heon Cho, Yue Chang, G A Pershing, Henrique Teles Maia, Maurizio Chiaramonte, Kevin Carlberg, and Eitan Grinspun.*

1. **MAgNet: Mesh agnostic neural PDE solver.** NIPS, 2022. [paper](https://openreview.net/pdf?id=tbIJmAdqYc8) 

   *Oussama Boussif, Dan Assouline, Loubna Benabbou, and Yoshua Bengio.*

1. **NTopo: Mesh-free topology optimization using implicit neural representations.** NIPS, 2021. [paper](http://crl.ethz.ch/papers/NTopoNeurIPS2021.pdf) 

   *Jonas Zehnder, Yue Li, Stelian Coros, and Bernhard Thomaszewski.*

1. **ContactNets: Learning discontinuous contact dynamics with smooth, implicit representations.** ICLR, 2020. [paper](https://proceedings.mlr.press/v155/pfrommer21a.html) 

   *Samuel Pfrommer, Mathew Halm, and Michael Posa.*

1. **Continuous PDE dynamics forecasting with implicit neural representations.** ICLR, 2023. [paper](https://openreview.net/forum?id=B73niNjbPs) 

   *Yuan Yin, Matthieu Kirchmeyer, Jean-Yves Franceschi, Alain Rakotomamonjy, and Patrick Gallinari.*

1. **Stability of implicit neural networks for long-term forecasting in dynamical systems.** ICLR, 2023. [paper](https://arxiv.org/abs/2305.17155v2)

   *Leon Migus, Julien Salomon, and Patrick Gallinari.*

1. **Operator learning with neural fields: Tackling PDEs on general geometries.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.07266) 

   *Louis Serrano, Lise Le Boudec, Armand Kassaï Koupaï, Thomas X Wang, Yuan Yin, Jean-Noël Vittaut, and Patrick Gallinari.*

1. **Accelerated solutions of convection-dominated partial differential equations using implicit feature tracking and empirical quadrature.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.15661) 

   *Marzieh Alireza Mirhoseini and Matthew J. Zahr.*

1. **Implicit neural spatial representations for time-dependent PDEs.** ICML, 2023. [paper](https://openreview.net/forum?id=7BO6rpA6qQ) 

   *Honglin Chen, Rundi Wu, Eitan Grinspun, Changxi Zheng, and Peter Yichen Chen.*

1. **Reduced-order modeling for parameterized PDEs via implicit neural representations.** NIPS, 2023. [paper](https://arxiv.org/abs/2311.16410) 

   *Tianshu Wen, Kookjin Lee, and Youngsoo Choi.*

1. **Geom-DeepONet: A point-cloud-based deep operator network for field predictions on 3D parameterized geometries.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.14788) 

   *Junyan He, Seid Koric, Diab Abueidda, Ali Najafi, and Iwona Jasiuk.*

1. **Physics-aware neural implicit solvers for multiscale, parametric PDEs with applications in heterogeneous media.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.19019) 

   *Matthaios Chatzopoulos and Phaedon-Stelios Koutsourelakis.*

### [Uncertainty Quantification](#content)
1. **Quantifying total uncertainty in physics-informed neural networks for solving forward and inverse stochastic problems.** arXiv, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119305340)

   *Dongkun Zhang, Lu Lu, Ling Guo, and George Em Karniadakis.*

1. **Adversarial uncertainty quantification in physics-informed neural networks.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303584)

   *Yibo Yang and Paris Perdikaris.*

1. **Conditional Karhunen-Loève expansion for uncertainty quantification and active learning in partial differential equation models.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120303788)

   *Ramakrishna Tipireddy, David A.Barajas-Solano, and Alexandre M.Tartakovsky.*

1. **Physics-constrained deep learning for high-dimensional surrogate modeling and uncertainty quantification without labeled data.** JCP, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119303559)

   *Yinhao Zhu, Nicholas Zabarasa, Phaedon-Stelios Koutsourelakisb, and Paris Perdikaris.*

1. **Error-aware B-PINNs: Improving uncertainty quantification in Bayesian physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.06965)

   *Olga Graf, Pablo Flores, Pavlos Protopapas, and Karim Pichara.*

1. **Physics-informed information field theory for modeling physical systems with uncertainty quantification.** arXiv, 2023. [paper](https://arxiv.org/abs/:2301.07609)

   *Alex Alberts and Ilias Bilionis.*

1. **Quantifying uncertainty for deep learning based forecasting and flow-reconstruction using neural architecture search ensembles.** arXiv, 2023. [paper](https://arxiv.org/abs/:2301.07609)

   *Romit Maulik, Romain Egele, Krishnan Raghavan, and Prasanna Balaprakash.*

1. **Physics-informed variational inference for uncertainty quantification of stochastic differential equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123002784)

   *Hyomin Shin and Minseok Choi.*

1. **Uncertainty quantification in scientific machine learning: Methods, metrics, and comparisons.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122009652)

   *Apostolos F. Psaros, Xuhui Meng, Zongren Zou, Ling Guo, and George Em Karniadakis.*

1. **Auto-weighted Bayesian physics-informed neural networks and robust estimations for multitask inverse problems in pore-scale imaging of dissolution.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.12864)

   *Sarah Perez and Philippe Poncet.*

1. **Neural SPDE solver for uncertainty quantification in high-dimensional space-time dynamics.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.01783)

   *Maxime Beauchamp, Hugo Georgenthum, and Ronan Fablet.*

1. **Ensemble models outperform single model uncertainties and predictions for operator-learning of hypersonic flows.** NIPS, 2023. [paper](https://arxiv.org/abs/2311.00060)

   *Victor J. Leon, Noah Ford, Honest Mrema, Jeffrey Gilbert, and Alexander New.*

1. **Evaluating Uncertainty Quantification approaches for Neural PDEs in scientific applications.** NIPS, 2023. [paper](https://arxiv.org/abs/2311.04457)

   *Vardhan Dongre and Gurpreet Singh Hora.*

1. **Uncertainty quantification for noisy inputs-outputs in physics-informed neural networks and neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.11262)

   *Zongren Zou, Xuhui Meng, and George Em Karniadakis.*

1. **Data-driven autoencoder numerical solver with uncertainty quantification for fast physical simulations.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.01021)

   *Christophe Bonneville, Youngsoo Choi, Debojyoti Ghosh, and Jonathan L. Belof.*

1. **Randomized physics-informed machine learning for uncertainty quantification in high-dimensional inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.06177)

   *Yifei Zong, David Barajas-Solano, and Alexandre M. Tartakovsky.*

1. **Bayesian deep learning framework for uncertainty quantification in stochastic partial differential equations.** SIAM Journal on Scientific Computing, 2024. [paper](https://epubs.siam.org/doi/abs/10.1137/23M1560574)

   *Jeahan Jung, Hyomin Shin, and Minseok Choi.*

1. **Uncertainty quantification for forward and inverse problems of PDEs via latent global evolution.** AAAI, 2024. [paper](https://arxiv.org/abs/2402.08383)

   *Tailin Wu, Willie Neiswanger, Hongtao Zheng, Stefano Ermon, and Jure Leskovec.*

1. **Physics-constrained polynomial chaos expansion for scientific machine learning and uncertainty quantification.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15115)

   *Himanshu Sharma, Lukáš Novák, and Michael D. Shields.*

1. **Physics-constrained polynomial chaos expansion for scientific machine learning and uncertainty quantification.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15115v1)

   *Himanshu Sharma, Lukáš Novák, and Michael D. Shields.*

1. **Conformalized-DeepOnet: A distribution-free framework for uncertainty quantification in deep operator networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15406)

   *Christian Moya, Amirhossein Mollaali, Zecheng Zhang, Lu Lu, and Guang Lin.*

1. **Leveraging viscous Hamilton-Jacobi PDEs for uncertainty quantification in scientific machine learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2404.08809)

   *Zongren Zou, Tingwei Meng, Paula Chen, Jérôme Darbon, and George Em Karniadakis.*

### [Generative Model](#content)
1. **A framework for data-driven solution and parameter estimation of PDEs using conditional generative adversarial networks.** NCS, 2021. [paper](https://www.nature.com/articles/s43588-021-00171-3)

   *Teeratorn Kadeethum, Daniel O’Malley, Jan Niklas Fuhg, Youngsoo Choi, Jonghyun Lee, Hari S. Viswanathan, and Nikolaos Bouklas.*

1. **Neural SDEs as infinite-dimensional GANs.** ICML, 2021. [paper](http://proceedings.mlr.press/v139/kidger21b.html)

   *Patrick Kidger, James Foster, Xuechen Li, and Terry J Lyons.*

1. **PID-GAN: A GAN framework based on a physics-informed discriminator for uncertainty quantification with physics.** KDD, 2021. [paper](https://dl.acm.org/doi/abs/10.1145/3447548.3467449)

   *Arka Daw, M. Maruf, and Anuj Karpatne.*

1. **Generative adversarial neural operators.** Transactions on Machine Learning Research, 2022. [paper](https://openreview.net/forum?id=X1VzbBU6xZ&referrer=%5BTMLR%5D(%2Fgroup%3Fid%3DTMLR))

   *Md Ashiqur Rahman, Manuel A Florez, Anima Anandkumar, Zachary E Ross, and Kamyar Azizzadenesheli.*

1. **Weak adversarial networks for high-dimensional partial differential equations.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120301832)

   *Yaohua Zang, Gang Bao, Xiaojing Ye, and Haomin Zhou.*

1. **Wasserstein generative adversarial uncertainty quantification in physics-informed neural networks.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122003321)

   *Yihang Gao and Michael K. Ng.*

1. **Competitive physics informed networks.** ICLR, 2023. [paper](https://openreview.net/forum?id=z9SIj-IM7tn)

   *Qi Zeng, Yash Kothari, Spencer H Bryngelson, and Florian Tobias Schaefer.*

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

1. **Score-based diffusion models in function space.** arXiv, 2023. [paper](https://arxiv.org/abs/2212.00217)

   *Jae Hyun Lim, Nikola B. Kovachki, Ricardo Baptista, Christopher Beckham, Kamyar Azizzadenesheli, Jean Kossaifi, Vikram Voleti, Jiaming Song, Karsten Kreis, Jan Kautz, Christopher Pal, Arash Vahdat, and Anima Anandkumar.*

1. **Infinite-dimensional diffusion models for function spaces.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.10130)

   *Jakiw Pidstrigach, Youssef Marzouk, Sebastian Reich, and Sven Wang.*

1. **A physics-informed diffusion model for high-fidelity flow field reconstruction.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123000670)

   *Dule Shu, Zijie Li, and Amir Barati Farimani.*

1. **Generative modelling with inverse heat dissipation.** ICLR, 2023. [paper](https://openreview.net/forum?id=4PJUBT9f2Ol)

   *Severi Rissanen, Markus Heinonen, and Arno Solin.*

1. **Differentiable Gaussianization layers for inverse problems regularized by deep generative models.** ICLR, 2023. [paper](https://openreview.net/forum?id=OXP9Ns0gnIq)

   *Dongzhuo Li.*

1. **Transformer meets boundary value inverse problems.** ICLR, 2023. [paper](https://openreview.net/forum?id=HnlCZATopvr)

   *Ruchi Guo, Shuhao Cao, and Long Chen.*

1. **ViTO: Vision Transformer-operator.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.08891)

   *Oded Ovadia, Adar Kahana, Panos Stinis, Eli Turkel, and George Em Karniadakis.*

1. **Latent PINNs: Generative physics-informed neural networks via a latent representation learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.07671)

   *Mohammad H. Taufik and Tariq Alkhalifah.*

1. **Generative diffusion learning for parametric partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.14703)

   *Ting Wang, Petr Plechac, and Jaroslaw Knap.*

1. **Scalable Transformer for PDE surrogate modeling.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.17560)

   *Zijie Li, Dule Shu, and Amir Barati Farimani.*

1. **Latent traversals in generative models as potential flows.** ICML, 2023. [paper](https://openreview.net/forum?id=N9F5wG0hEu)

   *Yue Song, T. Anderson Keller, Nicu Sebe, and Max Welling.*

1. **Learning space-time continuous neural PDEs from partially observed states.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.04110)

   *Valerii Iakovlev, Markus Heinonen, and Harri Lähdesmäki.*

1. **DiTTO: Diffusion-inspired temporal Transformer operator.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.09072)

   *Oded Ovadia, Eli Turkel, Adar Kahana, and George Em Karniadakis.*

1. **PINNsFormer: A Transformer-based framework For physics-informed neural networks.** ICLR, 2024. [paper](https://openreview.net/forum?id=DO2WFXU1Be)

   *Zhiyuan Zhao, Xueying Ding, and B. Aditya Prakash.*

1. **CoCoGen: Physically-consistent and conditioned score-based generative models for forward and inverse problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.10527)

   *Christian Jacobsen, Yilin Zhuang, and Karthik Duraisamy.*

1. **Neuroexplicit diffusion models for inpainting of optical flow fields.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.14599)

   *Tom Fischer, Pascal Peter, Joachim Weickert, and Eddy Ilg.*

### [Transformer](#content)
1. **Learning operators with coupled attention.** JMLR, 2022. [paper](https://www.jmlr.org/papers/v23/21-1521.html) 

   *Matthew Thorpe, Tan Minh Nguyen, Hedi Xia, Thomas Strohmer, Andrea Bertozzi, Stanley Osher, and Bao Wang.* 

1. **Choose a Transformer: Fourier or Galerkin.** NIPS, 2021. [paper](https://openreview.net/forum?id=ssohLcmn4-r)

   *Shuhao Cao.* 

1. **Predicting physics in mesh-reduced space with temporal attention.** ICLR, 2022. [paper](https://openreview.net/forum?id=XctLdNfCmP) 

   *Xu Han, Han Gao, Tobias Pfaff, Jianxun Wang, and Liping Liu.*

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

1. **Nonlinear reconstruction for operator learning of PDEs with discontinuities.** ICLR, 2023. [paper](https://openreview.net/forum?id=CrfhZAsJDsZ) 

   *Samuel Lanthaler, Roberto Molinaro, Patrik Hadorn, and Siddhartha Mishra.*

1. **GNOT: A general neural operator transformer for operator learning.** ICML, 2023. [paper](https://openreview.net/forum?id=JomvpMQ6NF) 

   *Zhongkai Hao, Chengyang Ying, Zhengyi Wang, Hang Su, Yinpeng Dong, Songming Liu, Ze Cheng, Jun Zhu, and Jian Song.*

1. **In-context operator learning for differential equation problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.07993) 

   *Liu Yang, Siting Liu, Tingwei Meng, and Stanley J. Osher.*

1. **Learning neural PDE solvers with parameter-guided channel attention.** ICML, 2023. [paper](https://arxiv.org/abs/2304.14118) 

   *Makoto Takamoto, Francesco Alesiani, and Mathias Niepert.*

1. **Physics informed token Transformer.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.08757) 

   *Cooper Lorsung, Zijie Li, and Amir Barati Farimani.*

1. **Improved operator learning by orthogonal attention.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.12487) 

   *Zipeng Xiao, Zhongkai Hao, Bokai Lin, Zhijie Deng, and Hang Su.*

1. **Multi-scale time-stepping of partial differential equations with Transformers.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.02225) 

   *AmirPouya Hemmasian and Amir Barati Farimani.*

1. **Deciphering and integrating invariants for neural operator learning with various physical mechanisms.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.14361) 

   *Rui Zhang, Qi Meng, and Zhiming Ma.*

1. **Attention-enhanced neural differential equations for physics-informed deep learning of ion transport.** NIPS, 2023. [paper](https://arxiv.org/abs/2312.02871) 

   *Danyal Rehman and John H. Lienhard.*

1. **Inducing point operator Transformer: A flexible and scalable architecture for solving PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.10975) 

   *Seungjun Lee and Taeil Oh.*

1. **Loss-attentional physics-informed neural networks.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S00219991240003055) 

   *Yanjie Song, He Wang, He Yang, Maria Luisa Taccari, and Xiaohui Chen.*

1. **PirateNets: Physics-informed deep learning with residual adaptive networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.00326v2) 

   *Sifan Wang, Bowen Li, Yuhan Chen, and Paris Perdikaris.*

1. **DPOT: Auto-regressive denoising operator transformer for large-scale PDE pre-training.** ICML, 2024. [paper](https://openreview.net/forum?id=X7UnDevHOM) 

   *Zhongkai Hao, Chang Su, Songming Liu, Julius Berner, Chengyang Ying, Hang Su, Anima Anandkumar, Jian Song, and Jun Zhu.*

1. **Positional knowledge is all you need: Position-induced Transformer (PiT) for operator learning.** ICML, 2024. [paper](https://arxiv.org/abs/2405.09285) 

   *Junfeng Chen and Kailiang Wu.*

1. **Hierarchical neural operator Transformer with learnable frequency-aware loss prior for arbitrary-scale super-resolution.** ICML, 2024. [paper](https://arxiv.org/abs/2405.12202) 

   *Xihaier Luo, Xiaoning Qian, and Byung-Jun Yoon.*

1. **Bridging operator learning and conditioned neural fields: A unifying perspective.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.13998) 

   *Sifan Wang, Jacob H Seidman, Shyam Sankaran, Hanwen Wang, George J. Pappas, and Paris Perdikaris.*

1. **Unisolver: PDE-conditional transformers are universal PDE solvers.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.17527) 

   *Zhou Hang, Yuezhou Ma, Haixu Wu, Haowen Wang, and Mingsheng Long.*

1. **Transformers as neural operators for solutions of differential equations with finite regularity.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.19166) 

   *Benjamin Shih, Ahmad Peyvan, Zhongqiang Zhang, and George Em Karniadakis.*

1. **Bridging operator learning and conditioned neural fields: A unifying perspective.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.13998) 

   *Sifan Wang, Jacob H Seidman, Shyam Sankaran, Hanwen Wang, George J. Pappas, and Paris Perdikaris.*

1. **Transolver: A fast Transformer solver for PDEs on general geometries.** ICML, 2024. [paper](https://openreview.net/forum?id=Ywl6pODXjB) 

   *Haixu Wu, Huakun Luo, Haowen Wang, Jianmin Wang, and Mingsheng Long.*

### [Theory](#content)
1. **Convergence analysis of a quasi-Monte Carlo-based deep learning algorithm for solving partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.16196)

   *Fengjiang Fu and Xiaoqun Wang.*

1. **Solving PDEs by variational physics-informed neural networks: A posteriori error analysis.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.00786)

   *Stefano Berrone, Claudio Canuto, and Moreno Pintore.*

1. **A unified framework for the error analysis of physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.00529)

   *Marius Zeinhofer, Rami Masri, and Kent-André Mardal.*

1. **Neural tangent kernel analysis of PINN for advection-diffusion equation.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.11716)

   *M. H. Saadat, B. Gjorgiev, L. Das, and G. Sansavini.* 

1. **Error estimates for DeepONets: A deep learning framework in infinite dimensions.** Transactions of Mathematics and Its Applications, 2022. [paper](https://academic.oup.com/imatrm/article/6/1/tnac001/6542709)

   *Samuel Lanthaler, Siddhartha Mishra, and George Em Karniadakis.*

1. **Hutchinson trace estimation for high-dimensional and high-order physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.14499)

   *Zheyuan Hu, Zekun Shi, George Em Karniadakis, and Kenji Kawaguchi.*

1. **An analysis of universal differential equations for data-driven discovery of ordinary differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.10335)

   *Mattia Silvestri, Federico Baldo, Eleonora Misino, and Michele Lombardi.*

1. **Exponential convergence of deep operator networks for elliptic partial differential equations.** SIAM Journal on Numerical Analysis, 2023. [paper](https://epubs.siam.org/doi/abs/10.1137/21M1465718)

   *Carlo Marcati and Christoph Schwab.*

1. **A discretization-invariant extension and analysis of some deep operator networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.09738)

   *Zecheng Zhang, Wing Tat Leung, and Hayden Schaeffer.*

1. **Machine learning for elliptic PDEs: Fast rate generalization bound, neural scaling law and minimax optimality.** ICLR, 2022. [paper](https://openreview.net/forum?id=mhYUBYNoGz)

   *Yiping Lu, Haoxuan Chen, Jianfeng Lu, Lexing Ying, and Jose Blanchet.* 

1. **Elliptic PDE learning is provably data-efficient.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.12888)

   *Nicolas Boullé, Diana Halikias, and Alex Townsend.*

1. **Error estimates of residual minimization using neural networks for linear PDEs.** Journal of Machine Learning for Modeling and Computing, 2023. [paper](https://arxiv.org/abs/2010.08019)

   *Yeonjong Shin, Zhongqiang Zhang, and George Em Karniadakis.*

1. **Analysis of the generalization error of deep learning based on randomized quasi-Monte Carlo for solving linear Kolmogorov PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.18100)

   *Jichang Xiao, Fengjiang Fu, and Xiaoqun Wang.*

1. **Rigorous a posteriori error bounds for PDE-defined PINNs.** TNNLS, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10337737)

   *Birgit Hillebrecht and Benjamin Unger.*

1. **Error estimation for physics-informed neural networks with implicit Runge-Kutta methods.** arXiv, 2023. [paper](https://arxiv.org/abs/2401.05211)

   *Jochen Stiasny and Spyros Chatzivasileiadis.*

1. **Approximation of solution operators for high-dimensional PDEs.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.10385)

   *Nathan Gaby and Xiaojing Ye.*

1. **Accuracy analysis of physics-informed neural networks for approximating the critical SQG equation.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.10879)

   *Elie Abdo, Ruimeng Hu, and Quyuan Lin.*

1. **Deep Ritz method for elliptical multiple eigenvalue problems.** Journal of Scientific Computing, 2024. [paper](https://link.springer.com/article/10.1007/s10915-023-02443-8)

   *Xia Ji, Yuling Jiao, Xiliang Lu, Pengcheng Song, and Fengru Wang.*

1. **Inf-Sup neural networks for high-dimensional elliptic PDE problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.17233)

   *Xiaokai Huo and Hailiang Liu.*

1. **The challenges of the nonlinear regime for physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.03864)

   *Andrea Bonfanti, Giuseppe Bruno, and Cristina Cipriani.*

1. **A hybrid iterative method based on MIONet for PDEs: Theory and numerical examples.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.03864)

   *Jun Hu and Pengzhan Jin.*

1. **A priori error estimation of physics-informed neural networks solving Allen--Cahn and Cahn--Hilliard equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.02667)

   *Guangtao Zhang, Jiani Lin, Qijia Zhai, Huiyu Yang, Xujun Chen, Xiaoning Zheng, and Ieng Tak Leong.*

1. **Convergence of the deep Galerkin method for mean field control problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.13346)

   *William Hofgard, Jingruo Sun, and Asaf Cohen.*

1. **Data complexity estimates for operator learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.15992)

   *Nikola B. Kovachki, Samuel Lanthaler, and Hrushikesh Mhaskar.*

1. **Bengining overfitting in fixed dimension via physics-informed learning with smooth iductive bias.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.18794)

   *Honam Wong, Wendao Wu, Fanghui Liu, and Yiping Lu.*

1. **Operator learning of Lipschitz operators: An information-theoretic perspective.** arXiv, 2024. [paper](https://arxiv.org/abs/2406.09194)

   *Samuel Lanthaler.*

1. **Guaranteed approximation bounds for mixed-precision neural operators.** ICLR, 2024. [paper](https://openreview.net/forum?id=QJGj07PD9C)

   *Renbo Tu, Colin White, Jean Kossaifi, Boris Bonev, Gennady Pekhimenko, Kamyar Azizzadenesheli, and Anima Anandkumar*

### [Gaussian Process](#content)
1. **PAGP: A physics-assisted Gaussian process framework with active learning for forward and inverse problems of partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.02583)

   *Jiahao Zhang, Shiqi Zhang, and Guang Lin.*

1. **Solving and learning nonlinear PDEs with Gaussian processes.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999121005635)

   *Yifan Chen, Bamdad Hosseini, Houman Owhadi, and Andrew M.Stuart.*

1. **Neural-net-induced Gaussian process regression for function approximation and PDE solution.** JCP, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119301032)

   *Guofei Pang, Liu Yang, and George Em Karniadakis.*

1. **Learning neural optimal interpolation models and solvers.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.07209)

   *Maxime Beauchamp, Joseph Thompson, Hugo Georgenthum, Quentin Febvre, and Ronan Fablet.*

1. **Inference of nonlinear partial differential equations via constrained Gaussian processes.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.11880)

   *Zhaohui Li, Shihao Yang, and Jeff Wu.*

1. **Gaussian process priors for systems of linear partial differential equations with constant coefficients.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.14319)

   *Marc Härkönen, Markus Lange-Hegermann, and Bogdan Raiţă.*

1. **Sparse Cholesky factorization for solving nonlinear PDEs via Gaussian processes.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.01294)

   *Yifan Chen, Houman Owhadi, and Florian Schäfer.*

1. **A mini-batch method for solving nonlinear PDEs with Gaussian processes.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.00307)

   *Xianjin Yang and Houman Owhadi.*

1. **Random grid neural processes for parametric partial differential equations.** ICML, 2023. [paper](https://openreview.net/forum?id=g6WlWFFZxa)

   *Arnaud Vadeboncoeur, Ieva Kazlauskaite, Yanni Papandreou, Fehmi Cirak, Mark Girolami, and Omer Deniz Akyildiz.*

1. **Gaussian process priors for systems of linear partial differential equations with constant coefficients.** ICML, 2023. [paper](https://openreview.net/forum?id=5ivhVPY8RC)

   *Marc Harkonen, Markus Lange-Hegermann, and Bogdan Raita.*

1. **GPLaSDI: Gaussian process-based interpretable latent space dynamics identification through deep autoencoder.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.05882)

   *Christophe Bonneville, Youngsoo Choi, Debojyoti Ghosh, and Jonathan L.Belof.*

1. **Solving high frequency and multi-scale PDEs with Gaussian processes.** ICLR, 2024. [paper](https://openreview.net/forum?id=q4AEBLHuA6)

   *Shikai Fang, Madison Cooley, Da Long, Shibo Li, Robert Kirby, and Shandian Zhe.*

1. **Physics-constrained convolutional neural networks for inverse problems in spatiotemporal partial differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.10306)

   *Daniel Kelshaw and Luca Magri.*

### [Variation](#content) 
1. **PI-VAE: Physics-informed variational auto-encoder for stochastic differential equations.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522006193)

   *Weiheng Zhong and Hadi Meidani.*

1. **Robust SDE-based variational formulations for solving linear PDEs via deep learning.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/richter22a.html)

   *Lorenz Richter and Julius Berner.*

1. **HP-VPINNs: Variational physics-informed neural networks with domain decomposition.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0045782520307325)

   *Ehsan Kharazmi, Zhongqiang Zhang, and George Em Karniadakis.*

1. **Variational onsager neural networks (VONNs): A thermodynamics-based variational learning strategy for non-equilibrium PDEs.** Journal of the Mechanics and Physics of Solids, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0022509622000692)

   *Shenglin Huang, Zequn He, Bryan Chem, and Celia Reina.*

1. **Variational Monte Carlo approach to partial differential equations with neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01927)

   *Moritz Reh and Martin Gärttner.*

1. **Energetic variational neural network discretizations to gradient flows.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.07303)

   *Ziqing Hu, Chun Liu, Yiwei Wang, and Zhiliang Xu.*

1. **Variational Bayes deep operator network: A data-driven Bayesian solver for parametric differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.05655)

   *Shailesh Garg and Souvik Chakraborty.*

1. **Variational inference in neural functional prior using normalizing flows: Application to differential equation and operator learning problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.10448)

   *Xuhui Meng.*

1. **Neural network approximations of PDEs beyond linearity: A representational perspective.** ICML, 2023. [paper](https://openreview.net/forum?id=nEsNOPLpgb)

   *Tanya Marwah, Zachary Chase Lipton, Jianfeng Lu, and Andrej Risteski.*

### [Bayesian](#content)
1. **Bayesian deep learning for partial differential equation parameter discovery with sparse and noisy data.** JCP: X, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S2590055222000117?via%3Dihub)

   *Christophe Bonneville and Christopher Earls.*

1. **B-PINNs: Bayesian physics-informed neural networks for forward and inverse PDE problems with noisy data.** JCP, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S0021999120306872)

   *Liu Yang, Xuhui Meng, and George Em Karniadakis.*

1. **Approximate Bayesian neural operators: Uncertainty quantification for parametric PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.01565)

   *Emilia Magnani, Nicholas Krämer, Runa Eschenhagen, Lorenzo Rosasco, and Philipp Hennig.*

1. **Bayesian autoencoders for data-driven discovery of coordinates, governing equations and fundamental constants.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.10575)

   *L. Mars Gao and J. Nathan Kutz.*

1. **Bayesian physics informed neural networks for data assimilation and spatio-temporal modelling of wildfires.** arXiv, 2022. [paper](https://arxiv.org/abs/2212.00970)

   *Joel Janek Dabrowski, Daniel Edward Pagendam, James Hilton, Conrad Sanderson, Daniel MacKinlay, Carolyn Huston, Andrew Bolt, and Petra Kuhnert.*

1. **Bayesian deep operator learning for homogenized to fine-scale maps for multiscale PDE.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.14188)

   *Zecheng Zhang, Christian Moya, Wing Tat Leung, Guang Lin, and Hayden Schaeffer.*

1. **Bayesian deep learning framework for uncertainty quantification in stochastic partial differential equations.** SIAM Journal on Scientific Computing, 2024. [paper](https://epubs.siam.org/doi/abs/10.1137/23M1560574)

   *Jeahan Jung, Hyomin Shin, and Minseok Choi .*

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

1. **Deep latent regularity network for modeling stochastic partial differential equations.** AAAI, 2023. [paper](https://discovery.ucl.ac.uk/id/eprint/10163280/1/Learning_SPDEs_via_Regularity_Structure.pdf)

   *Shiqi Gong, Peiyan Hu, Qi Meng, Yue Wang, Rongchan Zhu, Bingguang Chen, Zhiming Ma, Hao Ni, and Tieyan Liu.*

1. **Learning in latent spaces improves the predictive accuracy of deep neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2304.07599)

   *Katiana Kontolati, Somdatta Goswami, George Em Karniadakis, and Michael D. Shields.*

1. **Solving high-dimensional PDEs with latent spectral models.** ICML, 2023. [paper](https://openreview.net/forum?id=GwBsk5F1ti)

   *Haixu Wu, Tengge Hu, Huakun Luo, Jianmin Wang, and Mingsheng Long.*

1. **Physics-informed generator-encoder adversarial networks with latent space matching for stochastic differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.01708)

   *Ruisong Gao, Min Yang, and Jin Zhang.*

1. **Smooth and sparse latent dynamics in operator learning with Jerk regularization** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15636)

    *Xiaoyu Xie, Saviz Mowlavi, and Mouhacine Benosman.*

1. **Latent neural PDE solver: A reduced-order modelling framework for partial differential equations** arXiv, 2024. [paper](https://arxiv.org/abs/2402.17853)

    *Zijie Li, Saurabh Patil, Francis Ogoke, Dule Shu, Wilson Zhen, Michael Schneier, John R. Buchanan Jr., and Amir Barati Farimani.*

### [Lagrangian](#content)
1. **Lagrangian PINNs: A causality–conforming solution to failure modes of physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.02902)

   *Rambod Mojgani, Maciej Balajewicz, and Pedram Hassanzadeh.*

1. **AL-PINNs: Augmented Lagrangian relaxation method for physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2205.01059)

   *Hwijae Son, Sung Woong Cho, and Hyung Ju Hwang.*

1. **Lagrangian flow networks for conservation laws.** ICLR, 2024. [paper](https://openreview.net/forum?id=Nshk5YpdWE)

   *Fabricio Arend Torres, Marcello Massimo Negri, Marco Inversi, and Jonathan Aellen.*

1. **An adaptive augmented Lagrangian method for training physics and equality constrained artificial neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.04904)

   *Shamsulhaq Basir and Inanc Senocak.*

1. **Constrained optimization via exact augmented Lagrangian and randomized iterative sketching.** ICML, 2023. [paper](https://openreview.net/forum?id=oxS8hNmCuW)

   *Ilgee Hong, Sen Na, Michael W. Mahoney, and Mladen Kolar.*

1. **An adaptive augmented Lagrangian method for training physics and equality constrained artificial neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.04904)

   *Shamsulhaq Basir and Inanc Senocak.*

1. **Partitioned neural network approximation for partial differential equations enhanced with Lagrange multipliers and localized loss functions.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.14370)

   *Deok-Kyu Jang, Kyungsoo Kim, and Hyea Hyun Kim.*

### [Multi Scale](#content)
1. **Hierarchical deep learning of multiscale differential equation time-steppers.** Philosophical Transactions of the Royal Society A, 2022. [paper](https://royalsocietypublishing.org/doi/10.1098/rsta.2021.0200)

   *Yuying Liu, J. Nathan Kutz, and Steven L. Brunton.*

1. **NH-PINN: Neural homogenization-based physics-informed neural network for multiscale problems.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122006015)

   *Wing Tat Leung, Guang Lin, and Zecheng Zhang.*

1. **Deep multiscale model learning.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307764)

   *Yating Wang, Siu Wun Cheung, Eric T.Chung, Yalchin Efendiev, and Min Wang.*

1. **Multi-scale deep neural networks for solving high dimensional PDEs.** arXiv, 2019. [paper](https://www.science.org/doi/10.1126/sciadv.1602614)

   *Samuel H. Rudy, Steven L. Brunton, Joshua L. Proctor, and J. Nathan Kutz.*

1. **Towards multi-spatiotemporal-scale generalized PDE modeling.** arXiv, 2022. [paper](https://arxiv.org/abs/2209.15616)

   *Jayesh K. Gupta and Johannes Brandstetter.*

1. **MultiAdam: Parameter-wise scale-invariant optimizer for multiscale training of physics-informed neural networks.** ICML, 2023. [paper](https://openreview.net/forum?id=mernbGTe24)

   *Jiachen Yao, Chang Su, Zhongkai Hao, Songming Liu, Hang Su, and Jun Zhu.*

1. **Learning homogenization for elliptic operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.12006)

   *Kaushik Bhattacharya, Nikola Kovachki, Aakila Rajan, Andrew M. Stuart, and Margaret Trautner.*

1. **Multi-grade deep learning for partial differential equations with applications to the Burgers equation.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.07401)

   *Yuesheng Xu and Taishan Zeng.*

1. **Multiscale neural operators for solving time-independent PDEs.** NIPS, 2023. [paper](https://nips.cc/virtual/2023/75473)

   *Winfried Ripken, Lisa Coiffard, Felix Pieper, and Sebastian Dziadzio.*

1. **Multilevel scalable solvers for stochastic linear and nonlinear problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.14649)

   *Sudhi Sharma, Pierre Jolivet, Victorita Dolean, and Abhijit Sarkar.*

1. **Local convolution enhanced global Fourier neural operator for multiscale dynamic spaces prediction.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.12902)

   *Xuanle Zhao, Yue Sun, Tielin Zhang, and Bo Xu.*

1. **Mitigating spectral bias for the multiscale operator learning.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999124001931)

   *Xinliang Liu, Bo Xu, Shuhao Cao, and Lei Zhang.*

1. **SineNet: Learning temporal dynamics in time-dependent partial differential equations.** ICLR, 2024. [paper](https://openreview.net/forum?id=LSYhE2hLWG)

   *Xuan Zhang, Jacob Helwig, Yuchao Lin, Yaochen Xie, Cong Fu, Stephan Wojtowytsch, and Shuiwang Ji.*

1. **Multiscale attention wavelet neural operator for capturing steep trajectories in biochemical systems.** AAAI, 2024. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/29432)

   *Jiayang Su, Junbo Ma, Songyang Tong, Enze Xu, and Minghan Chen.*

1. **A practical PINN framework for multi-scale problems with multi-magnitude loss terms.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999124003619)

   *Yong Wang, Yanzhong Yao, Jiawei Guo, and Zhiming Gao.*

1. **Enhancing multiscale simulations with constitutive relations-aware deep operator networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.13759)

   *Hamidreza Eivazi, Mahyar Alikhani, Jendrik-Alexander Tröger, Stefan Wittek, Stefan Hartmann, and Andreas Rausch.*

1. **UGrid: An efficient-and-rigorous neural multigrid solver for linear PDEs.** ICML, 2024. [paper](https://openreview.net/forum?id=vFATIZXlCm)

   *Xi Han, Fei Hou, and Hong Qin.*

### [Multi Fidelity](#content)
1. **Multifidelity deep operator networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.09157)

   *Amanda A. Howard, Mauro Perego, George Em Karniadakis, and Panos Stinis.*

1. **Physics and equality constrained artificial neural networks: Application to forward and inverse problems with multi-fidelity data fusion.** JCP, 2022. [paper](https://dl.acm.org/doi/abs/10.1016/j.jcp.2022.111301)

   *Lulu Zhang, Tao Luo, Yaoyu Zhang, Weinan E, Zhiqin John Xu, and Zheng Ma.*

1. **A composite neural network that learns from multi-fidelity data: Application to function approximation and inverse PDE problems.** JCP, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0021999119307260)

   *Xuhui Meng and George Em Karniadakis.*

1. **Multifidelity deep neural operators for efficient learning of partial differential equations with application to fast inverse design of nanoscale heat transport.** Physical Review Research, 2022. [paper](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.4.023210)

   *Lu Lu, Raphaël Pestourie, Steven G. Johnson, and Giuseppe Romano.*

1. **Multi-fidelity reduced-order surrogate modeling.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.00325)

   *Paolo Conti, Mengwu Guo, Andrea Manzoni, Attilio Frangi, Steven L. Brunton, and J. Nathan Kutz.*

1. **Multifidelity deep operator networks for data-driven and physics-informed problems.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123005570)

   *Amanda A. Howard, Mauro Perego, George Em Karniadakis, and Panos Stinis.*

1. **A multi-fidelity machine learning based semi-Lagrangian finite volume scheme for linear transport equations and the nonlinear Vlasov-Poisson system.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.04943)

   *Yongsheng Chen, Wei Guo, and Xinghui Zhong.*

1. **Neural operator-based super-fidelity: A warm-start approach for accelerating steady-state simulations.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.11842)

   *Xuhui Zhou, Jiequn Han, Muhammad I. Zafar, Christopher J. Roy, Heng Xiao.*

1. **Multi-resolution partial differential equations preserved learning framework for spatiotemporal dynamics.** AAAI, 2024. [paper](https://www.nature.com/articles/s42005-024-01521-z)

   *Xinyang Liu, Min Zhu, Lu Lu, Hao Sun,  Jianxun Wang.*

### [Multi Grid](#content)
1. **Learning to optimize multigrid PDE solvers.** ICML, 2019. [paper](http://proceedings.mlr.press/v97/greenfeld19a.html)

   *Daniel Greenfeld, Meirav Galun, Ronen Basri, Irad Yavneh, and Ron Kimmel.*

1. **Reducing operator complexity in algebraic multigrid with machine learning approaches.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.07695)

   *Ru Huang, Kai Chang, Huan He, Ruipeng Li, and Yuanzhe Xi.*

1. **Multi-grid tensorized Fourier neural operator for high-resolution PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.00120)

   *Jean Kossaifi, Nikola Kovachki, Kamyar Azizzadenesheli, and Anima Anandkumar.*

1. **MgNO: Efficient parameterization of linear operators via multigrid.** ICLR, 2024 [paper](https://openreview.net/forum?id=8OxL034uEr)

   *Juncai He, Xinliang Liu, and Jinchao Xu.*

1. **MGCNN: A learnable multigrid solver for linear PDEs on structured grids.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.11093)

   *Yan Xie, Minrui Lv, and Chensong Zhang.*

1. **Neural physical simulation with multi-resolution hash grid encoding.** AAAI, 2024. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/28349)

   *Haoxiang Wang, Tao Yu, Tianwei Yang, Hui Qiao, and Qionghai Dai.*

1. **Multigrid-augmented deep learning preconditioners for the helmholtz equation using compact implicit layers.** Journal on Scientific Computing, 2024. [paper](https://epubs.siam.org/doi/abs/10.1137/23M1583302)

   *Bar Lerer, Ido Ben-Yair, and Eran Treister.*

### [Active Learning](#content)
1. **Neural Galerkin scheme with active learning for high-dimensional evolution equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2203.01360)

   *Joan Bruna, Benjamin Peherstorfer, and Eric Vanden-Eijnden.*

1. **Discovering and forecasting extreme events via active learning in neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2204.02488)

   *Ethan Pickering, Stephen Guth, George Em Karniadakis, and Themistoklis P. Sapsis.*

1. **Active learning based sampling for high-dimensional nonlinear partial differential equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122009111)

   *Wenhan Gao and Chunmei Wang.*

1. **An extreme learning machine-based method for computational PDEs in higher dimensions.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.07049)

   *Yiran Wang and Suchuan Dong.*

1. **Multi-resolution active learning of Fourier neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.16971)

   *Shibo Li, Xin Yu, Wei Xing, Mike Kirby, Akil Narayan, and Shandian Zhe.*

1. **A foundational neural operator that continuously learns without forgetting.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.18885)

   *Tapas Tripura and Souvik Chakraborty.*

1. **Neural Galerkin schemes with active learning for high-dimensional evolution equations.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999123006836)

   *Joan Bruna, Benjamin Peherstorfer, and Eric Vanden-Eijnden.*


## [Applications](#content)
### [Optimization](#content)
1. **Fast PDE-constrained optimization via self-supervised operator learning.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13297)

   *Sifan Wang, Mohamed Aziz Bhouri, and Paris Perdikaris.*

1. **An extended physics informed neural network for preliminary analysis of parametric optimal control problems.** arXiv, 2021. [paper](https://arxiv.org/abs/2110.13530)

   *Nicola Demo, Maria Strazzullo, and Gianluigi Rozza.*

1. **Optimal control of PDEs using physics-informed neural networks.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S002199912200794X)

   *Saviz Mowlavi and Saleh Nabi.*

1. **Solving PDE-constrained control problems using operator learning.** AAAI, 2022. [paper](https://aaai-2022.virtualchair.net/poster_aaai12978)

   *Rakhoon Hwang, Jae Yong Lee, Jin Young Shin, and Hyung Ju Hwang.*

1. **PDE-based optimal strategy for unconstrained online learning.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22d.html)

   *Zhiyu Zhang, Ashok Cutkosky, and Ioannis Paschalidis.*

1. **Control of partial differential equations via physics-informed neural networks.** Journal of Optimization Theory and Applications, 2022. [paper](https://link.springer.com/article/10.1007/s10957-022-02100-4)

   *Carlos J. García-Cervera, Mathieu Kessler, and Francisco Periago.*

1. **A machine learning framework for solving high-dimensional mean field game and mean field control problems.** PNAS, 2020. [paper](https://www.pnas.org/doi/abs/10.1073/pnas.1922204117)

   *Lars Ruthottoa, Stanley J. Osherc, Wuchen Lic, Levon Nurbekyanc, and Samy Wu Fung.*

1. **Bi-level physics-informed neural networks for PDE constrained optimization using Broyden's hypergradients.** ICLR, 2023. [paper](https://openreview.net/forum?id=kkpL4zUXtiw)

   *Zhongkai Hao, Chengyang Ying, Hang Su, Jun Zhu, Jian Song, and Ze Cheng.*

1. **A combination technique for optimal control problems constrained by random PDEs.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.00499)

   *Fabio Nobile and Tommaso Vanzan.*

1. **A multilevel reinforcement learning framework for PDE-based control.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.08400)

   *Atish Dixit and Ahmed H. Elsheikh.*

1. **Optimal learning of high-dimensional classification problems using deep neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2112.12555)

   *Philipp Petersen and Felix Voigtlaender.*

1. **The ADMM-PINNs algorithmic framework for nonsmooth PDE-constrained optimization: A deep learning approach.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.08309)

   *Yongcun Song, Xiaoming Yuan, and Hangrui Yue.*

1. **Learning differentiable solvers for systems with hard constraints.** ICLR, 2023. [paper](https://openreview.net/forum?id=vdv6CmGksr0)

   *Geoffrey Négiar, Geoffrey_Négiar, Michael W. Mahoney, and Aditi Krishnapriyan.*

1. **Volumetric optimal transportation by fast Fourier transform.** ICLR, 2023. [paper](https://openreview.net/forum?id=EVrz7UM-ZDm)

   *Na Lei, DONGSHENG An, Min Zhang, Xiaoyin Xu, and David Gu.*

1. **PDE-based optimal strategy for unconstrained online learning.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22d.html)

   *Zhiyu Zhang, Ashok Cutkosky, and Ioannis Paschalidis.*

1. **PDE-constrained models with neural network terms: Optimization and global convergence.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123001110)

   *Justin Sirignano, Jonathan MacArt, and Konstantinos Spiliopoulos.*

1. **Topology optimization using neural networks with conditioning field initialization for improved efficiency.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.10460)

   *Hongrui Chen, Aditya Joglekar, and Levent Burak Kara.*

1. **Deep reinforcement learning for optimal well control in subsurface systems with uncertain geology.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123000402)

   *Yusuf Nasir and Louis J. Durlofsky.*

1. **Constrained optimization via exact augmented lagrangian and randomized iterative sketching.** ICML, 2023. [paper](https://arxiv.org/abs/2305.18379)

   *Ilgee Hong, Sen Na, Michael W. Mahoney, and Mladen Kolar.*

1. **Efficient PDE-constrained optimization under high-dimensional uncertainty using derivative-informed neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.20053)

   *Dingcheng Luo, Thomas O'Leary-Roseberry, Peng Chen, and Omar Ghattas.*

1. **Dimension-independent certified neural network watermarks via mollifier smoothing.** ICML, 2023. [paper](https://openreview.net/forum?id=lO5sAPGWqv)

   *Jiaxiang Ren, Yang Zhou, Jiayin Jin, Lingjuan Lyu, and Da Yan.*

1. **Accelerated primal-dual methods with enlarged step sizes and operator learning for nonsmooth optimal control problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.00296)

   *Yongcun Song, Xiaoming Yuan, and Hangrui Yue.*

1. **Accelerated primal-dual methods with enlarged step sizes and operator learning for nonsmooth optimal control problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.00296)

   *Yongcun Song, Xiaoming Yuan, and Hangrui Yue.*

1. **Operator learning for continuous spatial-temporal model with a hybrid optimization scheme.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.11798)

   *Chuanqi Chen and Jinlong Wu.*

1. **Deep neural operators as accurate surrogates for shape optimization.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623017992)

   *Khemraj Shukla, Vivek Oommen, Ahmad Peyvan, Michael Penwarden, Nicholas Plewacki, Luis Bravo, Anindya Ghoshal, Robert M. Kirby, and George Em Karniadakis.*

1. **Accelerating Bayesian optimal experimental design with derivative-informed neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.14810)

   *Jinwoo Go and Peng Chen.*

1. **A supervised learning scheme for computing Hamilton-Jacobi equation via density coupling.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.15954)

   *Jianbo Cui, Shu Liu, and Haomin Zhou.*

1. **Optimization in SciML -- A function space perspective.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.07318)

   *Johannes Müller and Marius Zeinhofer.*

1. **Inverse design method for horn antennas based on knowledge-embedded physics-informed neural networks.** IEEE Antennas and Wireless Propagation Letters, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10433641)

   *Jinpin Liu, Bingzhong Wang, Chuansheng Chen, and Ren Wang.*

1. **G-RepsNet: A fast and general construction of equivariant networks for arbitrary matrix groups.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.15413)

   *Sourya Basu, Suhas Lohit, and Matthew Brandr.*

### [Fluid](#content)
1. **Physics-informed neural networks (PINNs) for fluid mechanics: A review.** Acta Mechanica Sinica, 2021. [paper](https://link.springer.com/article/10.1007/s10409-021-01148-1)

   *Shengze Cai, Zhiping Mao, Zhicheng Wang, Minglang Yin, and George Em Karniadakis.*

1. **Neural operator prediction of linear instability waves in high-speed boundary layers.** JCP, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S0021999122008567)

   *Patricio Clark Di Leoni, Lu Lu, Charles Meneveau, George Karniadakis, and Tamer A. Zaki.*

1. **A physics-informed convolutional neural network for the simulation and prediction of two-phase darcy flows in heterogeneous porous media.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123000141)

   *Zhao Zhang, Xia Yan, Piyang Liu, Kai Zhang, Renmin Han, and Sheng Wang.*

1. **DiscretizationNet: A machine-learning based solver for Navier–Stokes equations using finite volume discretization.** CMAME, 2021. [paper](https://www.sciencedirect.com/science/article/pii/S004578252100058X)

   *Rishikesh Ranade, Chris Hillb, and Jay Pathak.*

1. **Surrogate modeling for fluid flows based on physics-constrained deep learning without simulation data.** CMAME, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S004578251930622X)

   *Luning Sun, Han Gao, Shaowu Pan, and Jianxun Wang.*

1. **Towards physics-informed deep learning for turbulent flow prediction.** KDD, 2020. [paper](https://dl.acm.org/doi/10.1145/3394486.3403198)

   *Rui Wang, Karthik Kashinath, Mustafa Mustafa, Adrian Albert, and Rose Yu.*

1. **Learning to estimate and refine fluid motion with physical dynamics.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/zhang22ad/zhang22ad.pdf)

   *Mingrui Zhang, Jianhong Wang, James Tlhomole, and Matthew D. Piggott.*

1. **Physics informed neural fields for smoke reconstruction with sparse data.** ACM Transactions on Graphics, 2022. [paper](https://dl.acm.org/doi/10.1145/3528223.3530169)

   *Mengyu Chu, Lingjie Liu, Quan Zheng, Erik Franz, Hans-Peter Seidel, Christian Theobalt, and Rhaleb Zayer.*

1. **Physics-informed deep learning for traffic state estimation: A hybrid paradigm informed by second-order traffic models.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16132)

   *Rongye Shi, Zhaobin Mo, and Xuan Di.*

1. **Residual-based adaptivity for two-phase flow simulation in porous media using physics-informed neural networks.** CMAME, 2022. [paper](https://www.sciencedirect.com/science/article/pii/S004578252200295X)

   *John M.Hanna, José V.Aguado, Sebastien Comas-Cardona, Ramz Askri, and Domenico Borzacchiello.*

1. **Learned turbulence modelling with differentiable fluid solvers: Physics-based loss-functions and optimisation horizons.** JFM, 2022. [paper](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/learned-turbulence-modelling-with-differentiable-fluid-solvers-physicsbased-loss-functions-and-optimisation-horizons/28D19239CEDB81A3DA58F32E0E8CB3B2)

   *Björn List, Liwei Chen, and Nils Thuerey.*

1. **Learning hydrodynamic equations for active matter from particle simulations and experiments.** PNAS, 2023. [paper](https://www.pnas.org/doi/10.1073/pnas.2206994120)

   *Rohit Supekar, Boya Song, Alasdair Hastewell, Gary P. T. Choi, Alexander Mietke, and Jörn Dunkel.*

1. **Physics informed neural networks: A case study for gas transport problems.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0021999123001365)

   *Erik Laurin Strelow, Alf Gerisch, Jens Lang, and Marc E. Pfetsch.*

1. **Turbulence model augmented physics informed neural networks for mean flow reconstruction.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.01065)

   *Yusuf Patel, Vincent Mons, Olivier Marquet, and Georgios Rigas.*

1. **RANS-PINN based simulation surrogates for predicting turbulent flows.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.06034)

   *Shinjan Ghosh, Amit Chakraborty, Georgia Olympia Brikis, and Biswadip Dey.*

1. **Meta-learning for airflow simulations with graph neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.10624)

   *Wenzhuo Liu, Mouadh Yagoubi, and Marc Schoenauer.*

1. **Learning operators for identifying weak solutions to the Navier-Stokes equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.10685)

   *Dixi Wang and Cheng Yu.*

1. **Physics-informed neural networks modeling for systems with moving immersed boundaries: Application to an unsteady flow past a plunging foil.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.13395)

   *Rahul Sundar, Dipanjan Majumdar, Didier Lucor, and Sunetra Sarkar.*

1. **A machine learning pressure emulator for hydrogen embrittlement.** ICML, 2023. [paper](https://arxiv.org/abs/2306.13116)

   *Minh Triet Chau, João Lucas de Sousa Almeida, Elie Alhajjar, and Alberto Costa Nogueira Junior.*

1. **A probabilistic, data-driven closure model for RANS simulations with aleatoric, model uncertainty.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.02432)

   *Atul Agrawal and Phaedon-Stelios Koutsourelakis.*

1. **Physics-informed machine learning for calibrating macroscopic traffic flow models.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.06267)

   *Yu Tang, Li Jin, and Kaan Ozbay.*

1. **Radial basis function-differential quadrature-based physics-informed neural network for steady incompressible flows.** Physics of Fluids, 2023. [paper](https://pubs.aip.org/aip/pof/article/35/7/073607/2902185)

   *Yang Xiao, Liming Yang, Yinjie Du, Yuxin Song, and Chang Shu.*

1. **Long-term predictions of turbulence by implicit U-Net enhanced Fourier neural operator.** Physics of Fluids, 2023. [paper](https://pubs.aip.org/aip/pof/article/35/7/075145/2903750)

   *Zhijie Li, Wenhui Peng, Zelong Yuan, and Jianchun Wang.*

1. **Physics-informed neural networks for parametric compressible Euler equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.14045)

   *Simon Wassing, Stefan Langer, and Philipp Bekemeyer.*

1. **Simulation of rarefied gas flows using physics-informed neural network combined with discrete velocity method.** Physics of Fluids, 2023. [paper](https://pubs.aip.org/aip/pof/article/35/7/077124/2903882)

   *Linying Zhang, Wenjun Ma, Qin Lou, and Jun Zhang.*

1. **Influence of adversarial training on super-resolution turbulence models.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.16015)

   *Ludovico Nista, Christoph David Karl Schumann, Mathis Bode, Temistocle Grenga, Jonathan F. MacArt, Antonio Attili, and Heinz Pitsch.*

1. **Turbulent flow simulation using autoregressive conditional diffusion models.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.01745)

   *Georg Kohl, Liwei Chen, and Nils Thuerey.*

1. **Physics-informed neural networks for studying heat transfer in porous media.** International Journal of Heat and Mass Transfer, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0017931023008165)

   *Jiaxuan Xu, Han Wei, and Hua Bao.*

1. **Solution multiplicity and effects of data and eddy viscosity on Navier-Stokes solutions inferred by physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.06010)

   *Zhicheng Wang, Xuhui Meng, Xiaomo Jiang, Hui Xiang, and George Em Karniadakis.*

1. **Towards real-time training of physics-informed neural networks: Applications in ultrafast ultrasound blood flow imaging.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.04755)

   *Haotian Guan, Jinping Dong, and Weining Lee.*

1. **Multi-physical predictions in electro-osmotic micromixer by auto-encoder physics-informed neural networks.** Physics of Fluids, 2023. [paper](https://pubs.aip.org/aip/pof/article-abstract/35/10/102007/2914663/Multi-physical-predictions-in-electro-osmotic?redirectedFrom=fulltext)

   *Naiwen Chang, Ying Huai, Tingting Liu, Xi Chen, and Yuqi Jin.*

1. **Studying turbulent flows with physics-informed neural networks and sparse data.** International Journal of Heat and Fluid Flow, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0142727X23001315)

   *S. Hanrahan, M. Kozul, and R.D. Sandberg.*

1. **Enhancing physics informed neural networks for solving Navier–Stokes equations.** International Journal for Numerical Methods in Fluids, 2023. [paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/fld.5250)

   *Ayoub Farkane, Mounir Ghogho, Mustapha Oudani, and Mohamed Boutayeb.*

1. **Physics-informed tensor basis neural network for turbulence closure modeling.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.14576)

   *Leon Riccius, Atul Agrawal, and Phaedon-Stelios Koutsourelakis.*

1. **Investigation of low and high-speed fluid dynamics problems using physics-informed neural network.** International Journal of Computational Fluid Dynamics, 2023. [paper](https://www.tandfonline.com/doi/abs/10.1080/10618562.2023.2285330)

   *Anubhav Joshi,Alexandros Papados, and Rakesh Kumar.*

1. **Singular layer physics informed neural network method for plane parallel flows.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.15304)

   *Tengyuan Chang, Gungmin Gie, Youngjoon Hong, and Chang-Yeol Jung.*

1. **Data-efficient operator learning for solving high Mach number fluid flow problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.16860)

   *Noah Ford, Victor J. Leon, Honest Merman, Jeffrey Gilbert, and Alexander New.*

1. **Three-dimensional laminar flow using physics informed deep neural networks featured.** Physics of Fluids, 2023. [paper](https://pubs.aip.org/aip/pof/article/35/12/121703/2925751)

   *Saykat Kumar Biswas and N. K. Anand.*

1. **Real-time prediction of gas flow dynamics in diesel engines using a deep neural operator framework.** Applied Intelligence, 2023. [paper](https://link.springer.com/article/10.1007/s10489-023-05178-z)

   *Varun Kumar, Somdatta Goswami, Daniel Smith, and George Em Karniadakis.*

1. **Semi-analytic physics informed neural network for convection-dominated boundary layer problems in 2D.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.03295)

   *Gungmin Gie, Youngjoon Hong, Chang-Yeol Jung, and Dongseok Lee.*

1. **The improved backward compatible physics-informed neural networks for reducing error accumulation and applications in data-driven higher-order rogue waves.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.06715)

   *Shuning Lin and Yong Chen.*

1. **Learning characteristic parameters and dynamics of centrifugal pumps under multi-phase flow using physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.03001)

   *Felipe de Castro Teixeira Carvalho, Kamaljyoti Nath, Alberto Luiz Serpa, and George Em Karniadakis.*

1. **On the locality of local neural operator in learning fluid dynamics.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.09820)

   *Ximeng Ye, Hongyu Li, Jingjie Huang, and Guoliang Qin.*

1. **Multi-viscosity physics-informed neural networks for generating ultra high resolution flow field data.** International Journal of Computational Fluid Dynamics, 2023. [paper](https://www.tandfonline.com/doi/abs/10.1080/10618562.2023.2295286)

   *Sen Zhang, Xiaowei Guo, Chao Li, Ran Zhao, Canqun Yang, Wei Wang, and Yanxu Zhong.*

1. **Towards high-accuracy deep learning inference of compressible flows over aerofoils.** Computers & Fluids, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045793022003000)

   *Liwei Chen and Nils Thuerey.*

1. **Data-driven and physics-informed deep learning operators for solution of heat conduction equation with parametric heat source.** International Journal of Heat and Mass Transfer, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0017931022012777)

   *Seid Koric and Diab W. Abueidda.*

1. **Energy-preserving reduced operator inference for efficient design and control.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.02889)

   *Tomoki Koike and Elizabeth Qian.*

1. **Variable linear transformation improved physics-informed neural networks to solve thin-layer flow problems.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S002199912400010X)

   *Jiahao Wu, Yuxin Wu, Guihua Zhang, and Yang Zhang.*

1. **Riemannonets: Interpretable neural operators for Riemann problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.08886)

   *Ahmad Peyvan, Vivek Oommen, Ameya D. Jagtap, and George Em Karniadakis.*

1. **Physics-informed neural networks for incompressible flows with moving boundaries.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/1/013617/3105948)

   *Yongzheng Zhu, Weizhen Kong, Jian Deng, and Xin Bian.*

1. **Solving the one dimensional vertical suspended sediment mixing equation with arbitrary eddy diffusivity profiles using temporal normalized physics-informed neural networks.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/1/017132/3105970)

   *Shaotong Zhang, Jiaxin Deng, Xi'an Li, Zixi Zhao, Jinran Wu, Weide Li,Yougan Wang, and Dongsheng Jeng.*

1. **Neural SPH: Improved neural modeling of Lagrangian fluid dynamics.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.06275)

   *Artur P. Toshev, Jonas A. Erbesdobler, Nikolaus A. Adams, and Johannes Brandstetter.*

1. **Continuous and discontinuous compressible flows in a converging–diverging channel solved by physics-informed neural networks without exogenous data.** Scientific Reports, 2024. [paper](https://www.nature.com/articles/s41598-024-53680-2)

   *Hong Liang, Zilong Song, Chong Zhao, and Xin Bian.*

1. **Gauss-Newton natural gradient descent for physics-informed computational fluid dynamics.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.10680)

   *Anas Jnini, Flavio Vella, and Marius Zeinhofer.*

1. **Residual-enhanced physics-guided machine learning with hard constraints for subsurface flow in reservoir engineering.** TGRS, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10413628)

   *Haibo Cheng, Yunpeng He, Peng Zeng, and Valeriy Vyatkin.*

1. **Discovering artificial viscosity models for discontinuous Galerkin approximation of conservation laws using physics-informed machine learning.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.16517)

   *Matteo Caldana, Paola F. Antonietti, and Luca Dede'.*

1. **EuLagNet: Eulerian fluid prediction with Lagrangian dynamics.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.02425)

   *Qilong Ma, Haixu Wu, Lanxiang Xing, Jianmin Wang, and Mingsheng Long.*

1. **Physics-informed neural networks with domain decomposition for the incompressible Navier–Stokes equations.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/2/021914/3267717)

   *Linyan Gu, Shanlin Qin, Lei Xu, and Rongliang Chen.*

1. **Two-stage initial-value iterative physics-informed neural networks for simulating solitary waves of nonlinear wave equations.** JCP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0021999124001669)

   *Jin Song, Ming Zhong, George Em Karniadakis, and Zhenya Yan.*

1. **Continuous and discontinuous compressible flows in a converging–diverging channel solved by physics-informed neural networks without exogenous data.** Scientific Reports, 2024. [paper](https://www.nature.com/articles/s41598-024-53680-2)

   *Hong Liang, Zilong Song, Chong Zhao, and Xin Bian.*

1. **A fast general thermal simulation model based on multi-branch physics-informed deep operator neural network.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/3/037142/3277890)

   *Zibo Lu, Yuanye Zhou, Yanbo Zhang, Xiaoguang Hu, Qiao Zhao, and Xuyang Hu.*

1. **Potential of physics-informed neural networks for solving fluid flow problems with parametric boundary conditions.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/3/037143/3278488)

   *F. Lorenzen, A. Zargaran, and U. Janoske.*

1. **Physics-informed neural networks for transonic flow around a cylinder with high Reynolds number.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/3/036129/3278829)

   *Xiang Ren, Peng Hu, Hua Su, Feizhou Zhang, and Huahua Yu.*

1. **Physics-informed neural networks enhanced particle tracking velocimetry: An example for turbulent Jet flow.** TIM, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10522764)

   *Shengze Cai, Callum Gray, and George Em Karniadakis.*

1. **SPI-MIONet for surrogate modeling in phase-field hydraulic fracturing.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524003104)

   *Xiaoqiang Wang, Peichao Li, Kaile Jia, Shaoqi Zhang, Chun Li, Bangchen Wu, Yilun Dong, and Detang Lu.*

1. **Strategies for multi-case physics-informed neural networks for tube flows: A study using 2D flow scenarios.** Scientific Reports, 2024. [paper](https://www.nature.com/articles/s41598-024-62117-9)

   *Hong Shen Wong, Wei Xuan Chan, Bing Huan Li, and Choon Hwai Yap.*

1. **Physics-informed neural networks for fully non-linear free surface wave propagation.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article-abstract/36/6/062106/3296519/Physics-informed-neural-networks-for-fully-non?redirectedFrom=fulltext)

   *Haocheng Lu, Qian Wang, Wenhao Tang, and Hua Liu.*

1. **HelmFluid: Learning Helmholtz dynamics for interpretable fluid prediction.** ICML, 2024. [paper](https://openreview.net/forum?id=lHJFfDFbm6)

   *Lanxiang Xing, Haixu Wu, Yuezhou Ma, Jianmin Wang, and Mingsheng Long.*

1. **Strategies for multi-case physics-informed neural networks for tube flows: a study using 2D flow scenarios.** SR, 2024. [paper](https://www.nature.com/articles/s41598-024-62117-9)

   *Hong Shen Wong, Wei Xuan Chan, Bing Huan Li, and Choon Hwai Yap.*

1. **From zero to turbulence: Generative modeling for 3D flow simulation.** ICLR, 2024. [paper](https://openreview.net/forum?id=ZhlwoC1XaN)

   *Marten Lienen, David Lüdke, Jan Hansen-Palmus, and Stephan Günnemann.*

1. **Enhancing the accuracy of physics-informed neural networks for indoor airflow simulation with experimental data and Reynolds-averaged Navier–Stokes turbulence model.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article-abstract/36/6/065161/3299253/Enhancing-the-accuracy-of-physics-informed-neural?redirectedFrom=fulltext)

   *Chi Zhang, Chih-Yung Wen, Yuan Jia, Yu-Hsuan Juan, Yee-Ting Lee, Zhengwei Chen, An-Shik Yang, and Zhengtong Li.*

1. **Physics-informed neural networks for fully non-linear free surface wave propagation.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article-abstract/36/6/062106/3296519/Physics-informed-neural-networks-for-fully-non?redirectedFrom=fulltext)

   *Haocheng Lu, Qian Wang, Wenhao Tang, and Hua Liu.*

1. **Neural network with local converging input for unstructured-grid computational fluid dynamics.** AIAA Journal, 2024. [paper](https://arc.aiaa.org/doi/full/10.2514/1.J063885)

   *Weiming Ding, Haoxiang Huang, Tzu-Jung Lee, Yingjie Liu, and Vigor Yang.*

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

   *Yanwei Jia and Xunyu Zhou.*

1. **Physics-informed kernel embeddings: Integrating prior system knowledge with data-driven control.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.03565)

   *Adam J. Thorpe, Cyrus Neary, Franck Djeumou, Meeko M. K. Oishi, and Ufuk Topcu.*

1. **Distributed control of partial differential equations using convolutional reinforcement learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.10737)

   *Sebastian Peitz, Jan Stenner, Vikas Chidananda, Oliver Wallscheid, Steven L. Brunton, and Kunihiko Taira.*

1. **Neural control of parametric solutions for high-dimensional evolution PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.00045)

   *Nathan Gaby, Xiaojing Ye, and Haomin Zhou.*

1. **Bridging physics-informed neural networks with reinforcement learning: Hamilton-Jacobi-Bellman proximal policy optimization (HJBPPO).** arXiv, 2023. [paper](https://arxiv.org/abs/2302.00237)

   *Amartya Mukherjee and Jun Liu.*

1. **AONN: An adjoint-oriented neural network method for all-at-once solutions of parametric optimal control problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.02076)

   *Pengfei Yin, Guangqiang Xiao, Kejun Tang, and Chao Yang.*

1. **Neural operators for bypassing gain and control computations in PDE backstepping.** arXiv, 2023. [paper](https://arxiv.org/abs/2302.14265)

   *Luke Bhan, Yuanyuan Shi, and Miroslav Krstic.*

1. **Neural operators of backstepping controller and observer gain functions for reaction-diffusion PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.10506)

   *Miroslav Krstic, Luke Bhan, and Yuanyuan Shi.*

1. **Leveraging multi-time Hamilton-Jacobi PDEs for certain scientific machine learning problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.12928)

   *Paula Chen, Tingwei Meng, Zongren Zou, Jérôme Darbon, and George Em Karniadakis.*

1. **Learning to control PDEs with differentiable physics.** ICLR, 2020. [paper](https://openreview.net/forum?id=HyeSin4FPB)

   *Philipp Holl, Nils Thuerey, and Vladlen Koltun.*

1. **A generalizable physics-informed learning framework for risk probability estimation.** L4DC, 2020. [paper](https://arxiv.org/abs/2305.06432)

   *Zhuoyuan Wang and Yorie Nakahira.*

1. **Operator learning for nonlinear adaptive control.** L4DC, 2023. [paper](https://lukebhan.com/l4dc2023.pdf)

   *Luke Bhan, Yuanyuan Shi and Miroslav Krstic.*

1. **Optimal temperature trajectory for tubular reactor using physics informed neural networks.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0959152423000823)

   *Rahul Patel, Sharad Bhartiya, and Ravindra Gudi.*

1. **Physics-informed recurrent neural network modeling for predictive control of nonlinear processes.** Journal of Process Control, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0959152423000847)

   *Yingzhe Zheng, Cheng Hu, Xiaonan Wang, and Zhe Wu.*

1. **Physics-guided neural networks for inversion-based feedforward control applied to hybrid stepper motors.**arXiv, 2023. [paper](https://arxiv.org/abs/2306.12817)

   *Daiwei Fan, Max Bolderman, Sjirk Koekebakker, Hans Butler, and Mircea Lazar.*

1. **Physics-informed recurrent neural network modeling for predictive control of nonlinear processes.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0959152423000847)

   *Yingzhe Zheng, Cheng Hu, Xiaonan Wang, and Zhe Wu.*

1. **Optimal Dirichlet boundary control by Fourier neural operators applied to nonlinear optics.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.07292)

   *Nils Margenberg, Franz X. Kärtner, and Markus Bause.*

1. **Neural operators for delay-compensating control of hyperbolic PIDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2307.11436)

   *Jie Qi, Jing Zhang, and Miroslav Krstic.*

1. **Physics-informed online learning of gray-box models by moving horizon estimation.** European Journal of Control, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0947358023000900)

   *Kristoffer Fink Løwenstein, Daniele Bernardini, Lorenzo Fagiano, and Alberto Bemporad.*

1. **Online identification and control of PDEs via reinforcement learning methods.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.04068v1)

   *Alessandro Alla, Agnese Pacifico, Michele Palladino, and Andrea Pesare.*

1. **The hard-constraint PINNs for interface optimal control problems.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.06709)

   *Ming-Chih Lai, Yongcun Song, Xiaoming Yuan, Hangrui Yue, and Tianyou Zeng.*

1. **Deep learning of delay-compensated backstepping for reaction-diffusion PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.10501)

   *Shanshan Wang, Mamadou Diagne, and Miroslav Krstić.*

1. **Computationally efficient data-driven discovery and linear representation of nonlinear systems for control.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.04074)

   *Madhur Tiwari, George Nehma, and Bethany Lusch.*

1. **Physics-informed state-space neural networks for transport phenomena.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.12211)

   *Akshay J Dave and Richard B. Vilim.*

1. **A comparison of mesh-free differentiable programming and data-driven strategies for optimal control under PDE constraints.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.02286)

   *Roussel Desmond Nzoyem, David A.W. Barton, and Tom Deakin.*

1. **A data-driven tracking control framework using physics-informed neural networks and deep reinforcement learning for dynamical systems.** JCP, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623014409)

   *R.R. Faria, B.D.O. Capron, A.R. Secchi, and M.B. De Souza Jr.*

1. **Leveraging Hamilton-Jacobi PDEs with time-dependent Hamiltonians for continual scientific machine learning.** L4DC, 2023. [paper](https://arxiv.org/abs/2311.07790)

   *Paula Chen, Tingwei Meng, Zongren Zou, Jérôme Darbon, and George Em Karniadakis.*

1. **Physics-informed neural network Lyapunov functions: PDE characterization, learning, and verification.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.09131)

   *Jun Liu, Yiming Meng, Maxwell Fitzsimmons, and Ruikun Zhou.*

1. **Taming waves: A physically-interpretable machine learning framework for realizable control of wave dynamics.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.09460)

   *Tristan Shah, Feruza Amirkulova, and Stas Tiomkin.*

1. **Neural operators for boundary stabilization of stop-and-go traffic.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.10374)

   *Yihuai Zhang, Ruiguo Zhong, and Huan Yu.*

1. **Neural operator approximations of backstepping kernels for 2×2 hyperbolic PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.16762)

   *Shanshan Wang, Mamadou Diagne, and Miroslav Krstić.*

1. **Lyapunov-based physics-informed long short-term memory (LSTM) neural network-based adaptive control.** IEEE Control Systems Letters, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10374213)

   *Rebecca G. Hart, Emily J. Griffis, Omkar Sudhir Patil, and Warren E. Dixon.*

1. **Gain scheduling with a neural operator for a transport PDE with nonlinear recirculation.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.02511)

   *Maxence Lamarque, Luke Bhan, Rafael Vazquez, and Miroslav Krstic.*

1. **Physics-informed deep learning approach to solve optimal control problem.** AIAA, 2024. [paper](https://arc.aiaa.org/doi/abs/10.2514/6.2024-0945)

   *Kyung-Mi Na and Chang-Hun Lee.*

1. **Adaptive neural-operator backstepping control of a benchmark hyperbolic PDE.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.07862)

   *Maxence Lamarque, Luke Bhan, Yuanyuan Shi, and Miroslav Krstic.*

1. **Physical-informed neural network for MPC-based trajectory tracking of vehicles with noise considered.** TIV, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10414012)

   *Long Jin, Longqi Liu, Xingxia Wang, Mingsheng Shang, and Feiyue Wang.*

1. **Neural network approaches for parameterized optimal control.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.10033)

   *Deepanshu Verma, Nick Winovich, Lars Ruthotto, and Bart van Bloemen Waanders.*

1. **Physics-informed neural network policy iteration: Algorithms, convergence, and verification.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.10119)

   *Yiming Meng, Ruikun Zhou, Amartya Mukherjee, Maxwell Fitzsimmons, Christopher Song, and Jun Liu.*

1. **Nonlinear discrete-time observers with physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.12360)

   *Hector Vargas Alvarez, Gianluca Fabiani, Ioannis G. Kevrekidis, Nikolaos Kazantzis, and Constantinos Siettos.*

1. **Pathwise relaxed optimal control of rough differential equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.17900)

   *Prakash Chakraborty, Harsha Honnappa, and Samy Tindel.*

1. **Parametric PDE control with deep reinforcement learning and differentiable L^0-sparse polynomial policies.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.15267)

   *Nicolò Botteghi and Urban Fasel.*

1. **PDE control gym: A benchmark for data-driven boundary control of partial differential equations.** L4DC, 2024. [paper](https://arxiv.org/abs/2405.11401)

   *Luke Bhan, Yuexin Bian, Miroslav Krstic, and Yuanyuan Shi.*

1. **PhiBE: A PDE-based Bellman equation for continuous time policy evaluation.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.12535)

   *Yuhua Zhu.*

### [Climate](#content)
1. **FourCastNet: A global data-driven high-resolution weather model using adaptive Fourier neural operators.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.11214)

   *Jaideep Pathak, Shashank Subramanian, Peter Harrington, Sanjeev Raja, Ashesh Chattopadhyay, Morteza Mardani, Thorsten Kurth, David Hall, Zongyi Li, Kamyar Azizzadenesheli, Pedram Hassanzadeh, Karthik Kashinath, and Animashree Anandkumar.*

1. **Fourier neural operators for arbitrary resolution climate data downscaling.** JMLR, 2023. [paper](https://arxiv.org/abs/2305.14452)

   *Qidong Yang, Alex Hernandez-Garcia, Paula Harder, Venkatesh Ramesh, Prasanna Sattegeri, Daniela Szwarcman, Campbell D. Watson, and David Rolnick.*

1. **Modelling atmospheric dynamics with spherical Fourier neural operators.** ICLR, 2023. [paper](https://s3.us-east-1.amazonaws.com/climate-change-ai/papers/iclr2023/47/paper.pdf)

   *Boris Bonev, Thorsten Kurth, Christian Hundt, Jaideep Pathak, Maximilian Baust, Karthik Kashinath, and Anima Anandkumar.*

1. **Spatiotemporal modeling of European paleoclimate using doubly sparse Gaussian processes.** NIPS, 2022. [paper](https://arxiv.org/abs/2211.08160)

   *Seth D. Axen, Alexandra Gessner, Christian Sommer, Nils Weitzel, and Álvaro Tejero-Cantero.*

1. **ClimSim: An open large-scale dataset for training high-resolution physics emulators in hybrid multi-scale climate simulators.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.08754v2)

   *Sungduk Yu, Walter M. Hannah, Liran Peng, Mohamed Aziz Bhouri, Ritwik Gupta, Jerry Lin, Björn Lütjens, Justus C. Will, Tom Beucler, Bryce E. Harrop, Benjamin R. Hillman, Andrea M. Jenney, Savannah L. Ferretti, Nana Liu, Anima Anandkumar, Noah D. Brenowitz, Veronika Eyring, Pierre Gentine, Stephan Mandt, Jaideep Pathak, Carl Vondrick, Rose Yu, Laure Zanna, Ryan P. Abernathey, Fiaz Ahmed, David C. Bader, Pierre Baldi, Elizabeth A. Barnes, Gunnar Behrens, Christopher S. Bretherton, Julius J. M. Busecke, Peter M. Caldwell, Wayne Chuang, Yilun Han, Yu Huang, Fernando Iglesias-Suarez, Sanket Jantre, Karthik Kashinath, Marat Khairoutdinov, Thorsten Kurth, Nicholas J. Lutsko, Po-Lun Ma, Griffin Mooers, J. David Neelin, David A. Randall, Sara Shamekh, Akshay Subramaniam, Mark A. Taylor, Nathan M. Urban, Janni Yuval, Guang J. Zhang, Tian Zheng, and Michael S. Pritchard.*

1. **Seismic traveltime simulation for variable velocity models using physics-informed Fourier neural operator.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.03751)

   *Chao Song, Tianshuo Zhao, Umair bin Waheed, and Cai Liu.*

1. **DeepPhysiNet: Bridging deep learning and atmospheric physics for accurate and continuous weather modeling.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.04125)

   *Wenyuan Li, Zili Liu, Keyan Chen, Hao Chen, Shunlin Liang, Zhengxia Zou, and Zhenwei Shi.*

1. **Residual-enhanced physics-guided machine learning with hard constraints for subsurface flow in reservoir engineering.** TGRS, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10413628)

   *Haibo Cheng, Yunpeng He, Peng Zeng, and Valeriy Vyatkin.*

### [Mechanics](#content)
1. **Wavelet neural operator for solving parametric partial differential equations in computational mechanics problems.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782522007393)

   *Tapas Tripura and Souvik Chakraborty.*

1. **Graph neural networks for airfoil design.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.05469)

   *Florent Bonnet.*

1. **Exact Dirichlet boundary physics-informed neural network EPINN for solid mechanics.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523003080)

   *Jiaji Wang, Y.L. Mo, Bassam Izzuddin, and Chul-Woo Kim.*

1. **Solving multi-material problems in solid mechanics using physics-informed neural networks based on domain decomposition technology.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S004578252300244X)

   *Yu Diao, Jianchuan Yang, Ying Zhang, Dawei Zhang, and Yiming Du.*

1. **A novel key performance analysis method for permanent magnet coupler using physics-informed neural networks.** Engineering with Computers, 2023. [paper](https://link.springer.com/article/10.1007/s00366-023-01914-8)

   *Huayan Pu, Bo Tan, Jin Yi, Shujin Yuan, Jinglei Zhao, Ruqing Bai, and Jun Luo.*

1. **Mechanical characterization and inverse design of stochastic architected metamaterials using neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.13812)

   *Hanxun Jin, Enrui Zhang, Boyu Zhang, Sridhar Krishnaswamy, George Em Karniadakis, and Horacio D. Espinosa.*

1. **A deep learning energy-based method for classical elastoplasticity.** International Journal of Plasticity, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0749641923000177)

   *Junyan He, Diab Abueidda, Rashid Abu Al-Ru, Seid Koric, and Iwona Jasiuk.*

1. **Physics-informed neural networks for magnetostatic problems on axisymmetric transformer geometries.** IEEE Journal of Emerging and Selected Topics in Industrial Electronics, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10373037)

   *Philipp Brendel, Vlad Medvedev, and Andreas Rosskopf.*

1. **Neural born series operator for biomedical ultrasound computed tomography.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.15575)

   *Zhijun Zeng, Yihang Zheng, Youjia Zheng, Yubing Li, Zuoqiang Shi, and He Sun.*

1. **Learning thermoacoustic interactions in combustors using a physics-informed neural network.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.00061)

   *Sathesh Mariappan, Kamaljyoti Nath, and George Em Karniadakis.*

1. **Flight dynamic uncertainty quantification modeling using physics-informed neural networks.** AIAA, 2024. [paper](https://arc.aiaa.org/doi/abs/10.2514/6.2024-0575)

   *Nathaniel Michek, Piyush Mehta, and Wade Huebsch.*

1. **Peridynamic neural operators: A data-driven nonlocal constitutive model for complex material responses.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.06070)

   *Siavash Jafarzadeh, Stewart Silling, Ning Liu, Zhongqiang Zhang, and Yue Yu.*

1. **Stochastic dynamics of aircraft ground taxiing via improved physics-informed neural networks.** Nonlinear Dynamics, 2024. [paper](https://link.springer.com/article/10.1007/s11071-023-09173-4)

   *Ying Zhang, Zhengrong Jin, Long Wang, Kaixin Zheng, and Wantao Jia.*

1. **Damage identification for plate structures using physics-informed neural networks.** MSSP, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0888327024000098)

   *Wei Zhou and Yongfeng Xu.*

1. **Quantification of gradient energy coefficients using physics-informed neural networks.** International Journal of Mechanical Sciences, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0020740324002522)

   *Lan Shang, Yunhong Zhao, Sizheng Zheng, Jin Wang, Tongyi Zhang, and Jie Wang.*

1. **MPIPN: A multi physics-informed PointNet for solving parametric acoustic-structure systems.** arXiv, 2024. [paper](https://arxiv.org/abs/2403.01132)

   *Chu Wang, Jinhong Wu, Yanzhi Wang, Zhijian Zha, and Qi Zhou.*

1. **A hierarchically normalized physics-informed neural network for solving differential equations: Application for solid mechanics problems.** EAAI, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S095219762400558X)

   *Thang Le-Duc, Seunghye Lee, H. Nguyen-Xuan , and Jaehong Lee.*

1. **Physics-informed machine learning using low-fidelity flowfields for inverse airfoil shape design.** AIAA, 2024. [paper](https://arc.aiaa.org/doi/abs/10.2514/1.J063570)

   *Benjamin Y. J. Wong, Murali Damodaran, and Boo Cheong Khoo.*

1. **A hard constraint and domain decomposition based physics-informed neural network framework for nonhomogeneous transient thermal analysis.** TCPMT, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10562356)

   *Zengkai Wu, Li Jun Jiang, Sheng Sun, and Ping Li.*

### [Robotics](#content)
1. **Hybrid learning of time-series inverse dynamics models for locally isotropic robot motion.** RAL, 2022. [paper](https://ieeexplore.ieee.org/document/9954138)

   *Tolga-Can Çallar and Sven Böttger.*

1. **NTFields: Neural time fields for physics-informed robot motion planning.** ICLR, 2023. [paper](https://openreview.net/forum?id=ApF0dmi1_9K)

   *Ruiqi Ni and Ahmed H Qureshi.*

1. **Online parameter estimation using physics-informed deep learning for vehicle stability algorithms.** arXiv, 2023. [paper](https://arxiv.org/abs/2303.00474)

   *Kemal Koysuren, Ahmet Faruk Keles, and Melih Cakmakci.*

1. **A locality-based neural solver for optical motion capture.** SIGGRAPH, 2023. [paper](https://arxiv.org/abs/2309.00428)

   *Xiaoyu Pan, Bowen Zheng, Xinwei Jiang, Guanglong Xu, Xianli Gu, Jingxiang Li, Qilong Kou, He Wang, Tianjia Shao, Kun Zhou, and Xiaogang Jin.*

1. **Approximating high-dimensional minimal surfaces with physics-informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.02589)

   *Steven Zhou and Xiaojing Ye.*

1. **A spatial-temporally adaptive PINN framework for 3D bi-ventricular electrophysiological simulations and parameter inference.** MICCAI, 2023. [paper](https://link.springer.com/chapter/10.1007/978-3-031-43990-2_16)

   *Yubo Ye, Huafeng Liu, Xiajun Jiang, Maryam Toloubidokhti, and Linwei Wang.*

1. **Using the Transformer model for physical simulation: An application on transient thermal analysis for 3D printing process simulation.** NIPS, 2023. [paper](https://openreview.net/forum?id=tuXhnv6pgo)

   *Qian Chen, Luyang Kong, Florian Dugast, and Albert To.*

1. **Physics-informed neural network for solution of forward and inverse kinematic wave problems.** Journal of Hydrology, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0022169424003287)

   *Qingzhi Hou, Yixin Li, Vijay P. Singh, Zewei Sun, and Jianguo Wei.*

1. **PhyGrasp: Generalizing robotic grasping with physics-informed large multimodal models.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.16836)

   *Dingkun Guo, Yuqi Xiang, Shuqi Zhao, Xinghao Zhu, Masayoshi Tomizuka, Mingyu Ding, and Wei Zhan.*

1. **Structure-preserving operator learning: Modeling the collision operator of kinetic equations.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.16613)

   *Jae Yong Lee, Steffen Schotthöfer, Tianbai Xiao, Sebastian Krumscheid, and Martin Frank.*

### [Physics](#content)
1. **Dynamic weights enabled physics-informed neural network for simulating the mobility of engineered nano-particles in a contaminated aquifer.** NIPS, 2022. [paper](https://arxiv.org/pdf/2211.03525.pdf)

   *Shikhar Nilabh and Fidel Grandia.*

1. **Learning two-phase microstructure evolution using neural operators and autoencoder architectures.** NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00876-7)

   *Vivek Oommen, Khemraj Shukla, Somdatta Goswami, Rémi Dingreville, and George Em Karniadakis.*

1. **Predicting glass structure by physics-informed machine learning.** NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00882-9)

   *Mikkel L. Bødker, Mathieu Bauchy, Tao Du, John C. Mauro, and Morten M. Smedskjaer.*

1. **Physics-informed deep learning for solving phonon Boltzmann transport equation with large temperature non-equilibrium.** NPJ Computational Materials, 2022. [paper](https://www.nature.com/articles/s41524-022-00712-y)

   *Ruiyang Li, Jianxun Wang, Eungkyu Lee, and Tengfei Luo.*

1. **Design of Turing systems with physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.13464)

   *Jordon Kho, Winston Koh, Jian Cheng Wong, Pao-Hsiung Chiu, and Chin Chun Ooi.*

1. **Spatio-temporal super-resolution of dynamical systems using physics-informed deep-learning.** AAAI, 2023. [paper](https://arxiv.org/abs/2212.04457)

   *Rajat Arora and Ankit Shrivastava.*

1. **Rapid seismic waveform modeling and inversion with neural operators.** TGRS, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10091544)

   *Yan Yang, Angela F. Gao, Kamyar Azizzadenesheli, Robert W. Clayton, and Zachary E. Ross.*

1. **Accelerating heat exchanger design by combining Physics-Informed deep learning and transfer learning.** Chemical Engineering Science, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0009250923008412)

   *Zhiyong Wu, Bingjian Zhang, Haoshui Yu, Jingzheng Ren, Ming Pan, Chang He, and Qinglin Chen.*

1. **Energy stable neural network for gradient flow equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.10002)

   *Ganghua Fan, Tianyu Jin, Yuan Lan, Yang Xiang, and Luchan Zhang.*

1. **Physics-informed neural network with transfer learning (TL-PINN) based on domain similarity measure for prediction of nuclear reactor transients.** Scientific Reports, 2023. [paper](https://www.nature.com/articles/s41598-023-43325-1)

   *Konstantinos Prantikos, Stylianos Chatzidakis, Lefteri H. Tsoukalas, and Alexander Heifetz.*

1. **Plasma surrogate modelling using Fourier neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.05967)

   *Vignesh Gopakumar, Stanislas Pamela, Lorenzo Zanisi, Zongyi Li, Ander Gray, Daniel Brennand, Nitesh Bhatia, Gregory Stathopoulos, Matt Kusner, Marc Peter Deisenroth, Anima Anandkumar, JOREK Team, and MAST Team.*

1. **Training a deep operator network as a surrogate solver for two-dimensional parabolic-equation models.** Journal of the Acoustical Society of America, 2023. [paper](https://pubs.aip.org/asa/jasa/article-abstract/154/5/3276/2922093/Training-a-deep-operator-network-as-a-surrogate?redirectedFrom=fulltext)

   *Liang Xu, Haigang Zhang, and Minghui Zhang.*

1. **Grad-Shafranov equilibria via data-free physics informed neural networks.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.13491)

   *Byoungchan Jang, Alan A. Kaptanoglu, Rahul Gaur, Shaw Pan, Matt Landreman, and William Dorland.*

1. **Physics-informed deep learning of rate-and-state fault friction.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.09403)

   *Cody Rucker and Brittany A. Erickson.*

1. **Physics-informed neural networks with embedded analytical models: Inverse design of multilayer dielectric-loaded rectangular waveguide devices.** IEEE Transactions on Microwave Theory and Techniques, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10372139)

   *Yinqing Pan, Ren Wang, and Bingzhong Wang.*

1. **En-DeepONet: An enrichment approach for enhancing the expressivity of neural operators with applications to seismology.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/pii/S0045782523008046)

   *Ehsan Haghighat, Umair bin Waheed, and George Karniadakis.*

1. **Solving seismic wave equations on variable velocity models with Fourier neural operator.** TGRS, 2023. [paper](https://ieeexplore.ieee.org/abstract/document/10319762)

   *Bian Li, Hanchen Wang, Shihang Feng, Xiu Yang, and Youzuo Lin.*

1. **Calculating quasi-normal modes of Schwarzschild black holes with physics informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.01440)

   *Nirmal Patel, Aycin Aykutalp, and Pablo Laguna.*

1. **Deep neural operator-driven real-time inference to enable digital twin solutions for nuclear energy systems.** Scientific Reports, 2024. [paper](https://www.nature.com/articles/s41598-024-51984-x)

   *Kazuma Kobayashi and Syed Bahauddin Alam.*

1. **A physics-informed deep learning description of Knudsen layer reactivity reduction.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.08495)

   *Christopher J. McDevitt and Xianzhu Tang.*

1. **Inverse design method for horn antennas based on knowledge-embedded physics-informed neural networks.** IEEE Antennas and Wireless Propagation Letters, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10433641)

   *Jinpin Liu, Bingzhong Wang, Chuan-Sheng Chen, and Ren Wang.*

1. **Combined analysis of thermofluids and electromagnetism using physics-informed neural networks.** EAAI, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10433641)

   *Yeonhwi Jeong, Junhyoung Jo, Tonghun Lee, and Jihyung Yoo.*

1. **Fully convolutional network enhanced DeepONet-based surrogate of predicting the travel-time fields.** TGRS, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10530929)

   *Yifan Mei, Yijie Zhang, Xueyu Zhu, Rongxi Gou, and Jinghuai Gao.*

1. **Seismic wavefields modeling with variable horizontally-layered velocity models via velocity-encoded PINN.** TGRS, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10551894)

   *Jingbo Zou, Cai Liu, Pengfei Zhao, and Chao Song.*

1. **SPI-MIONet for surrogate modeling in phase-field hydraulic fracturing.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782524003104)

   *Xiaoqiang Wang, Peichao Li, Kaile Jia, Shaoqi Zhang, Chun Li, Bangchen Wu, Yilun Dong, and Detang Lu.*

### [Image](#content)
1. **Learning to diffuse: A new perspective to design PDEs for visual analysis.** TPAMI, 2016. [paper](https://ieeexplore.ieee.org/document/7393839)

   *Risheng Liu, Guangyu Zhong, Junjie Cao, Zhouchen Lin, Shiguang Shan, and Zhongxuan Luo.*

1. **Reformulating optical flow to solve image-based inverse problems and quantify uncertainty.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9870569)

   *Aleix Boquet-Pujadas and Jean-Christophe Olivo-Marin.*

1. **WarpPINN: Cine-MR image registration with physics-informed neural networks.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.12549)

   *Pablo Arratia Lopez, Hernan Mella, Sergio Uribe, Daniel E. Hurtado, and Francisco Sahli Costabal.*

1. **NODE-ImgNet: A PDE-informed effective and robust model for image denoising.** arXiv, 2023. [paper](https://arxiv.org/abs/2305.11049)

   *Xinheng Xie, Yue Wu, Hao Nib, and Cuiyu He.*

1. **Microscopy image reconstruction with physics-informed denoising diffusion probabilistic model.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.02929)

   *Rui Li, Gabriel della Maggiora, Vardan Andriasyan, Anthony Petkidis, Artsemi Yushkevich, Mikhail Kudryashev, and Artur Yakimovich.*

1. **TGM-Nets: A deep learning framework for enhanced forecasting of tumor growth by integrating imaging and modeling.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623010515)

   *Qijing Chen, Qi Ye, Weiqi Zhang, He Li, and Xiaoning Zheng.*

1. **The use of physics-informed neural network approach to image restoration via nonlinear PDE tools.** Computers & Mathematics with Applications, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0898122123004431)

   *Neda Namaki, M.R. Eslahchi, and Rezvan Salehi.*

1. **Personalized predictions of glioblastoma infiltration: Mathematical models, physics-informed neural networks and multimodal scans.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.16536)

   *Ray Zirui Zhang, Ivan Ezhov, Michal Balcerak, Andy Zhu, Benedikt Wiestler, Bjoern Menze, and John Lowengrub.*

1. **Real-time FJ/MAC PDE solvers via tensorized, back-propagation-free optical PINN training.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.00413)

   *Yequan Zhao, Xian Xian, Xinling Yu, Ziyue Liu, Zhixiong Chen, Geza Kurczveil, Raymond G. Beausoleil, and Zheng Zhang.*

1. **Performance of Fourier-based activation function in physics-informed neural networks for patient-specific cardiovascular flows.** Computer Methods and Programs in Biomedicine, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S0169260724000774)

   *Arman Aghaee and M. Owais Khan.*

1. **Effective medium properties of stealthy hyperuniform photonic structures using multiscale physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2405.07878)

   *Roberto Riganti, Yilin Zhu, Wei Cai, Salvatore Torquato, and Luca Dal Negro.*

### [Chemistry](#content)
1. **Combustion chemistry acceleration with DeepONets.** Fuel, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0016236124003582)

   *Anuj Kumar and Tarek Echekki.*

### [Materials](#content)
1. **Microstructure-sensitive deformation modeling and materials design with physics-informed neural networks.** AIAA Journal, 2024. [paper](https://arc.aiaa.org/doi/abs/10.2514/1.J062708)

   *Mahmudul Hasan, Zekeriya Ender Eger, Arulmurugan Senthilnathan, and Pınar Acar.*

1. **A novel Fourier neural operator framework for classification of multi-sized images: Application to three dimensional digital porous media.** Physics of Fluids, 2024. [paper](https://pubs.aip.org/aip/pof/article/36/5/057131/3293884)

   *Ali Kashefi and Tapan Mukerji.*

1. **A fast learning-based surrogate of electrical machines using a reduced basis.** ICML, 2024. [paper](https://openreview.net/forum?id=IK8CLXqffb)

   *Alejandro Ribés, Nawfal Benchekroun, and Théo Delagnes.*

### [Molecules](#content)
1. **Symmetry-informed geometric representation for molecules, proteins, and crystalline materials.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.09375)

   *Shengchao Liu, Weitao Du, Yanjing Li, Zhuoxinran Li, Zhiling Zheng, Chenru Duan, Zhiming Ma, Omar Yaghi, Anima Anandkumar, Christian Borgs, Jennifer Chayes, Hongyu Guo, and Jian Tang.*

1. **Solving nonconvex energy minimization problems in martensitic phase transitions with a mesh-free deep learning approach.** CMAME, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S004578252300508X)

   *Xiaoli Chen, Phoebus Rosakis, Zhizhang Wu, and Zhiwen Zhang.*

1. **A physics-guided bi-fidelity Fourier-featured operator learning framework for predicting time evolution of drag and lift coefficients.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.03639)

   *Amirhossein Mollaali, Izzet Sahin, Iqrar Raza, Christian Moya, Guillermo Paniagua, and Guang Lin.*

1. **Mixed form based physics-informed neural networks for performance evaluation of two-phase random materials.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623014343)

   *Xiaodan Ren and Xianrui Lyu.*

1. **Deep learning based solution of nonlinear partial differential equations arising in the process of arterial blood flow.** Mathematics and Computers in Simulation, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0378475423004469)

   *Bivas Bhaumik, Soumen De, and Satyasaran Changdar.*

1. **Physics-informed neural networks for solving dynamic two-phase interface problems.** SIAM Journal on Scientific Computing, 2023. [paper](https://epubs.siam.org/doi/abs/10.1137/22M1517081)

   *Xingwen Zhu, Xiaozhe Hu, and Pengtao Sun.*

1. **Rethinking materials simulations: Blending direct numerical simulations with neural operators.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.05410)

   *Vivek Oommen, Khemraj Shukla, Saaketh Desai, Remi Dingreville, and George Em Karniadakis.*

1. **A conservative hybrid physics-informed neural network method for Maxwell-Ampère-Nernst-Planck equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.05891)

   *Cheng Chang, Zhouping Xin, and Tieyong Zeng.*

1. **A data-driven physics-constrained deep learning computational framework for solving von Mises plasticity.** EAAI, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0952197623002336)

   *Arunabha M. Roy and Suman Guha.*

1. **Learning stiff chemical kinetics using extended deep neural operators.** CMAME, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0045782523007971)

   *Somdatta Goswami, Ameya D. Jagtap, Hessam Babaee, Bryan T. Susi, and George Em Karniadakis.*

1. **Deep-learning based parameter identification enables rationalization of battery material evolution in complex electrochemical systems.** Journal of Computational Science, 2023. [paper](https://www.sciencedirect.com/science/article/abs/pii/S1877750322002599)

   *Ivonne Sgura, Luca Mainetti, Francesco Negro, Maria Grazia Quarta, and Benedetto Bozzini.*

1. **AI-aided geometric design of anti-infection catheters.** Science Advances, 2023. [paper](https://www.science.org/doi/10.1126/sciadv.adj1741)

   *Tingtao Zhou, Xuan Wan, Daniel Zhengyu Huang, Zongyi Li, Zhiwei Peng, Anima Anandkumar, John F. Brady, Paul W. Sternberg, and Chiara Daraio.*

1. **Physics-informed deep learning to solve three-dimensional Terzaghi’s consolidation equation: Forward and inverse problems.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.05439)

   *Biao Yuan, Ana Heitor, He Wang, and Xiaohui Chen.*

1. **Solving the discretised multiphase flow equations with interface capturing on structured grids using machine learning libraries.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.06755)

   *Boyang Chen, Claire E. Heaney, Jefferson L. M. A. Gomes, Omar K. Matar, and Christopher C. Pain.*

1. **Combustion chemistry acceleration with DeepONets.** Fuel, 2024. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0016236124003582)

   *Anuj Kumar and Tarek Echekki.*

1. **Identifying heterogeneous micromechanical properties of biological tissues via physics-informed neural networks.** arXiv, 2024. [paper](https://arxiv.org/abs/2402.10741v1)

   *Wensi Wu, Mitchell Daneker, Kevin T. Turner, Matthew A. Jolley, and Lu Lu.*

1. **Adaptive data-driven deep-learning surrogate model for frontal polymerization in dicyclopentadiene.** The Journal of Physical Chemistry B, 2024. [paper](https://pubs.acs.org/doi/abs/10.1021/acs.jpcb.3c07714)

   *Qibang Liu, Diab Abueidda, Sagar Vyas, Yuan Gao, Seid Koric, and Philippe H. Geubelle.*

### [Reconstruction](#content)
1. **Occupancy networks: Learning 3D reconstruction in function space.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mescheder_Occupancy_Networks_Learning_3D_Reconstruction_in_Function_Space_CVPR_2019_paper.pdf)

   *Lars Mescheder, Michael Oechsle, Michael Niemeyer, Sebastian Nowozin, and Andreas Geiger.*
   
1. **Transfer learning for flow reconstruction based on multifidelity data.** AIAA Journal, 2022. [paper](https://arc.aiaa.org/doi/abs/10.2514/1.J061647)

   *Jiaqing Kou, Chenjia Ning, and Weiwei Zhang.*

1. **Learning-based state reconstruction for a scalar hyperbolic PDE under noisy lagrangian sensing.** L4DC, 2022. [paper](http://proceedings.mlr.press/v144/barreau21a.html)

   *Matthieu Barreau, John Liu, and Karl Henrik Johansson.*

### [Quantum](#content)
1. **Physics-informed neural networks for quantum eigenvalue problems.** IJCNN, 2022. [paper](https://ieeexplore.ieee.org/document/9891944)

   *Henry Jin, Marios Mattheakis, and Pavlos Protopapas.*

1. **Quantum-inspired tensor neural networks for partial differential equations.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.02235)

   *Raj Patel, Chia-Wei Hsing, Serkan Sahin, Saeed S. Jahromi, Samuel Palmer, Shivam Sharma, Christophe Michel, Vincent Porte, Mustafa Abid, Stephane Aubert, Pierre Castellani, Chi-Guhn Lee, Samuel Mugel, and Roman Orus.*

1. **Quantum Fourier networks for solving parametric PDEs.** arXiv, 2023. [paper](https://arxiv.org/abs/2306.15415)

   *Nishant Jain, Jonas Landman, Natansh Mathur, and Iordanis Kerenidis.*

1. **Q-Flow: Generative modeling for differential equations of open quantum dynamics with normalizing flows.** ICML, 2023. [paper](https://openreview.net/forum?id=0rnA1l6WAc)

   *Owen M Dugan, Peter Y. Lu, Rumen Dangovski, Di Luo, and Marin Soljacic.*

1. **Physics-informed quantum machine learning: Solving nonlinear differential equations in latent spaces without costly grid evaluations.** arXiv, 2023. [paper](https://arxiv.org/abs/2308.01827)

   *Annie E. Paine, Vincent E. Elfving, and Oleksandr Kyriienko.*

1. **Physics-informed quantum machine learning for solving partial differential equations.** arXiv, 2023. [paper](https://arxiv.org/abs/2312.09215)

   *Abhishek Setty, Rasul Abdusalamov, and Mikhail Itskov.*

### [Game Theory](#content)
1. **Approximating discontinuous Nash equilibria values of two-player general-sum differential games.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.01773)

   *Lei Zhang, Mukesh Ghimire, Wenlong Zhang, Zhe Xu, and Yi Ren.*

1. **Solving two-player general-sum games between swarms.** arXiv, 2023. [paper](https://arxiv.org/abs/2310.01682)

   *Mukesh Ghimire, Lei Zhang, Wenlong Zhang, Yi Ren, and Zhe Xu.*

1. **Value approximation for two-player general-sum differential games with state constraints.** arXiv, 2023. [paper](https://arxiv.org/abs/2311.16520)

   *Lei Zhang, Mukesh Ghimire, Wenlong Zhang, Zhe Xu, and Yi Ren.*

1. **Pontryagin neural operator for solving parametric general-sum differential games.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.01502)

   *Lei Zhang, Mukesh Ghimire, Zhe Xu, Wenlong Zhang, and Yi Ren.*

1. **Unsupervised solution operator learning for mean-field games via sampling-invariant parametrizations.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.15482)

   *Han Huang and Rongjie Lai .*

### [Industry](#content)
1. **Physics-aware machine learning surrogates for real-time manufacturing digital twin.** Manufacturing Letters, 2022. [paper](https://www.sciencedirect.com/science/article/abs/pii/S2213846322001845)

   *Aditya Balu, Soumik Sarkar, Baskar Ganapathysubramanian, and Adarsh Krishnamurthy.*

1. **Multi-scale digital twin: Developing a fast and physics-informed surrogate model for groundwater contamination with uncertain climate models.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.10884)

   *Lijing Wang, Takuya Kurihana, Aurelien Meray, Ilijana Mastilovic, Satyarth Praveen, Zexuan Xu, Milad Memarzadeh, Alexander Lavin, and Haruko Wainwright.*

1. **SciAI4Industry--Solving PDEs for industry-scale problems with deep learning.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.12709)

   *Philipp A. Witte, Russell J. Hewett, Kumar Saurabh, AmirHossein Sojoodi, and Ranveer Chandra.*

1. **Operator learning framework for digital twin and complex engineering systems.** arXiv, 2023. [paper](https://arxiv.org/abs/2301.06701)

   *Kazuma Kobayashi, James Daniell, and Syed B. Alam.*

1. **Towards solving industry-grade surrogate modeling problems using physics informed machine learning.** arXiv, 2023. [paper](https://arxiv.org/abs/2309.03374)

   *Saakaar Bhatnagar, Andrew Comerford, and Araz Banaeizadeh.*

1. **Data-driven physics-informed neural networks: A digital twin perspective.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.08667)

   *Sunwoong Yang, Hojin Kim, Yoonpyo Hong, Kwanjung Yee, Romit Maulik, and Namwoo Kang.*

1. **Physically informed synchronic-adaptive learning for industrial systems modeling in heterogeneous media with unavailable time-varying interface.** arXiv, 2024. [paper](https://arxiv.org/abs/2401.14609)

   *Aina Wang, Pan Qin, and Ximing Sun.*

1. **Improved generalization with deep neural operators for engineering systems: Path towards digital twin.** EAAI, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S0952197624000022)

   *Kazuma Kobayashi, James Daniell, and Syed Bahauddin Alam.*

1. **A deep transfer operator learning method for temperature field reconstruction in a lithium-ion battery pack.** TII, 2024. [paper](https://ieeexplore.ieee.org/abstract/document/10462637)

   *Yuchen Wang, Can Xiong, Changjiang Ju, Genke Yang, Yuwang Chen, and Xiaotian Yu.*

1. **ro-PINN: A reduced order physics-informed neural network for solving the macroscopic model of pedestrian flows.** Transportation Research Part C: Emerging Technologies, 2024. [paper](https://www.sciencedirect.com/science/article/pii/S0968090X24001797)

   *Renbin Pan, Feng Xiao, and Minyu Shen.*

### [Economics](#content)
1. **A deep learning based numerical PDE method for option pricing.** Computational Economics, 2023. [paper](https://link.springer.com/article/10.1007/s10614-022-10279-x)

   *Xiang Wang, Jessica Li, and Jichun Li.*R