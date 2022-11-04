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
<tr><td colspan="2"><a href="#applications">3. Applications</a></td></tr> 
<tr>
    <td>&ensp;<a href="#physics">3.1 Physics</a></td>
    <td>&ensp;<a href="#chemistry-and-biology">3.2 Chemistry and Biology</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#knowledge-graph">3.3 Knowledge Graph</a></td>
    <td>&ensp;<a href="#recommender-systems">3.4 Recommender Systems</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#computer-vision">3.5 Computer Vision</a></td>
    <td>&ensp;<a href="#natural-language-processing">3.6 Natural Language Processing</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#generation">3.7 Generation</a></td>
    <td>&ensp;<a href="#combinatorial-optimization">3.8 Combinatorial Optimization</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#adversarial-attack">3.9 Adversarial Attack</a></td>
    <td>&ensp;<a href="#graph-clustering">3.10 Graph Clustering</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#graph-classification">3.11 Graph Classification</a></td>
    <td>&ensp;<a href="#reinforcement-learning">3.12 Reinforcement Learning</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#traffic-network">3.13 Traffic Network</a></td>
    <td>&ensp;<a href="#few-shot-and-zero-shot-learning">3.14 Few-shot and Zero-shot Learning</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#program-representation">3.15 Program Representation</a></td>
    <td>&ensp;<a href="#social-network">3.16 Social Network</a></td>
</tr> 
<tr>
    <td>&ensp;<a href="#graph-matching">3.17 Graph Matching</a></td>
    <td>&ensp;<a href="#computer-network">3.18 Computer Network</a></td>
</tr>
</table>






## [Survey papers](#content)

1. **Physics-informed machine learning.** Nature Reviews Physics, 2021. [paper](https://www.nature.com/articles/s42254-021-00314-5)

   *George Em Karniadakis, Ioannis G. Kevrekidis, Lu Lu, Paris Perdikaris, Sifan Wang, and Liu Yang.*

1. **DeepXDE: A Deep Learning Library for Solving Differential Equations.** SIAM Review, 2021. [paper](https://epubs.siam.org/doi/abs/10.1137/19M1274067)

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
   
1. </details>

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

1. **Representation Learning on Graphs with Jumping Knowledge Networks.** ICML 2018. [paper](https://arxiv.org/pdf/1806.03536.pdf)

   *Keyulu Xu, Chengtao Li, Yonglong Tian, Tomohiro Sonobe, Ken-ichi Kawarabayashi, Stefanie Jegelka.* 

1. **Deeper Insights into Graph Convolutional Networks for Semi-Supervised Learning.** AAAI 2018. [paper](https://arxiv.org/pdf/1801.07606.pdf)

   *Qimai Li, Zhichao Han, Xiao-Ming Wu.*

1. **How Powerful are Graph Neural Networks?** ICLR 2019. [paper](https://openreview.net/pdf?id=ryGs6iA5Km)

   *Keyulu Xu, Weihua Hu, Jure Leskovec, Stefanie Jegelka.*

1. **Stability and Generalization of Graph Convolutional Neural Networks.** KDD 2019. [paper](https://arxiv.org/pdf/1905.01004.pdf)

   *Saurabh Verma, Zhi-Li Zhang.*

1. **Simplifying Graph Convolutional Networks.** ICML 2019. [paper](https://arxiv.org/pdf/1902.07153)

   *Felix Wu, Tianyi Zhang, Amauri Holanda de Souza Jr., Christopher Fifty, Tao Yu, Kilian Q. Weinberger.*

1. **Explainability Methods for Graph Convolutional Neural Networks.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Pope_Explainability_Methods_for_Graph_Convolutional_Neural_Networks_CVPR_2019_paper.pdf)

   *Phillip E. Pope, Soheil Kolouri, Mohammad Rostami, Charles E. Martin, Heiko Hoffmann.*

1. **Can GCNs Go as Deep as CNNs?** ICCV 2019. [paper](https://arxiv.org/pdf/1904.03751.pdf)

   *Guohao Li, Matthias Müller, Ali Thabet, Bernard Ghanem.*

1. **Weisfeiler and Leman Go Neural: Higher-order Graph Neural Networks.** AAAI 2019. [paper](https://arxiv.org/pdf/1810.02244.pdf)    

   *Christopher Morris, Martin Ritzert, Matthias Fey, William L. Hamilton, Jan Eric Lenssen, Gaurav Rattan, Martin Grohe.*

1. **Understanding Attention and Generalization in Graph Neural Networks.** NeurIPS 2019. [paper](https://arxiv.org/pdf/1905.02850.pdf)

   *Boris Knyazev, Graham W. Taylor, Mohamed R. Amer.*

1. **GNNExplainer: Generating Explanations for Graph Neural Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-4956)

   *Zhitao Ying, Dylan Bourgeois, Jiaxuan You, Marinka Zitnik, Jure Leskovec.*

1. **Universal Invariant and Equivariant Graph Neural Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-3832)

   *Nicolas Keriven, Gabriel Peyré.*

1. **On the equivalence between graph isomorphism testing and function approximation with GNNs.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-9347)

   *Zhengdao Chen, Soledad Villar, Lei Chen, Joan Bruna.*

1. **Understanding the Representation Power of Graph Neural Networks in Learning Graph Topology.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-8876)

   *Nima Dehmamy, Albert-Laszlo Barabasi, Rose Yu.*

1. **Graph Neural Networks Exponentially Lose Expressive Power for Node Classification.** ICLR 2020. [paper](https://openreview.net/pdf?id=S1ldO2EFPr)

   *Kenta Oono, Taiji Suzuki.*

1. **What graph neural networks cannot learn: depth vs width.** ICLR 2020. [paper](https://openreview.net/pdf?id=B1l2bp4YwS)

   *Andreas Loukas.*

1. **The Logical Expressiveness of Graph Neural Networks.** ICLR 2020. [paper](https://openreview.net/pdf?id=r1lZ7AEKvB)

   *Pablo Barceló, Egor V. Kostylev, Mikael Monet, Jorge Pérez, Juan Reutter, Juan Pablo Silva.*

1. **On the Equivalence between Positional Node Embeddings and Structural Graph Representations.** ICLR 2020. [paper](https://openreview.net/pdf?id=SJxzFySKwH)

   *Balasubramaniam Srinivasan, Bruno Ribeiro.*

1. **Can Graph Neural Networks Count Substructures?** NeurIPS 2020. [paper](https://arxiv.org/pdf/2002.04025.pdf)

   *Zhengdao Chen, Lei Chen, Soledad Villar, Joan Bruna.*

### [Efficiency](#content)

1. **Stochastic Training of Graph Convolutional Networks with Variance Reduction.** ICML 2018. [paper](http://www.scipaper.net/uploadfile/2018/0716/20180716100330880.pdf)

   *Jianfei Chen, Jun Zhu, Le Song.*

1. **FastGCN: Fast Learning with Graph Convolutional Networks via Importance Sampling.** ICLR 2018. [paper](https://arxiv.org/pdf/1801.10247.pdf)

   *Jie Chen, Tengfei Ma, Cao Xiao.*

1. **Adaptive Sampling Towards Fast Graph Representation Learning.** NeurIPS 2018. [paper](https://arxiv.org/pdf/1809.05343.pdf)

   *Wenbing Huang, Tong Zhang, Yu Rong, Junzhou Huang.*

1. **Large-Scale Learnable Graph Convolutional Networks.** KDD 2018. [paper](https://arxiv.org/pdf/1808.03965.pdf)

   *Hongyang Gao, Zhengyang Wang, Shuiwang Ji.*

1. **Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks.** KDD 2019. [paper](https://arxiv.org/pdf/1905.07953.pdf)

   *Wei-Lin Chiang, Xuanqing Liu, Si Si, Yang Li, Samy Bengio, Cho-Jui Hsieh.*

1. **A Degeneracy Framework for Scalable Graph Autoencoders.** IJCAI 2019. [paper](https://arxiv.org/pdf/1902.08813.pdf)

   *Guillaume Salha, Romain Hennequin, Viet Anh Tran, Michalis Vazirgiannis.*

1. **Layer-Dependent Importance Sampling for Training Deep and Large Graph Convolutional Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-6006)

   *Difan Zou, Ziniu Hu, Yewen Wang, Song Jiang, Yizhou Sun, Quanquan Gu.*

1. **GraphSAINT: Graph Sampling Based Inductive Learning Method.** ICLR 2020. [paper](https://arxiv.org/pdf/1907.04931.pdf) [code](https://github.com/GraphSAINT/GraphSAINT)

   *Hanqing Zeng, Hongkuan Zhou, Ajitesh Srivastava, Rajgopal Kannan, Viktor Prasanna.*

1. **Scalable Graph Convolutional Network Based Link Prediction on a Distributed Graph Database Server.** IEEE CLOUD 2020. [paper](https://github.com/miyurud/miyurud.github.io/blob/master/papers/2020/IEEE_CLOUD_2020_JasmineGraph-web.pdf) [code](https://github.com/miyurud/jasminegraph)

   *Anuradha Karunarathna, Dinika Senarath, Shalika Madhushanki, Chinthaka Weerakkody, Miyuru Dayarathna, Sanath Jayasena, Toyotaro Suzumura.*


1. **Memory Efficient Graph Convolutional Networkbased Distributed Link Prediction.** IEEE Big Data 2020. [paper](https://raw.githubusercontent.com/miyurud/miyurud.github.io/master/papers/2020/IEEE_BigData_Workshop_2020_JasmineGraph_web.pdf) [code](https://github.com/miyurud/jasminegraph)

   *Damitha Senevirathne, Isuru Wijesiri, Suchitha Dehigaspitiya, Miyuru Dayarathna, Sanath Jayasena, and Toyotaro Suzumura.*


### [Explainability](#content)

1. **Explainability Techniques for Graph Convolutional Networks.** ICML 2019. [paper](https://arxiv.org/abs/1905.13686)

   *Federico Baldassarre, Hossein Azizpour.*

1. **GNNExplainer: Generating Explanations for Graph Neural Networks.** NeurIPS 2019. [paper](https://arxiv.org/abs/1903.03894)

   *Rex Ying, Dylan Bourgeois, Jiaxuan You, Marinka Zitnik, Jure Leskovec.*

1. **GCN-LRP Explanation: Exploring Latent Attention of Graph Convolutional Networks.** IJCNN 2020. [paper](https://ieeexplore.ieee.org/document/9207639)

   *Jinlong Hu, Tenghui Li, Shoubin Dong.*

1. **Parameterized Explainer for Graph Neural Network.** NeurIPS 2020. [paper](https://arxiv.org/abs/2011.04573)

   *Dongsheng Luo, Wei Cheng, Dongkuan Xu, Wenchao Yu, Bo Zong, Haifeng Chen, Xiang Zhang.*

1. **XGNN: Towards Model-Level Explanations of Graph Neural Networks.** KDD 2020. [paper](https://arxiv.org/abs/2006.02587)

   *Hao Yuan, Jiliang Tang, Xia Hu, Shuiwang Ji.*

1. **Contrastive Graph Neural Network Explanation.** ICML 2020. [paper](https://arxiv.org/abs/2010.13663)

   *Lukas Faber, Amin K. Moghaddam, Roger Wattenhofer.*

1. **Interpreting Graph Neural Networks for NLP With Differentiable Edge Maskin.** ICLR 2021. [paper](https://arxiv.org/abs/2010.00577)

   *Michael Sejr Schlichtkrull, Nicola De Cao, Ivan Titov.*

1. **On Explainability of Graph Neural Networks via Subgraph Explorations.** ICML 2021. [paper](https://arxiv.org/abs/2102.05152)

   *Hao Yuan, Haiyang Yu, Jie Wang, Kang Li, Shuiwang Ji.*

1. **Generative Causal Explanations for Graph Neural Networks.** ICML 2021. [paper](https://arxiv.org/abs/2104.06643)

   *Wanyu Lin, Hao Lan, Baochun Li.*

1. **GraphSVX: Shapley Value Explanations for Graph Neural Networks.** ECML PKDD 2021. [paper](https://arxiv.org/abs/2104.10482)

   *Alexandre Duval, Fragkiskos D. Malliaros.*


## [Applications](#content)

### [Physics](#content)

1. **Discovering objects and their relations from entangled scene representations.** ICLR Workshop 2017. [paper](https://arxiv.org/pdf/1702.05068.pdf)

   *David Raposo, Adam Santoro, David Barrett, Razvan Pascanu, Timothy Lillicrap, Peter Battaglia.*  

1. **A simple neural network module for relational reasoning.** NIPS 2017. [paper](https://arxiv.org/pdf/1706.01427.pdf)

   *Adam Santoro, David Raposo, David G.T. Barrett, Mateusz Malinowski, Razvan Pascanu, Peter Battaglia, Timothy Lillicrap.*  

1. **Interaction Networks for Learning about Objects, Relations and Physics.** NIPS 2016. [paper](https://arxiv.org/pdf/1612.00222.pdf)

   *Peter Battaglia, Razvan Pascanu, Matthew Lai, Danilo Rezende, Koray Kavukcuoglu.* 

1. **Visual Interaction Networks: Learning a Physics Simulator from Video.** NIPS 2017. [paper](http://papers.nips.cc/paper/7040-visual-interaction-networks-learning-a-physics-simulator-from-video.pdf)

   *Nicholas Watters, Andrea Tacchetti, Théophane Weber, Razvan Pascanu, Peter Battaglia, Daniel Zoran.* 

1. **Graph networks as learnable physics engines for inference and control.** ICML 2018. [paper](https://arxiv.org/pdf/1806.01242.pdf)

   *Alvaro Sanchez-Gonzalez, Nicolas Heess, Jost Tobias Springenberg, Josh Merel, Martin Riedmiller, Raia Hadsell, Peter Battaglia.* 

1. **Learning Multiagent Communication with Backpropagation.** NIPS 2016. [paper](https://arxiv.org/pdf/1605.07736.pdf)

   *Sainbayar Sukhbaatar, Arthur Szlam, Rob Fergus.* 

1. **VAIN: Attentional Multi-agent Predictive Modeling.** NIPS 2017 [paper](https://arxiv.org/pdf/1706.06122.pdf)

   *Yedid Hoshen.* 

1. **Neural Relational Inference for Interacting Systems.** ICML 2018. [paper](https://arxiv.org/pdf/1802.04687.pdf)

   *Thomas Kipf, Ethan Fetaya, Kuan-Chieh Wang, Max Welling, Richard Zemel.* 

1. **Graph Element Networks: adaptive, structured computation and memory.** ICML 2019. [paper](https://arxiv.org/pdf/1904.09019)

   *Ferran Alet, Adarsh K. Jeewajee, Maria Bauza, Alberto Rodriguez, Tomas Lozano-Perez, Leslie Pack Kaelbling.*

1. **Physics-aware Difference Graph Networks for Sparsely-Observed Dynamics.** ICLR 2020. [paper](https://openreview.net/pdf?id=r1gelyrtwH)

   *Sungyong Seo, Chuizheng Meng, Yan Liu.*

### [Chemistry and Biology](#content)

1. **Convolutional networks on graphs for learning molecular fingerprints.** NIPS 2015. [paper](https://arxiv.org/pdf/1509.09292.pdf)

   *David Duvenaud, Dougal Maclaurin, Jorge Aguilera-Iparraguirre, Rafael Gómez-Bombarelli, Timothy Hirzel, Alán Aspuru-Guzik, Ryan P. Adams.* 

1. **Molecular Graph Convolutions: Moving Beyond Fingerprints.** Journal of computer-aided molecular design 2016. [paper](https://arxiv.org/pdf/1603.00856.pdf)

   *Steven Kearnes, Kevin McCloskey, Marc Berndl, Vijay Pande, Patrick Riley.* 

1. **Protein Interface Prediction using Graph Convolutional Networks.** NIPS 2017. [paper](http://papers.nips.cc/paper/7231-protein-interface-prediction-using-graph-convolutional-networks.pdf)

   *Alex Fout, Jonathon Byrd, Basir Shariat, Asa Ben-Hur.* 

1. **Hybrid Approach of Relation Network and Localized Graph Convolutional Filtering for Breast Cancer Subtype Classification.** IJCAI 2018. [paper](https://arxiv.org/abs/1711.05859)

   *Sungmin Rhee, Seokjun Seo, Sun Kim.*

1. **Modeling polypharmacy side effects with graph convolutional networks.** ISMB 2018. [paper](https://arxiv.org/abs/1802.00543)

   *Marinka Zitnik, Monica Agrawal, Jure Leskovec.*

1. **Spectral Multigraph Networks for Discovering and Fusing Relationships in Molecules.** NeurIPS Workshop 2018. [paper](https://arxiv.org/pdf/1811.09595.pdf)

   *Boris Knyazev, Xiao Lin, Mohamed R. Amer, Graham W. Taylor.*

1. **MR-GNN: Multi-Resolution and Dual Graph Neural Network for Predicting Structured Entity Interactions.** IJCAI 2019. [paper](https://arxiv.org/pdf/1905.09558.pdf)

   *Nuo Xu, Pinghui Wang, Long Chen, Jing Tao, Junzhou Zhao.*

1. **Pre-training of Graph Augmented Transformers for Medication Recommendation.** IJCAI 2019. [paper](https://arxiv.org/pdf/1906.00346.pdf)

   *Junyuan Shang, Tengfei Ma, Cao Xiao, Jimeng Sun.*

1. **GAMENet: Graph Augmented MEmory Networks for Recommending Medication Combination.** AAAI 2019. [paper](https://arxiv.org/pdf/1809.01852.pdf)

   *Junyuan Shang, Cao Xiao, Tengfei Ma, Hongyan Li, Jimeng Sun.*

1. **AffinityNet: semi-supervised few-shot learning for disease type prediction.** AAAI 2019. [paper](https://arxiv.org/pdf/1805.08905.pdf)

   *Tianle Ma, Aidong Zhang.*

1. **Graph Transformation Policy Network for Chemical Reaction Prediction.** KDD 2019. [paper](https://arxiv.org/pdf/1812.09441)

   *Kien Do, Truyen Tran, Svetha Venkatesh.*

1. **Functional Transparency for Structured Data: a Game-Theoretic Approach.** ICML 2019. [paper](https://arxiv.org/pdf/1902.09737)

   *Guang-He Lee, Wengong Jin, David Alvarez-Melis, Tommi S. Jaakkola.*

1. **Learning Multimodal Graph-to-Graph Translation for Molecular Optimization.** ICLR 2019. [paper](https://openreview.net/pdf?id=B1xJAsA5F7)

   *Wengong Jin, Kevin Yang, Regina Barzilay, Tommi Jaakkola.*

1. **A Generative Model For Electron Paths.** ICLR 2019. [paper](https://openreview.net/pdf?id=r1x4BnCqKX)

   *John Bradshaw, Matt J. Kusner, Brooks Paige, Marwin H. S. Segler, José Miguel Hernández-Lobato.*

1. **Retrosynthesis Prediction with Conditional Graph Logic Network.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-4761)

   *Hanjun Dai, Chengtao Li, Connor Coley, Bo Dai, Le Song.*

1. **Learning the Graphical Structure of Electronic Health Records with Graph Convolutional Transformer.** AAAI 2020. [paper](https://arxiv.org/abs/1906.04716)

   *Edward Choi, Zhen Xu, Yujia Li, Michael W. Dusenberry, Gerardo Flores, Yuan Xue, Andrew M. Dai.*

### [Knowledge Graph](#content)

1. **Modeling Relational Data with Graph Convolutional Networks.** ESWC 2018. [paper](https://arxiv.org/pdf/1703.06103.pdf)

   *Michael Schlichtkrull, Thomas N. Kipf, Peter Bloem, Rianne van den Berg, Ivan Titov, Max Welling.*

1. **Cross-lingual Knowledge Graph Alignment via Graph Convolutional Networks.** EMNLP 2018. [paper](http://www.aclweb.org/anthology/D18-1032)

   *Zhichun Wang, Qingsong Lv, Xiaohan Lan, Yu Zhang.*

1. **Representation learning for visual-relational knowledge graphs.** arxiv 2017. [paper](https://arxiv.org/pdf/1709.02314.pdf)

   *Daniel Oñoro-Rubio, Mathias Niepert, Alberto García-Durán, Roberto González, Roberto J. López-Sastre.*

1. **End-to-end Structure-Aware Convolutional Networks for Knowledge Base Completion.** AAAI 2019. [paper](https://arxiv.org/pdf/1811.04441.pdf)

   *Chao Shang, Yun Tang, Jing Huang, Jinbo Bi, Xiaodong He, Bowen Zhou.*

1. **Knowledge Transfer for Out-of-Knowledge-Base Entities : A Graph Neural Network Approach.** IJCAI 2017. [paper](https://arxiv.org/pdf/1706.05674.pdf)

   *Takuo Hamaguchi, Hidekazu Oiwa, Masashi Shimbo, Yuji Matsumoto.* 

1. **Logic Attention Based Neighborhood Aggregation for Inductive Knowledge Graph Embedding.** AAAI 2019. [paper](https://arxiv.org/pdf/1811.01399.pdf)

   *Peifeng Wang, Jialong Han, Chenliang Li, Rong Pan.*

1. **Dynamic Graph Generation Network: Generating Relational Knowledge from Diagrams.** CVPR 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Kim_Dynamic_Graph_Generation_CVPR_2018_paper.pdf)

   *Haoyu Wang, Defu Lian, Yong Ge.*

1. **Estimating Node Importance in Knowledge Graphs Using Graph Neural Networks.** KDD 2019. [paper](https://arxiv.org/pdf/1905.08865)

   *Namyong Park, Andrey Kan, Xin Luna Dong, Tong Zhao, Christos Faloutsos.*

1. **OAG: Toward Linking Large-scale Heterogeneous Entity Graphs.** KDD 2019. [paper](http://keg.cs.tsinghua.edu.cn/jietang/publications/KDD19-Zhang-et-al-Open_Academic_Graph.pdf)

   *Fanjin Zhang, Xiao Liu, Jie Tang, Yuxiao Dong, Peiran Yao, Jie Zhang, Xiaotao Gu, Yan Wang, Bin Shao, Rui Li, Kuansan Wang.*

1. **Learning Attention-based Embeddings for Relation Prediction in Knowledge Graphs.** ACL 2019. [paper](https://arxiv.org/pdf/1906.01195)

   *Deepak Nathani, Jatin Chauhan, Charu Sharma, Manohar Kaul.*

1. **Cross-lingual Knowledge Graph Alignment via Graph Matching Neural Network.** ACL 2019. [paper](https://128.84.21.199/pdf/1905.11605)

   *Kun Xu, Mo Yu, Yansong Feng, Yan Song, Zhiguo Wang, Dong Yu.*

1. **Multi-relational Poincaré Graph Embeddings.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-2511)

   *Ivana Balazevic, Carl Allen, Timothy Hospedales.*

1. **Dynamically Pruned Message Passing Networks for Large-scale Knowledge Graph Reasoning.** ICLR 2020. [paper](https://openreview.net/pdf?id=rkeuAhVKvB)

   *Xiaoran Xu, Wei Feng, Yunsheng Jiang, Xiaohui Xie, Zhiqing Sun, Zhi-Hong Deng.*

1. **Efficient Probabilistic Logic Reasoning with Graph Neural Networks.** ICLR 2020. [paper](https://openreview.net/pdf?id=rJg76kStwH)

   *Yuyu Zhang, Xinshi Chen, Yuan Yang, Arun Ramamurthy, Bo Li, Yuan Qi, Le Song.*

### [Recommender Systems](#content)

1. **Graph Convolutional Neural Networks for Web-Scale Recommender Systems.** KDD 2018. [paper](https://arxiv.org/abs/1806.01973)

   *Rex Ying, Ruining He, Kaifeng Chen, Pong Eksombatchai, William L. Hamilton, Jure Leskovec.*

1. **Geometric Matrix Completion with Recurrent Multi-Graph Neural Networks.** NIPS 2017. [paper](https://arxiv.org/abs/1704.06803)

   *Federico Monti, Michael M. Bronstein, Xavier Bresson.*

1. **Graph Convolutional Matrix Completion.** 2017. [paper](https://arxiv.org/abs/1706.02263)

   *Rianne van den Berg, Thomas N. Kipf, Max Welling.*

1. **STAR-GCN: Stacked and Reconstructed Graph Convolutional Networks for Recommender Systems.** IJCAI 2019. [paper](https://arxiv.org/pdf/1905.13129.pdf)

   *Jiani Zhang, Xingjian Shi, Shenglin Zhao, Irwin King.*

1. **Binarized Collaborative Filtering with Distilling Graph Convolutional Networks.** IJCAI 2019. [paper](https://arxiv.org/pdf/1906.01829.pdf)

   *Haoyu Wang, Defu Lian, Yong Ge.*

1. **Graph Contextualized Self-Attention Network for Session-based Recommendation.** IJCAI 2019. [paper](https://www.ijcai.org/proceedings/2019/0547.pdf)

   *Chengfeng Xu, Pengpeng Zhao, Yanchi Liu, Victor S. Sheng, Jiajie Xu, Fuzhen Zhuang, Junhua Fang, Xiaofang Zhou.*

1. **Session-based Recommendation with Graph Neural Networks.** AAAI 2019. [paper](https://arxiv.org/pdf/1811.00855.pdf)

   *Shu Wu, Yuyuan Tang, Yanqiao Zhu, Liang Wang, Xing Xie, Tieniu Tan.*

1. **Geometric Hawkes Processes with Graph Convolutional Recurrent Neural Networks.** AAAI 2019. [paper](https://jshang2.github.io/pubs/geo.pdf)

   *Jin Shang, Mingxuan Sun.*

1. **Knowledge-aware Graph Neural Networks with Label Smoothness Regularization for Recommender Systems.** KDD 2019. [paper](https://arxiv.org/pdf/1905.04413)

   *Hongwei Wang, Fuzheng Zhang, Mengdi Zhang, Jure Leskovec, Miao Zhao, Wenjie Li, Zhongyuan Wang.*

1. **Exact-K Recommendation via Maximal Clique Optimization.** KDD 2019. [paper](https://arxiv.org/pdf/1905.07089)

   *Yu Gong, Yu Zhu, Lu Duan, Qingwen Liu, Ziyu Guan, Fei Sun, Wenwu Ou, Kenny Q. Zhu.*

1. **KGAT: Knowledge Graph Attention Network for Recommendation.** KDD 2019. [paper](https://arxiv.org/pdf/1905.07854)

   *Xiang Wang, Xiangnan He, Yixin Cao, Meng Liu, Tat-Seng Chua.*

1. **Knowledge Graph Convolutional Networks for Recommender Systems.** WWW 2019. [paper](https://arxiv.org/pdf/1904.12575.pdf)

   *Hongwei Wang, Miao Zhao, Xing Xie, Wenjie Li, Minyi Guo.*

1. **Dual Graph Attention Networks for Deep Latent Representation of Multifaceted Social Effects in Recommender Systems.** WWW 2019. [paper](https://arxiv.org/pdf/1903.10433.pdf)

   *Qitian Wu, Hengrui Zhang, Xiaofeng Gao, Peng He, Paul Weng, Han Gao, Guihai Chen.*

1. **Graph Neural Networks for Social Recommendation.** WWW 2019. [paper](https://arxiv.org/pdf/1902.07243.pdf)

   *Wenqi Fan, Yao Ma, Qing Li, Yuan He, Eric Zhao, Jiliang Tang, Dawei Yin.*

1. **Memory Augmented Graph Neural Networks for Sequential Recommendation.** AAAI 2020. [paper](https://arxiv.org/abs/1912.11730)

   *Chen Ma, Liheng Ma, Yingxue Zhang, Jianing Sun, Xue Liu, Mark Coates.*

1. **Revisiting Graph based Collaborative Filtering: A Linear Residual Graph Convolutional Network Approach.** AAAI 2020. [paper](https://arxiv.org/abs/2001.10167)

   *Lei Chen, Le Wu, Richang Hong, Kun Zhang, Meng Wang.*

1. **Inductive Matrix Completion Based on Graph Neural Networks.** ICLR 2020. [paper](https://openreview.net/pdf?id=ByxxgCEYDS)

   *Muhan Zhang, Yixin Chen.*

### [Computer Vision](#content)

1. **Graph Neural Networks for Object Localization.** ECAI 2006. [paper](http://ebooks.iospress.nl/volumearticle/2775)

   *Gabriele Monfardini, Vincenzo Di Massa, Franco Scarselli, Marco Gori.*

1. **Learning Human-Object Interactions by Graph Parsing Neural Networks.** ECCV 2018. [paper](https://arxiv.org/pdf/1808.07962.pdf)

   *Siyuan Qi, Wenguan Wang, Baoxiong Jia, Jianbing Shen, Song-Chun Zhu.*

1. **Learning Conditioned Graph Structures for Interpretable Visual Question Answering.** NeurIPS 2018. [paper](https://arxiv.org/pdf/1806.07243)

   *Will Norcliffe-Brown, Efstathios Vafeias, Sarah Parisot.*

1. **Symbolic Graph Reasoning Meets Convolutions.** NeurIPS 2018. [paper](http://papers.nips.cc/paper/7456-symbolic-graph-reasoning-meets-convolutions.pdf)

   *Xiaodan Liang, Zhiting Hu, Hao Zhang, Liang Lin, Eric P. Xing.*

1. **Out of the Box: Reasoning with Graph Convolution Nets for Factual Visual Question Answering.** NeurIPS 2018. [paper](http://papers.nips.cc/paper/7531-out-of-the-box-reasoning-with-graph-convolution-nets-for-factual-visual-question-answering.pdf)

   *Medhini Narasimhan, Svetlana Lazebnik, Alexander Schwing.*

1. **Structural-RNN: Deep Learning on Spatio-Temporal Graphs.** CVPR 2016. [paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Jain_Structural-RNN_Deep_Learning_CVPR_2016_paper.pdf)

   *Ashesh Jain, Amir R. Zamir, Silvio Savarese, Ashutosh Saxena.*

1. **Relation Networks for Object Detection.** CVPR 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers_backup/Hu_Relation_Networks_for_CVPR_2018_paper.pdf)

   *Han Hu, Jiayuan Gu, Zheng Zhang, Jifeng Dai, Yichen Wei.*

1. **Learning Region features for Object Detection.** ECCV 2018. [paper](https://arxiv.org/pdf/1803.07066)

   *Jiayuan Gu, Han Hu, Liwei Wang, Yichen Wei, Jifeng Dai.*

1. **The More You Know: Using Knowledge Graphs for Image Classification.** CVPR 2017. [paper](https://arxiv.org/pdf/1612.04844.pdf)

   *Kenneth Marino, Ruslan Salakhutdinov, Abhinav Gupta.* 

1. **Understanding Kin Relationships in a Photo.** TMM 2012. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6151163)

   *Siyu Xia, Ming Shao, Jiebo Luo, Yun Fu.* 

1. **Graph-Structured Representations for Visual Question Answering.** CVPR 2017. [paper](https://arxiv.org/pdf/1609.05600.pdf)

   *Damien Teney, Lingqiao Liu, Anton van den Hengel.* 

1. **Spatial Temporal Graph Convolutional Networks for Skeleton-Based Action Recognition.** AAAI 2018. [paper](https://arxiv.org/pdf/1801.07455.pdf)

   *Sijie Yan, Yuanjun Xiong, Dahua Lin.* 

1. **Dynamic Graph CNN for Learning on Point Clouds.** CVPR 2018. [paper](https://arxiv.org/pdf/1801.07829.pdf)

   *Yue Wang, Yongbin Sun, Ziwei Liu, Sanjay E. Sarma, Michael M. Bronstein, Justin M. Solomon.* 

1. **PointNet: Deep Learning on Point Sets for 3D Classification and Segmentation.** CVPR 2018. [paper](https://arxiv.org/pdf/1612.00593.pdf)

   *Charles R. Qi, Hao Su, Kaichun Mo, Leonidas J. Guibas.* 

1. **3D Graph Neural Networks for RGBD Semantic Segmentation.** CVPR 2017. [paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Qi_3D_Graph_Neural_ICCV_2017_paper.pdf)

   *Xiaojuan Qi, Renjie Liao, Jiaya Jia, Sanja Fidler, Raquel Urtasun.* 

1. **Iterative Visual Reasoning Beyond Convolutions.** CVPR 2018. [paper](https://arxiv.org/pdf/1803.11189)

   *Xinlei Chen, Li-Jia Li, Li Fei-Fei, Abhinav Gupta.* 

1. **Dynamic Edge-Conditioned Filters in Convolutional Neural Networks on Graphs.** CVPR 2017. [paper](https://arxiv.org/pdf/1704.02901)

   *Martin Simonovsky, Nikos Komodakis.* 

1. **Situation Recognition with Graph Neural Networks.** ICCV 2017. [paper](https://arxiv.org/pdf/1708.04320)

   *Ruiyu Li, Makarand Tapaswi, Renjie Liao, Jiaya Jia, Raquel Urtasun, Sanja Fidler.* 

1. **Deep Reasoning with Knowledge Graph for Social Relationship Understanding.** IJCAI 2018. [paper](https://arxiv.org/pdf/1807.00504.pdf)

   *Zhouxia Wang, Tianshui Chen, Jimmy Ren, Weihao Yu, Hui Cheng, Liang Lin.* 

1. **I Know the Relationships: Zero-Shot Action Recognition via Two-Stream Graph Convolutional Networks and Knowledge Graphs.** AAAI 2019. [paper](http://nlpr-web.ia.ac.cn/mmc/homepage/jygao/JY_Gao_files/Conference_Papers/AAAI2019-GJY.pdf)

   *Junyu Gao, Tianzhu Zhang, Changsheng Xu.*

<details><summary>more</summary>



21. **Graph CNNs with Motif and Variable Temporal Block for Skeleton-based Action Recognition.** AAAI 2019. [paper](https://ecs.victoria.ac.nz/foswiki/pub/Groups/Graphics/RGB-DDataProcessingForRobotics/Graph%20CNNs%20with%20Motif%20and%20Variable%20Temporal%20Block%20for%20Skeleton-based%20Action%20Recognition.pdf)

    *Yu-Hui Wen, Lin Gao, Hongbo Fu, Fang-Lue Zhang, Shihong Xia.*

22. **Multi-Label Image Recognition with Graph Convolutional Networks.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.03582.pdf)

    *Zhao-Min Chen, Xiu-Shen Wei, Peng Wang, Yanwen Guo.*

23. **Spatial-Aware Graph Relation Network for Large-Scale Object Detection.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Xu_Spatial-Aware_Graph_Relation_Network_for_Large-Scale_Object_Detection_CVPR_2019_paper.pdf)

    *Hang Xu, Chenhan Jiang, Xiaodan Liang, Zhenguo Li.*

24. **GCAN: Graph Convolutional Adversarial Network for Unsupervised Domain Adaptation.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Ma_GCAN_Graph_Convolutional_Adversarial_Network_for_Unsupervised_Domain_Adaptation_CVPR_2019_paper.pdf)

    *Xinhong Ma, Tianzhu Zhang, Changsheng Xu.*

25. **Mind Your Neighbours: Image Annotation With Metadata Neighbourhood Graph Co-Attention Networks.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Mind_Your_Neighbours_Image_Annotation_With_Metadata_Neighbourhood_Graph_Co-Attention_CVPR_2019_paper.pdf)

    *Junjie Zhang, Qi Wu, Jian Zhang, Chunhua Shen, Jianfeng Lu.*

26. **Attentive Relational Networks for Mapping Images to Scene Graphs.** CVPR 2019. [paper](https://arxiv.org/pdf/1811.10696.pdf)

    *Mengshi Qi, Weijian Li, Zhengyuan Yang, Yunhong Wang, Jiebo Luo.*

27. **Knowledge-Embedded Routing Network for Scene Graph Generation.** CVPR 2019. [paper](https://arxiv.org/pdf/1903.03326.pdf)

    *Tianshui Chen, Weihao Yu, Riquan Chen, Liang Lin.*

28. **Auto-Encoding Scene Graphs for Image Captioning.** CVPR 2019. [paper](https://arxiv.org/pdf/1812.02378.pdf)

    *Xu Yang, Kaihua Tang, Hanwang Zhang, Jianfei Cai.*

29. **Learning to Cluster Faces on an Affinity Graph.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.02749.pdf)

    *Lei Yang, Xiaohang Zhan, Dapeng Chen, Junjie Yan, Chen Change Loy, Dahua Lin.*

30. **Learning a Deep ConvNet for Multi-label Classification with Partial Labels.** CVPR 2019. [paper](https://arxiv.org/pdf/1902.09720.pdf)

    *Thibaut Durand, Nazanin Mehrasa, Greg Mori.*

31. **Graph Convolutional Label Noise Cleaner: Train a Plug-and-play Action Classifier for Anomaly Detection.** CVPR 2019. [paper](https://arxiv.org/pdf/1903.07256.pdf)

    *Jia-Xing Zhong, Nannan Li, Weijie Kong, Shan Liu, Thomas H. Li, Ge Li.*

32. **Learning Actor Relation Graphs for Group Activity Recognition.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.10117.pdf)

    *Jianchao Wu, Limin Wang, Li Wang, Jie Guo, Gangshan Wu.*

33. **ABC: A Big CAD Model Dataset For Geometric Deep Learning.** CVPR 2019. [paper](https://arxiv.org/pdf/1812.06216.pdf)

    *Sebastian Koch, Albert Matveev, Zhongshi Jiang, Francis Williams, Alexey Artemov, Evgeny Burnaev, Marc Alexa, Denis Zorin, Daniele Panozzo.*

34. **Neighbourhood Watch: Referring Expression Comprehension via Language-guided Graph Attention Networks.** CVPR 2019. [paper](https://arxiv.org/pdf/1812.04794.pdf)

    *Peng Wang, Qi Wu, Jiewei Cao, Chunhua Shen, Lianli Gao, Anton van den Hengel.*

35. **Graph-Based Global Reasoning Networks.** CVPR 2019. [paper](https://arxiv.org/pdf/1811.12814.pdf)

    *Yunpeng Chen, Marcus Rohrbach, Zhicheng Yan, Shuicheng Yan, Jiashi Feng, Yannis Kalantidis.*

36. **Linkage Based Face Clustering via Graph Convolution Network.** CVPR 2019. [paper](https://arxiv.org/pdf/1903.11306.pdf)

    *Zhongdao Wang, Liang Zheng, Yali Li, Shengjin Wang.*

37. **Fast Interactive Object Annotation with Curve-GCN.** CVPR 2019. [paper](https://arxiv.org/pdf/1903.06874.pdf)

    *Huan Ling, Jun Gao, Amlan Kar, Wenzheng Chen, Sanja Fidler.*

38. **Semantic Graph Convolutional Networks for 3D Human Pose Regression.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.03345.pdf)

    *Long Zhao, Xi Peng, Yu Tian, Mubbasir Kapadia, Dimitris N. Metaxas.*

39. **Neural Task Graphs: Generalizing to Unseen Tasks from a Single Video Demonstration.** CVPR 2019. [paper](https://arxiv.org/pdf/1807.03480.pdf)

    *De-An Huang, Suraj Nair, Danfei Xu, Yuke Zhu, Animesh Garg, Li Fei-Fei, Silvio Savarese, Juan Carlos Niebles.*

40. **Graphonomy: Universal Human Parsing via Graph Transfer Learning.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.04536.pdf)

    *Ke Gong, Yiming Gao, Xiaodan Liang, Xiaohui Shen, Meng Wang, Liang Lin.*

41. **Learning Context Graph for Person Search.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.01830.pdf)

    *Yichao Yan, Qiang Zhang, Bingbing Ni, Wendong Zhang, Minghao Xu, Xiaokang Yang.*

42. **Occlusion-Net: 2D/3D Occluded Keypoint Localization Using Graph Networks.** CVPR 2019. [paper](http://www.cs.cmu.edu/~mvo/index_files/Papers/ONet_19.pdf)

    *N. Dinesh Reddy, Minh Vo, Srinivasa G. Narasimhan.*

43. **MAN: Moment Alignment Network for Natural Language Moment Retrieval via Iterative Graph Adjustment.** CVPR 2019. [paper](https://arxiv.org/pdf/1812.00087.pdf)

    *Da Zhang, Xiyang Dai, Xin Wang, Yuan-Fang Wang, Larry S. Davis.*

44. **Context-Aware Visual Compatibility Prediction.** CVPR 2019. [paper](https://arxiv.org/pdf/1902.03646.pdf)

    *Guillem Cucurull, Perouz Taslakian, David Vazquez.*

45. **Graph Attention Convolution for Point Cloud Semantic Segmentation.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wang_Graph_Attention_Convolution_for_Point_Cloud_Semantic_Segmentation_CVPR_2019_paper.pdf)

    *Lei Wang, Yuchun Huang, Yaolin Hou, Shenman Zhang, Jie Shan.*

46. **An Attention Enhanced Graph Convolutional LSTM Network for Skeleton-Based Action Recognition.** CVPR 2019. [paper](https://arxiv.org/pdf/1902.09130.pdf)

    *Chenyang Si, Wentao Chen, Wei Wang, Liang Wang, Tieniu Tan.*

47. **Actional-Structural Graph Convolutional Networks for Skeleton-based Action Recognition.** CVPR 2019. [paper](https://arxiv.org/pdf/1904.12659.pdf)

    *Maosen Li, Siheng Chen, Xu Chen, Ya Zhang, Yanfeng Wang, Qi Tian.*

48. **Graph Convolutional Tracking.** CVPR 2019. [paper](http://nlpr-web.ia.ac.cn/mmc/homepage/jygao/JY_Gao_files/Conference_Papers/GCT-CVPR2019-GJY.pdf)

    *Junyu Gao, Tianzhu Zhang, Changsheng Xu.*

49. **Two-Stream Adaptive Graph Convolutional Networks for Skeleton-Based Action Recognition.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Shi_Two-Stream_Adaptive_Graph_Convolutional_Networks_for_Skeleton-Based_Action_Recognition_CVPR_2019_paper.pdf)

    *Lei Shi, Yifan Zhang, Jian Cheng, Hanqing Lu.*

50. **Skeleton-Based Action Recognition With Directed Graph Neural Networks.** CVPR 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Shi_Skeleton-Based_Action_Recognition_With_Directed_Graph_Neural_Networks_CVPR_2019_paper.pdf)

    *Lei Shi, Yifan Zhang, Jian Cheng, Hanqing Lu.*

51. **Neural Module Networks.** CVPR 2016. [paper](https://arxiv.org/pdf/1511.02799.pdf)

    *Jacob Andreas, Marcus Rohrbach, Trevor Darrell, Dan Klein.*

52. **LatentGNN: Learning Efficient Non-local Relations for Visual Recognition.** ICML 2019. [paper](https://arxiv.org/pdf/1905.11634)

    *Songyang Zhang, Shipeng Yan, Xuming He.*

53. **Graph Convolutional Gaussian Processes.** ICML 2019. [paper](https://arxiv.org/pdf/1905.05739)

    *Ian Walker, Ben Glocker.*

54. **GEOMetrics: Exploiting Geometric Structure for Graph-Encoded Objects.** ICML 2019. [paper](https://arxiv.org/pdf/1901.11461)

    *Edward J. Smith, Scott Fujimoto, Adriana Romero, David Meger.*

55. **Learning Cross­‐modal Context Graph Networks for Visual Grounding.** AAAI 2020. [paper](https://arxiv.org/abs/1911.09042)

    *Yongfei Liu, Bo Wan, Xiaodan Zhu, Xuming He.*

56. **Zero­‐Shot Sketch-based Image Retrieval via Graph Convolution Network.** AAAI 2020. [paper]()

    *Zhaolong Zhang, Yuejie Zhang, Rui Feng, Tao Zhang, Weiguo Fan.*

57. **Hybrid Graph Neural Networks for Crowd Counting.** AAAI 2020. [paper](https://arxiv.org/pdf/2002.00092)

    *Ao Luo, Fan Yang, Xin Li, Dong Nie, Zhicheng Jiao, Shangchen Zhou, Hong Cheng.*

58. **Learning Graph Convolutional Network for Skeleton-­‐based Human Action Recognition by Neural Searching.** AAAI 2020. [paper](https://arxiv.org/abs/1911.04131)

    *Wei Peng, Xiaopeng Hong, Haoyu Chen, Guoying Zhao.*

59. **STEP: Spatial Temporal Graph Convolutional Networks for Emotion Perception from Gaits.** AAAI 2020. [paper](https://arxiv.org/abs/1910.12906)

    *Uttaran Bhattacharya, Trisha Mittal, Rohan Chandra, Tanmay Randhavane, Aniket Bera, Dinesh Manocha.*

60. **Relation‐Aware Pedestrian Attribute Recognition with Graph Convolutional Networks.** AAAI 2020. [paper]()

    *Zichang Tan, Yang Yang, Jun Wan, Stan Li.*

61. **Deep Generative Probabilistic Graph Neural Networks for Scene Graph Generation.** AAAI 2020. [paper](https://grlearning.github.io/papers/135.pdf)

    *Mahmoud Khademi, Oliver Schulte.*

62. **Zero-­‐shot Ingredient Recognition by Multi-­‐Relational Graph Convolutional Network.** AAAI 2020. [paper](http://www.liangmingpan.com/files/publications/AAAI20_Paper.pdf)

    *Jingjing Chen, Liang-Ming Pan, Zhi-Peng Wei, Xiang Wang, Chong-Wah Ngo,Tat-Seng Chua.*

63. **Location-aware Graph Convolutional Networks for Video Question Answering.** AAAI 2020. [paper]()

    *Deng Huang, Peihao Chen, Runhao Zeng, Qing Du, Mingkui Tan, Chuang Gan.*

64. **Facial Action Unit Intensity Estimation via Semantic Correspondence Learning with Dynamic Graph Convolution.** AAAI 2020. [paper]()

    *Fan Yingruo, Jacqueline C.K. Lam, Victor Li.*

65. **Reasoning with Heterogeneous Graph Alignment for Video Question Answering.** AAAI 2020. [paper]()

    *Pin Jiang, Yahong Han.*

66. **Multi-Label Classification with Label Graph Superimposing.** AAAI 2020. [paper](https://arxiv.org/abs/1911.09243)

    *Ya Wang, Dongliang He, Fu Li, Xiang Long, Zhichao Zhou, Jinwen Ma, Shilei Wen.*

67. **Part-Level Graph Convolutional Network for Skeleton-Based Action Recognition.** AAAI 2020. [paper]()

    *Linjiang Huang, Yan Huang, Wanli Ouyang, Liang Wang.*

68. **SOGNet: Scene Overlap Graph Network for Panoptic Segmentation.** AAAI 2020. [paper](https://arxiv.org/abs/1911.07527)

    *Yibo Yang, Hongyang Li, Xia Li, Qijie Zhao, Jianlong Wu, Zhouchen Lin.*

69. **Universal-RCNN: Universal Object Detector via Transferable Graph R-CNN.** AAAI 2020. [paper](https://arxiv.org/abs/2002.07417)

    *Hang Xu, Linpu Fang, Xiaodan Liang, Wenxiong Kang, Zhenguo Li.*

70. **Abstract Diagrammatic Reasoning with Multiplex Graph Networks.** ICLR 2020. [paper](https://openreview.net/pdf?id=ByxQB1BKwH)

    *Duo Wang, Mateja Jamnik, Pietro Lio.*

</details>

### [Natural Language Processing](#content)

1. **Conversation Modeling on Reddit using a Graph-Structured LSTM.** TACL 2018. [paper](https://arxiv.org/pdf/1704.02080)

   *Vicky Zayats, Mari Ostendorf.* 

1. **Learning Graphical State Transitions.** ICLR 2017. [paper](https://openreview.net/forum?id=HJ0NvFzxl)

   *Daniel D. Johnson.*

1. **Multiple Events Extraction via Attention-based Graph Information Aggregation.** EMNLP 2018. [paper](https://arxiv.org/pdf/1809.09078.pdf)

   *Xiao Liu, Zhunchen Luo, Heyan Huang.*

1. **Recurrent Relational Networks.** NeurIPS 2018. [paper](http://papers.nips.cc/paper/7597-recurrent-relational-networks.pdf)

   *Rasmus Palm, Ulrich Paquet, Ole Winther.*

1. **Improved Semantic Representations From Tree-Structured Long Short-Term Memory Networks.** ACL 2015. [paper](https://www.aclweb.org/anthology/P15-1150)

   *Kai Sheng Tai, Richard Socher, Christopher D. Manning.*

1. **Encoding Sentences with Graph Convolutional Networks for Semantic Role Labeling.** EMNLP 2017. [paper](https://arxiv.org/abs/1703.04826)

   *Diego Marcheggiani, Ivan Titov.*

1. **Graph Convolutional Networks with Argument-Aware Pooling for Event Detection.** AAAI 2018. [paper](http://ix.cs.uoregon.edu/~thien/pubs/graphConv.pdf)

   *Thien Huu Nguyen, Ralph Grishman.*

1. **Exploiting Semantics in Neural Machine Translation with Graph Convolutional Networks.** NAACL 2018. [paper](http://www.aclweb.org/anthology/N18-2078)

   *Diego Marcheggiani, Joost Bastings, Ivan Titov.*

1. **Exploring Graph-structured Passage Representation for Multi-hop Reading Comprehension with Graph Neural Networks.** 2018. [paper](https://arxiv.org/abs/1809.02040)

   *Linfeng Song, Zhiguo Wang, Mo Yu, Yue Zhang, Radu Florian, Daniel Gildea.*

1. **Graph Convolution over Pruned Dependency Trees Improves Relation Extraction.** EMNLP 2018. [paper](https://arxiv.org/abs/1809.10185)

   *Yuhao Zhang, Peng Qi, Christopher D. Manning.*

1. **N-ary relation extraction using graph state LSTM.** EMNLP 18. [paper](https://arxiv.org/abs/1808.09101)

   *Linfeng Song, Yue Zhang, Zhiguo Wang, Daniel Gildea.*

1. **A Graph-to-Sequence Model for AMR-to-Text Generation.** ACL 2018. [paper](https://arxiv.org/abs/1805.02473)

   *Linfeng Song, Yue Zhang, Zhiguo Wang, Daniel Gildea.*

1. **Graph-to-Sequence Learning using Gated Graph Neural Networks.** ACL 2018. [paper](https://arxiv.org/pdf/1806.09835.pdf)

   *Daniel Beck, Gholamreza Haffari, Trevor Cohn.*

1. **Cross-Sentence N-ary Relation Extraction with Graph LSTMs.** TACL. [paper](https://arxiv.org/abs/1708.03743)

   *Nanyun Peng, Hoifung Poon, Chris Quirk, Kristina Toutanova, Wen-tau Yih.*

1. **Sentence-State LSTM for Text Representation.** ACL 2018. [paper](https://arxiv.org/abs/1805.02474)

   *Yue Zhang, Qi Liu, Linfeng Song.*

1. **End-to-End Relation Extraction using LSTMs on Sequences and Tree Structures.** ACL 2016. [paper](https://arxiv.org/abs/1601.00770)

   *Makoto Miwa, Mohit Bansal.*

1. **Graph Convolutional Encoders for Syntax-aware Neural Machine Translation.** EMNLP 2017. [paper](https://arxiv.org/pdf/1704.04675)

   *Joost Bastings, Ivan Titov, Wilker Aziz, Diego Marcheggiani, Khalil Sima'an.* 

1. **Semi-supervised User Geolocation via Graph Convolutional Networks.** ACL 2018. [paper](https://arxiv.org/pdf/1804.08049.pdf)

   *Afshin Rahimi, Trevor Cohn, Timothy Baldwin.* 

1. **Modeling Semantics with Gated Graph Neural Networks for Knowledge Base Question Answering.** COLING 2018. [paper](https://arxiv.org/pdf/1808.04126.pdf)

   *Daniil Sorokin, Iryna Gurevych.* 

1. **Graph Convolutional Networks for Text Classification.** AAAI 2019. [paper](https://arxiv.org/pdf/1809.05679.pdf)

   *Liang Yao, Chengsheng Mao, Yuan Luo.* 

<details><summary>more</summary>



21. **Constructing Narrative Event Evolutionary Graph for Script Event Prediction.** IJCAI 2018. [paper](https://arxiv.org/pdf/1805.05081.pdf)

    *Zhongyang Li, Xiao Ding, Ting Liu.* 

22. **Incorporating Syntactic and Semantic Information in Word Embeddings using Graph Convolutional Networks.** ACL 2019. [paper](https://arxiv.org/pdf/1809.04283)

    *Shikhar Vashishth, Manik Bhandari, Prateek Yadav, Piyush Rai, Chiranjib Bhattacharyya, Partha Talukdar*

23. **PaperRobot: Incremental Draft Generation of Scientific Ideas.** ACL 2019. [paper](https://arxiv.org/pdf/1905.07870)

    *Qingyun Wang, Lifu Huang, Zhiying Jiang, Kevin Knight, Heng Ji, Mohit Bansal, Yi Luan.*

24. **Inter-sentence Relation Extraction with Document-level Graph Convolutional Neural Network.** ACL 2019. [paper](https://arxiv.org/pdf/1906.04684)

    *Sunil Kumar Sahu, Fenia Christopoulou, Makoto Miwa, Sophia Ananiadou.*

25. **Textbook Question Answering with Multi-modal Context Graph Understanding and Self-supervised Open-set Comprehension.** ACL 2019. [paper](https://arxiv.org/pdf/1811.00232)

    *Daesik Kim, Seonhoon Kim, Nojun Kwak.*

26. **Multi-hop Reading Comprehension across Multiple Documents by Reasoning over Heterogeneous Graphs.** ACL 2019. [paper](https://arxiv.org/pdf/1905.07374)

    *Ming Tu, Guangtao Wang, Jing Huang, Yun Tang, Xiaodong He, Bowen Zhou.*

27. **Dynamically Fused Graph Network for Multi-hop Reasoning.** ACL 2019. [paper](https://arxiv.org/pdf/1905.06933)

    *Yunxuan Xiao, Yanru Qu, Lin Qiu, Hao Zhou, Lei Li, Weinan Zhang, Yong Yu.*

28. **Cognitive Graph for Multi-Hop Reading Comprehension at Scale.** ACL 2019. [paper](https://arxiv.org/pdf/1905.05460)

    *Ming Ding, Chang Zhou, Qibin Chen, Hongxia Yang, Jie Tang.*

29. **Joint Type Inference on Entities and Relations via Graph Convolutional Networks.** ACL 2019. [paper](http://www.czsun.site/publications/joint_entrel_gcn.pdf)

    *Changzhi Sun, Yeyun Gong, Yuanbin Wu, Ming Gong, Daxing Jiang, Man Lan, Shiliang Sun1, Nan Duan.*

30. **Attention Guided Graph Convolutional Networks for Relation Extraction.** ACL 2019. [paper](http://www.statnlp.org/wp-content/uploads/2019/06/Attention_Guided_Graph_Convolutional_Networks_for_Relation_Extraction.pdf)

    *Zhijiang Guo, Yan Zhang, Wei Lu.*

31. **GraphRel: Modeling Text as Relational Graphs for Joint Entity and Relation Extraction.** ACL 2019. [paper](https://tsujuifu.github.io/pubs/acl19_graph-rel.pdf)

    *Tsu-Jui Fu, Peng-Hsuan Li, Wei-Yun Ma.*

32. **Graph Neural Networks with Generated Parameters for Relation Extraction.** ACL 2019. [paper](https://arxiv.org/pdf/1902.00756)

    *Hao Zhu, Yankai Lin, Zhiyuan Liu, Jie Fu, Tat-seng Chua, Maosong Sun.*

33. **Generating Logical Forms from Graph Representations of Text and Entities.** ACL 2019. [paper](https://arxiv.org/pdf/1905.08407)

    *Peter Shaw, Philip Massey, Angelica Chen, Francesco Piccinno, Yasemin Altun.*

34. **Matching Article Pairs with Graphical Decomposition and Convolutions.** ACL 2019. [paper](https://arxiv.org/pdf/1802.07459)

    *Bang Liu, Di Niu, Haojie Wei, Jinghong Lin, Yancheng He, Kunfeng Lai, Yu Xu.*

35. **Representing Schema Structure with Graph Neural Networks for Text-to-SQL Parsing.** ACL 2019. [paper](https://arxiv.org/pdf/1905.06241)

    *Ben Bogin, Matt Gardner, Jonathan Berant.*

36. **Coherent Comment Generation for Chinese Articles with a Graph-to-Sequence Model.** ACL 2019. [paper](https://arxiv.org/pdf/1906.01231)

    *Wei Li, Jingjing Xu, Yancheng He, Shengli Yan, Yunfang Wu, Xu sun.*

37. **GEAR: Graph-based Evidence Aggregating and Reasoning for Fact Verification.** ACL 2019. [paper](https://www.aclweb.org/anthology/P19-1085)

    *Jie Zhou, Xu Han, Cheng Yang, Zhiyuan Liu, Lifeng Wang, Changcheng Li, Maosong Sun.*

38. **Look Again at the Syntax: Relational Graph Convolutional Network for Gendered Ambiguous Pronoun Resolution.** ACL 2019. [paper](https://arxiv.org/pdf/1905.08868.pdf)

    *Yinchuan Xu, Junlin Yang.*

39. **Structured Neural Summarization.** ICLR 2019. [paper](https://openreview.net/pdf?id=H1ersoRqtm)

    *Patrick Fernandes, Miltiadis Allamanis, Marc Brockschmidt.*

40. **Long-tail Relation Extraction via Knowledge Graph Embeddings and Graph Convolution Networks.** NAACL 2019. [paper](https://arxiv.org/pdf/1903.01306.pdf)

    *Ningyu Zhang, Shumin Deng, Zhanlin Sun, Guanying Wang, Xi Chen, Wei Zhang, Huajun Chen.*

41. **Text Generation from Knowledge Graphs with Graph Transformers.** NAACL 2019. [paper](https://arxiv.org/pdf/1904.02342.pdf)

    *Rik Koncel-Kedziorski, Dhanush Bekal, Yi Luan, Mirella Lapata, Hannaneh Hajishirzi.*

42. **Question Answering by Reasoning Across Documents with Graph Convolutional Networks.** NAACL 2019. [paper](https://arxiv.org/pdf/1808.09920.pdf)

    *Nicola De Cao, Wilker Aziz, Ivan Titov.*

43. **BAG: Bi-directional Attention Entity Graph Convolutional Network for Multi-hop Reasoning Question Answering.** NAACL 2019. [paper](https://arxiv.org/pdf/1904.04969.pdf)

    *Yu Cao, Meng Fang, Dacheng Tao.*

44. **GraphIE: A Graph-Based Framework for Information Extraction.** NAACL 2019. [paper](https://arxiv.org/pdf/1810.13083.pdf)

    *Yujie Qian, Enrico Santus, Zhijing Jin, Jiang Guo, Regina Barzilay.*

45. **Graph Convolution for Multimodal Information Extraction from Visually Rich Documents.** NAACL 2019. [paper](https://arxiv.org/pdf/1903.11279.pdf)

    *Xiaojing Liu, Feiyu Gao, Qiong Zhang, Huasha Zhao.*

46. **Structural Neural Encoders for AMR-to-text Generation.** NAACL 2019. [paper](https://arxiv.org/pdf/1903.11410.pdf)

    *Marco Damonte, Shay B. Cohen.*

47. **Abusive Language Detection with Graph Convolutional Networks.** NAACL 2019. [paper](https://arxiv.org/pdf/1904.04073.pdf)

    *Pushkar Mishra, Marco Del Tredici, Helen Yannakoudakis, Ekaterina Shutova.*

48. **Learning Graph Pooling and Hybrid Convolutional Operations for Text Representations.** WWW 2019. [paper](https://arxiv.org/pdf/1901.06965.pdf)

    *Hongyang Gao, Yongjun Chen, Shuiwang Ji.*

49. **Graph­‐based Transformer with Cross-candidate Verification for Semantic Parsing.** AAAI 2020. [paper]()

    *Bo Shao, Yeyun Gong, Weizhen Qi, Guihong Cao, Jianshu Ji, Xiaola Lin.*

50. **Efficient Multi-Person Pose Estimation with Provable Guarantees.** AAAI 2020. [paper](https://arxiv.org/abs/1711.07794)

    *Shaofei Wang, Konrad Paul Kording, Julian Yarkony.*

51. **Graph Transformer for Graph-to-Sequence Learning.** AAAI 2020. [paper](https://arxiv.org/abs/1911.07470)

    *Deng Cai, Wai Lam.*

52. **Multi-­‐label Patent Categorization with Non-­‐local Attention-­‐based Graph Convolutional Network.** AAAI 2020. [paper]()

    *Pingjie Tang, Meng Jiang, Bryan (Ning) Xia, Jed Pitera, Jeff Welser, Nitesh Chawla.*

53. **Multi-task Learning for Metaphor Detection with Graph Convolutional Neural Networks and Word Sense Disambiguation.** AAAI 2020. [paper]()

    *Duong Minh Le, My Thai and Thien Huu Nguyen.*

54. **Schema-Guided Multi-Domain Dialogue State Tracking with Graph Attention Neural Networks.** AAAI 2020. [paper]()

    *Lu Chen, Boer Lv, Chi Wang, Su Zhu, Bowen Tan, Kai Yu.*

55. **GraphER: Token-Centric Entity Resolution with Graph Convolutional Neural Networks.** AAAI 2020. [paper]()

    *Bing Li, Wei Wang, Yifang Sun, Linhan Zhang, Muhammad Asif Ali, Yi Wang.*

56. **CFGNN:Cross Flow Graph Neural Networks for Question Answering on Complex Tables.** AAAI 2020. [paper]()

    *Xuanyu Zhang.*
    </details>

### [Generation](#content)

1. **Graph Convolutional Policy Network for Goal-Directed Molecular Graph Generation.** NeurIPS 2018. [paper](https://arxiv.org/pdf/1806.02473)

   *Jiaxuan You, Bowen Liu, Rex Ying, Vijay Pande, Jure Leskovec.*

1. **Constrained Generation of Semantically Valid Graphs via Regularizing Variational Autoencoders.** NeurIPS 2018. [paper](https://papers.nips.cc/paper/7942-constrained-generation-of-semantically-valid-graphs-via-regularizing-variational-autoencoders.pdf)

   *Tengfei Ma, Jie Chen, Cao Xiao.*

1. **Learning deep generative models of graphs.** ICLR Workshop 2018. [paper](https://arxiv.org/abs/1803.03324)

   *Yujia Li, Oriol Vinyals, Chris Dyer, Razvan Pascanu, Peter Battaglia.*

1. **MolGAN: An implicit generative model for small molecular graphs.** 2018. [paper](https://arxiv.org/abs/1805.11973)

   *Nicola De Cao, Thomas Kipf.*

1. **GraphRNN: Generating Realistic Graphs with Deep Auto-regressive Models.** ICML 2018. [paper](https://arxiv.org/abs/1802.08773)

   *Jiaxuan You, Rex Ying, Xiang Ren, William L. Hamilton, Jure Leskovec.*

1. **NetGAN: Generating Graphs via Random Walks.** ICML 2018. [paper](https://arxiv.org/abs/1803.00816)

   *Aleksandar Bojchevski, Oleksandr Shchur, Daniel Zügner, Stephan Günnemann.*

1. **Graphite: Iterative Generative Modeling of Graphs.** ICML 2019. [paper](https://arxiv.org/pdf/1803.10459)

   *Aditya Grover, Aaron Zweig, Stefano Ermon.*

1. **Generative Code Modeling with Graphs.** ICLR 2019. [paper](https://openreview.net/pdf?id=Bke4KsA5FX)

   *Marc Brockschmidt, Miltiadis Allamanis, Alexander L. Gaunt, Oleksandr Polozov.*

1. **Efficient Graph Generation with Graph Recurrent Attention Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-2394)

   *Renjie Liao, Yujia Li, Yang Song, Shenlong Wang, Will Hamilton, David Duvenaud, Raquel Urtasun, Richard Zemel.*

1. **Graph Normalizing Flows.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-7511)

   *Jenny Liu, Aviral Kumar, Jimmy Ba, Jamie Kiros, Kevin Swersky.*

1. **Conditional Structure Generation through Graph Variational Generative Adversarial Nets.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-772)

   *Carl Yang, Peiye Zhuang, Wenhan Shi, Alan Luu, Pan Li.*

1. **GraphAF: a Flow-based Autoregressive Model for Molecular Graph Generation.** ICLR 2020. [paper](https://openreview.net/pdf?id=S1esMkHYPr)

   *Chence Shi, Minkai Xu, Zhaocheng Zhu, Weinan Zhang, Ming Zhang, Jian Tang.*

### [Combinatorial Optimization](#content)

1. **Combinatorial Optimization with Graph Convolutional Networks and Guided Tree Search.** NeurIPS 2018. [paper](http://papers.nips.cc/paper/7335-combinatorial-optimization-with-graph-convolutional-networks-and-guided-tree-search.pdf)

   *Zhuwen Li, Qifeng Chen, Vladlen Koltun.*

1. **Learning a SAT Solver from Single-Bit Supervision.** ICLR 2019. [paper](https://arxiv.org/abs/1802.03685)

   *Daniel Selsam, Matthew Lamm, Benedikt Bünz, Percy Liang, Leonardo de Moura, David L. Dill.*

1. **A Note on Learning Algorithms for Quadratic Assignment with Graph Neural Networks.** PADL 2017. [paper](https://www.padl.ws/papers/Paper%2017.pdf)

   *Alex Nowak, Soledad Villar, Afonso S. Bandeira, Joan Bruna.*

1. **Attention Solves Your TSP, Approximately.** 2018. [paper](https://arxiv.org/abs/1803.08475)

   *Wouter Kool, Herke van Hoof, Max Welling.*

1. **Learning to Solve NP-Complete Problems - A Graph Neural Network for Decision TSP.** AAAI 2019. [paper](https://arxiv.org/pdf/1809.02721.pdf)

   *Marcelo O. R. Prates, Pedro H. C. Avelar, Henrique Lemos, Luis Lamb, Moshe Vardi.*

1. **DAG-GNN: DAG Structure Learning with Graph Neural Networks.** ICML 2019. [paper](https://arxiv.org/pdf/1904.10098)

   *Yue Yu, Jie Chen, Tian Gao, Mo Yu.*

1. **Exact Combinatorial Optimization with Graph Convolutional Neural Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-9029)

   *Maxime Gasse, Didier Chetelat, Nicola Ferroni, Laurent Charlin, Andrea Lodi.*

1. **Approximation Ratios of Graph Neural Networks for Combinatorial Problems.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-2252)

   *Ryoma Sato, Makoto Yamada, Hisashi Kashima.*

### [Adversarial Attack](#content)

1. **Adversarial Attacks on Neural Networks for Graph Data.** KDD 2018. [paper](http://delivery.acm.org/10.1145/3230000/3220078/p2847-zugner.pdf?ip=101.5.139.169&id=3220078&acc=ACTIVE%20SERVICE&key=BF85BBA5741FDC6E%2E587F3204F5B62A59%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1545706391_e7484be677293ffb5f18b39ce84a0df9)

   *Daniel Zügner, Amir Akbarnejad, Stephan Günnemann.*

1. **Adversarial Attack on Graph Structured Data.** ICML 2018. [paper](https://arxiv.org/abs/1806.02371)

   *Hanjun Dai, Hui Li, Tian Tian, Xin Huang, Lin Wang, Jun Zhu, Le Song.*

1. **Adversarial Examples on Graph Data: Deep Insights into Attack and Defense.** IJCAI 2019. [paper](https://arxiv.org/pdf/1903.01610.pdf)

   *Huijun Wu, Chen Wang, Yuriy Tyshetskiy, Andrew Docherty, Kai Lu, Liming Zhu.*

1. **Topology Attack and Defense for Graph Neural Networks: An Optimization Perspective.** IJCAI 2019. [paper](https://arxiv.org/pdf/1906.04214.pdf)

   *Kaidi Xu, Hongge Chen, Sijia Liu, Pin-Yu Chen, Tsui-Wei Weng, Mingyi Hong, Xue Lin.*

1. **Robust Graph Convolutional Networks Against Adversarial Attacks.** KDD 2019. [paper](http://pengcui.thumedialab.com/papers/RGCN.pdf)

   *Dingyuan Zhu, Ziwei Zhang, Peng Cui, Wenwu Zhu.*

1. **Certifiable Robustness and Robust Training for Graph Convolutional Networks.** KDD 2019. [paper](https://arxiv.org/pdf/1906.12269)

   *Daniel Zügner, Stephan Günnemann.*

1. **Adversarial Attacks on Node Embeddings via Graph Poisoning.** ICML 2019. [paper](https://arxiv.org/pdf/1809.01093)

   *Aleksandar Bojchevski, Stephan Günnemann.*

1. **Adversarial Attacks on Graph Neural Networks via Meta Learning.** ICLR 2019. [paper]()

   *Daniel Zügner, Stephan Günnemann.*

1. **PeerNets: Exploiting Peer Wisdom Against Adversarial Attacks.** ICLR 2019. [paper](https://openreview.net/pdf?id=Sk4jFoA9K7)

   *Jan Svoboda, Jonathan Masci, Federico Monti, Michael Bronstein, Leonidas Guibas.*

1. **Certifiable Robustness to Graph Perturbations.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-4514)

   *Aleksandar Bojchevski, Stephan Günnemann.*

1. **A Unified Framework for Data Poisoning Attack to Graph-based Semi-supervised Learning.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-5182)

   *Xuanqing Liu, Si Si, Jerry Zhu, Yang Li, Cho-Jui Hsieh.*

1. **GNNGuard: Defending Graph Neural Networks against Adversarial Attacks.** NeurIPS 2020. [paper](https://papers.nips.cc/paper/2020/hash/690d83983a63aa1818423fd6edd3bfdb-Abstract.html)

   *Xiang Zhang, Marinka Zitnik.*

### [Graph Clustering](#content)

1. **Attributed Graph Clustering: A Deep Attentional Embedding Approach.** IJCAI 2019. [paper](https://arxiv.org/pdf/1906.06532.pdf)

   *Chun Wang, Shirui Pan, Ruiqi Hu, Guodong Long, Jing Jiang, Chengqi Zhang.*

1. **Attributed Graph Clustering via Adaptive Graph Convolution.** IJCAI 2019. [paper](https://arxiv.org/pdf/1906.01210.pdf)

   *Xiaotong Zhang, Han Liu, Qimai Li, Xiao-Ming Wu.*

### [Graph Classification](#content)

1. **Contextual Graph Markov Model: A Deep and Generative Approach to Graph Processing.** ICML 2018. [paper](https://arxiv.org/pdf/1805.10636.pdf)

   *Davide Bacciu, Federico Errica, Alessio Micheli.*

1. **Semi-Supervised Graph Classification: A Hierarchical Graph Perspective.** WWW 2019. [paper](https://arxiv.org/pdf/1904.05003.pdf)

   *Jia Li, Yu Rong, Hong Cheng, Helen Meng, Wenbing Huang, Junzhou Huang.*

1. **DDGK: Learning Graph Representations for Deep Divergence Graph Kernels.** WWW 2019. [paper](https://arxiv.org/pdf/1904.09671.pdf)

   *Rami Al-Rfou, Dustin Zelle, Bryan Perozzi.*

1. **Unsupervised Inductive Graph-Level Representation Learning via Graph-Graph Proximity.** IJCAI 2019. [paper](https://arxiv.org/pdf/1904.01098.pdf)

   *Yunsheng Bai, Hao Ding, Yang Qiao, Agustin Marinovic, Ken Gu, Ting Chen, Yizhou Sun, Wei Wang.*

1. **Motif-matching based Subgraph-level Attentional Convolution Network for Graph Classification.** AAAI 2020. [paper]()

   *Hao Peng, Jianxin Li,  Qiran Gong, Yuanxing Ning, Senzhang Wang, Lifang He.*

1. **InfoGraph: Unsupervised and Semi-supervised Graph-Level Representation Learning via Mutual Information Maximization.** ICLR 2020. [paper](https://openreview.net/pdf?id=r1lfF2NYvH)

   *Fan-Yun Sun, Jordan Hoffman, Vikas Verma, Jian Tang.*

1. **A Fair Comparison of Graph Neural Networks for Graph Classification.** ICLR 2020. [paper](https://openreview.net/pdf?id=HygDF6NFPB)

   *Federico Errica, Marco Podda, Davide Bacciu, Alessio Micheli.*

### [Reinforcement Learning](#content)

1. **NerveNet: Learning Structured Policy with Graph Neural Networks.** ICLR 2018. [paper](https://openreview.net/pdf?id=S1sqHMZCb)

   *Tingwu Wang, Renjie Liao, Jimmy Ba, Sanja Fidler.* 

1. **Structured Dialogue Policy with Graph Neural Networks.** ICCL 2018. [paper](http://www.aclweb.org/anthology/C18-1107)

   *Lu Chen, Bowen Tan, Sishan Long, Kai Yu.* 

1. **Action Schema Networks: Generalised Policies with Deep Learning.** AAAI 2018. [paper](https://arxiv.org/abs/1709.04271)

   *Sam Toyer, Felipe Trevizan, Sylvie Thiébaux, Lexing Xie.*

1. **Relational inductive bias for physical construction in humans and machines.** CogSci 2018. [paper](https://arxiv.org/abs/1806.01203)

   *Jessica B. Hamrick, Kelsey R. Allen, Victor Bapst, Tina Zhu, Kevin R. McKee, Joshua B. Tenenbaum, Peter W. Battaglia.* 

1. **Relational Deep Reinforcement Learning.** arxiv 2018. [paper](https://arxiv.org/abs/1806.01830)

   *Vinicius Zambaldi, David Raposo, Adam Santoro, Victor Bapst, Yujia Li, Igor Babuschkin, Karl Tuyls, David Reichert, Timothy Lillicrap, Edward Lockhart, Murray Shanahan, Victoria Langston, Razvan Pascanu, Matthew Botvinick, Oriol Vinyals, Peter Battaglia.*

1. **Playing Text-Adventure Games with Graph-Based Deep Reinforcement Learning.** NAACL 2019. [paper](https://arxiv.org/pdf/1812.01628.pdf)

   *Prithviraj Ammanabrolu, Mark O. Riedl.*

1. **Learning Transferable Graph Exploration.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-1444)

   *Hanjun Dai, Yujia Li, Chenglong Wang, Rishabh Singh, Po-Sen Huang, Pushmeet Kohli.*

1. **Graph Neural Networks and Reinforcement Learning for Behavior Generation in Semantic Environments.** IV 2020. [paper](https://arxiv.org/abs/2006.12576)

   *Patrick Hart, Alois Knoll.*

1. **Multi-Agent Game Abstraction via Graph Attention Neural Network.** AAAI 2020. [paper](https://arxiv.org/abs/1911.10715)

   *Yong Liu, Weixun Wang, Yujing Hu, Jianye Hao, Xingguo Chen, Yang Gao.*

1. **Graph Convolutional Reinforcement Learning.** ICLR 2020. [paper](https://openreview.net/pdf?id=HkxdQkSYDB)

   *Jiechuan Jiang, Chen Dun, Tiejun Huang, Zongqing Lu.*

1. **Reinforcement Learning Based Graph-to-Sequence Model for Natural Question Generation.** ICLR 2020. [paper](https://openreview.net/pdf?id=HygnDhEtvr)

   *Yu Chen, Lingfei Wu, Mohammed J. Zaki.*

1. **Reinforced Genetic Algorithm Learning for Optimizing Computation Graphs.** ICLR 2020. [paper](https://openreview.net/pdf?id=rkxDoJBYPB)

   *Aditya Paliwal, Felix Gimeno, Vinod Nair, Yujia Li, Miles Lubin, Pushmeet Kohli, Oriol Vinyals.*

### [Traffic Network](#content)

1. **Spatiotemporal Multi‐Graph Convolution Network for Ride-hailing Demand Forecasting.** AAAI 2019. [paper](http://www-scf.usc.edu/~yaguang/papers/aaai19_multi_graph_convolution.pdf)

   *Xu Geng, Yaguang Li, Leye Wang, Lingyu Zhang, Qiang Yang, Jieping Ye, Yan Liu.*

1. **Attention Based Spatial-Temporal Graph Convolutional Networks for Traffic Flow Forecasting.** AAAI 2019. [paper](https://github.com/Davidham3/ASTGCN/blob/master/papers/2019%20AAAI_Attention%20Based%20Spatial-Temporal%20Graph%20Convolutional%20Networks%20for%20Traffic%20Flow%20Forecasting.pdf)

   *Shengnan Guo, Youfang Lin, Ning Feng, Chao Song, Huaiyu Wan.*

1. **Traffic Graph Convolutional Recurrent Neural Network: A Deep Learning Framework for Network-Scale Traffic Learning and Forecasting.** arxiv 2018. [paper](https://arxiv.org/pdf/1802.07007.pdf)

   *Zhiyong Cui, Kristian Henrickson, Ruimin Ke, Yinhai Wang.* 

1. **Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting.** IJCAI 2018. [paper](https://arxiv.org/pdf/1709.04875.pdf)

   *Bing Yu, Haoteng Yin, Zhanxing Zhu.* 

1. **Origin-Destination Matrix Prediction via Graph Convolution: a New Perspective of Passenger Demand Modeling.** KDD 2019. [paper](https://www.dropbox.com/s/erz0b9c13aeoelj/KDD19-Yuandong.pdf?dl=0)

   *Yuandong Wang, Hongzhi Yin, Hongxu Chen, Tianyu Wo, Jie Xu, Kai Zheng.*

1. **Predicting Path Failure In Time-Evolving Graphs.** KDD 2019. [paper](https://arxiv.org/pdf/1905.03994)

   *Jia Li, Zhichao Han, Hong Cheng, Jiao Su, Pengyun Wang, Jianfeng Zhang, Lujia Pan.*

1. **Stochastic Weight Completion for Road Networks using Graph Convolutional Networks.** ICDE 2019. [paper](http://people.cs.aau.dk/~byang/papers/ICDE2019-GCWC.pdf)

   *Jilin Hu, Chenjuan Guo, Bin Yang, Christian S. Jensen.*

1. **STG2Seq: Spatial-temporal Graph to Sequence Model for Multi-step Passenger Demand Forecasting.** IJCAI 2019. [paper](https://arxiv.org/pdf/1905.10069.pdf)

   *Lei Bai, Lina Yao, Salil.S Kanhere, Xianzhi Wang, Quan.Z Sheng.*

1. **Graph WaveNet for Deep Spatial-Temporal Graph Modeling.** IJCAI 2019. [paper](https://shiruipan.github.io/pdf/IJCAI-19-graph-wavenet.pdf)

   *Zonghan Wu, Shirui Pan, Guodong Long, Jing Jiang, Chengqi Zhang.*

1. **Semi-Supervised Hierarchical Recurrent Graph Neural Network for City-Wide Parking Availability Prediction.** AAAI 2020. [paper](https://arxiv.org/pdf/1911.10516.pdf)

   *Weijia Zhang, Hao Liu, Yanchi Liu, Jingbo Zhou, Hui Xiong.*

1. **Social-BiGAT: Multimodal Trajectory Forecasting using Bicycle-GAN and Graph Attention Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-75)

   *Vineet Kosaraju, Amir Sadeghian, Roberto Martín-Martín, Ian Reid, Hamid Rezatofighi, Silvio Savarese.*

1. **GMAN: A Graph Multi-Attention Network for Traffic Prediction.** AAAI 2020. [paper](https://arxiv.org/abs/1911.08415)

   *Chuanpan Zheng, Xiaoliang Fan, Cheng Wang, Jianzhong Qi.*

### [Few-shot and Zero-shot Learning](#content)

1. **Few-Shot Learning with Graph Neural Networks.** ICLR 2018. [paper](https://arxiv.org/pdf/1711.04043.pdf)

   *Victor Garcia, Joan Bruna.* 

1. **Prototype Propagation Networks (PPN) for Weakly-supervised Few-shot Learning on Category Graph.** IJCAI 2019. [paper](https://arxiv.org/pdf/1905.04042.pdf)

   *Lu Liu, Tianyi Zhou, Guodong Long, Jing Jiang, Lina Yao, Chengqi Zhang.*

1. **Edge-labeling Graph Neural Network for Few-shot Learning.** CVPR 2019. [paper](https://arxiv.org/pdf/1905.01436.pdf)

   *Jongmin Kim, Taesup Kim, Sungwoong Kim, Chang D. Yoo.*

1. **Generating Classification Weights with GNN Denoising Autoencoders for Few-Shot Learning.** CVPR 2019. [paper](https://arxiv.org/pdf/1905.01102.pdf)

   *Spyros Gidaris, Nikos Komodakis.*

1. **Zero-shot Recognition via Semantic Embeddings and Knowledge Graphs.** CVPR 2018. [paper](https://arxiv.org/pdf/1803.08035.pdf)

   *Xiaolong Wang, Yufei Ye, Abhinav Gupta.* 

1. **Rethinking Knowledge Graph Propagation for Zero-Shot Learning.** CVPR 2019. [paper](https://arxiv.org/pdf/1805.11724.pdf)

   *Michael Kampffmeyer, Yinbo Chen, Xiaodan Liang, Hao Wang, Yujia Zhang, Eric P. Xing.* 

1. **Multi-Label Zero-Shot Learning with Structured Knowledge Graphs.** CVPR 2018. [paper](https://arxiv.org/pdf/1711.06526.pdf)

   *Chung-Wei Lee, Wei Fang, Chih-Kuan Yeh, Yu-Chiang Frank Wang.* 

1. **Learning to Propagate for Graph Meta-Learning.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-610)

   *LU LIU, Tianyi Zhou, Guodong Long, Jing Jiang, Chengqi Zhang.*

1. **Zero-Shot Video Object Segmentation via Attentive Graph Neural Networks** ICCV 2019. [paper](https://arxiv.org/pdf/2001.06807.pdf)

   *Wenguan Wang, Xiankai Lu, Jianbing Shen, David Crandall, Ling Shao.*

1. **Attribute Propagation Network for Graph Zero-­shot Learning.** AAAI 2020. [paper]()

   *LU LIU, Tianyi Zhou, Guodong Long, Jing Jiang, Chengqi Zhang.*

1. **Graph Few-­‐shot Learning via Knowledge Transfer.** AAAI 2020. [paper](https://arxiv.org/abs/1910.03053)

   *Huaxiu Yao, Chuxu Zhang, Ying WEI, Meng Jiang, Suhang Wang, Junzhou Huang, Nitesh Chawla, Zhenhui Li.*

1. **FEW-SHOT LEARNING ON GRAPHS VIA SUPER-CLASSES BASED ON GRAPH SPECTRAL MEASURES.** ICLR 2020. [paper](https://openreview.net/pdf?id=Bkeeca4Kvr)

   *Jatin Chauhan, Deepak Nathani, Manohar Kaul.*

1. **Learning to Extrapolate Knowledge: Transductive Few-shot Out-of-Graph Link Prediction.** NeurIPS 2020. [paper](https://arxiv.org/abs/2006.06648)

   *Jinheon Baek, Dong Bok Lee, Sung Ju Hwang.*

1. **Graph Meta Learning via Local Subgraphs.** NeurIPS 2020. [paper](https://papers.nips.cc/paper/2020/hash/412604be30f701b1b1e3124c252065e6-Abstract.html)

   *Kexin Huang, Marinka Zitnik.*

### [Program Representation](#content)

1. **Learning to Represent Programs with Graphs.** ICLR 2018. [paper](https://arxiv.org/abs/1711.00740)

   *Miltiadis Allamanis, Marc Brockschmidt, Mahmoud Khademi.*

1. **Open Vocabulary Learning on Source Code with a Graph-Structured Cache.** ICML 2019. [paper](https://arxiv.org/pdf/1810.08305)

   *Milan Cvitkovic, Badal Singh, Anima Anandkumar.*

1. **Devign: Effective Vulnerability Identification by Learning Comprehensive Program Semantics via Graph Neural Networks.** NeurIPS 2019. [paper](http://papers.nips.cc/paper/by-source-2019-5389)

   *Yaqin Zhou, Shangqing Liu, Jingkai Siow, Xiaoning Du, Yang Liu.*

1. **LambdaNet: Probabilistic Type Inference using Graph Neural Networks.** ICLR 2020. [paper](https://openreview.net/pdf?id=Hkx6hANtwH)

   *Jiayi Wei, Maruth Goyal, Greg Durrett, Isil Dillig.*

1. **HOPPITY: LEARNING GRAPH TRANSFORMATIONS TO DETECT AND FIX BUGS IN PROGRAMS.** ICLR 2020. [paper](https://openreview.net/pdf?id=SJeqs6EFvB)

   *Elizabeth Dinella, Hanjun Dai, Ziyang Li, Mayur Naik, Le Song, Ke Wang.*

### [Social Network](#content)

1. **Link Prediction Based on Graph Neural Networks.** NeurIPS 2018. [paper](https://arxiv.org/pdf/1802.09691.pdf)

   *Muhan Zhang, Yixin Chen.*

1. **DeepInf: Social Influence Prediction with Deep Learning.** KDD 2018. [paper](https://arxiv.org/pdf/1807.05560.pdf)

   *Jiezhong Qiu, Jian Tang, Hao Ma, Yuxiao Dong, Kuansan Wang, Jie Tang.*

1. **Characterizing and Forecasting User Engagement with In-app Action Graph: A Case Study of Snapchat.** KDD 2019. [paper](https://arxiv.org/pdf/1906.00355)

   *Yozen Liu, Xiaolin Shi, Lucas Pierce, Xiang Ren.*

1. **MCNE: An End-to-End Framework for Learning Multiple Conditional Network Representations of Social Network.** KDD 2019. [paper](https://arxiv.org/pdf/1905.11013)

   *Hao Wang, Tong Xu, Qi Liu, Defu Lian, Enhong Chen, Dongfang Du, Han Wu, Wen Su.*

1. **Is a Single Vector Enough? Exploring Node Polysemy for Network Embedding.** KDD 2019. [paper](https://arxiv.org/pdf/1905.10668)

   *Ninghao Liu, Qiaoyu Tan, Yuening Li, Hongxia Yang, Jingren Zhou, Xia Hu.*

1. **Encoding Social Information with Graph Convolutional Networks for Political Perspective Detection in News Media.** ACL 2019. [paper](https://www.cs.purdue.edu/homes/dgoldwas//downloads/papers/LiG_acl_2019.pdf)

   *Chang Li, Dan Goldwasser.*

1. **Fine-grained Event Categorization with Heterogeneous Graph Convolutional Networks.** IJCAI 2019. [paper](https://arxiv.org/pdf/1906.04580.pdf)

   *Hao Peng, Jianxin Li, Qiran Gong, Yangqiu Song, Yuanxing Ning, Kunfeng Lai, Philip S. Yu.*

1. **Graph Convolutional Networks with Markov Random Field Reasoning for Social Spammer Detection.** AAAI 2020. [paper](http://staff.ustc.edu.cn/~liandefu/paper/aaai2020_spammer.pdf)

   *Yongji Wu, Defu Lian, Yiheng Xu, Le Wu, Enhong Chen.*

1. **Rumor Detection on Social Media with Bi-Directional Graph Convolutional Networks.** AAAI 2020. [paper](https://arxiv.org/abs/2001.06362)

   *Tian Bian, Xi Xiao, Tingyang Xu, Peilin Zhao, Wenbing Huang, Yu Rong, Junzhou Huang.*

### [Graph Matching](#content)

1. **Deep Graph Matching Consensus.** ICLR 2020. [paper](https://openreview.net/pdf?id=HyeJf1HKvS)

   *Matthias Fey, Jan E. Lenssen, Christopher Morris, Jonathan Masci, Nils M. Kriege.*


### [Computer Network](#content)

1. **Unveiling the potential of Graph Neural Networks for network modeling and optimization in SDN.** ACM SOSR 2019. [paper](https://arxiv.org/pdf/1901.08113.pdf)

   *Krzysztof Rusek, José Suárez-Varela, Albert Mestres, Pere Barlet-Ros, Albert Cabellos-Aparicio.*

