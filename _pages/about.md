---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hi! I am Shengjie Luo (罗胜杰), a fourth-year Ph.D. student at School of Intelligence Science and Technology in Peking University, advised by [Prof.Liwei Wang](http://www.liweiwang-pku.com/) and [Prof.Di He](https://dihe-pku.github.io/). Before that, I finished my undergraduate study at ShenYuan Honors College in Beihang University, majoring in Computer Science. I have been a research intern at [Microsoft Research Asia](https://www.msra.cn/).

My main research area lies in machine learning, with special interests in models and algorithms inspired by theoretical insights. Recently, my works focus on representation learning on structured data (e.g., graphs and sequences) and provide comprehensive analysis on foundational architectures (Transformers, GNNs) covering their expressiveness, efficiency and effectiveness, as well as apply them to AI for Science, Graph Learning and Natural Language Processing. I have published several papers and been reviewers at the top machine learning and artificial intelligence conferences such as NeurIPS, ICML and ICLR.

If you are interested in collaborating with me or want to have a chat, always feel free to contact me through e-mail or WeChat :)



# 🔥 News
- *2024.05*: Two papers are accepted at ICML 2024!
- *2024.01*: Our paper "Enabling Efficient Equivariant Operations in the Fourier Basis via Gaunt Tensor Products" is selected as  **<font color="#DC143C">Spotlight Presentation</font>** (top 4.96%) at ICLR 2024, see you in Vienna!
- *2024.01*: One paper is accepted at ICLR 2024!
- *2023.03*: Our paper "Rethinking the Expressive Power of GNNs via Graph Biconnectivity" received the  
             **<font color="#DC143C">ICLR 2023 Outstanding Paper Award</font>** (top 4/4966)!
- *2023.01*: Two papers are accepted at ICLR 2023!
- *2022.11*: Transformer-M has been used by all Top-3 winners in [PCQM4Mv2 Track, 2nd OGB Large-Scale Challenge, NeurIPS 2022](https://ogb.stanford.edu/neurips2022/results/#winners_pcqm4mv2)!
- *2022.09*: One paper is accepted at NeurIPS 2022! 
- *2021.09*: Two papers are accepted at NeurIPS 2021!
- *2021.06*: Graphormer won the 1st place in [PCQM4M Track, OGB Large-Scale Challenge, KDD CUP 2021](https://ogb.stanford.edu/kddcup2021/results/#awardees-of-pcqm4m-lsc-track-leaderboard)!
- *2021.05*: One paper is accepted at ICML 2021!

# 📝 Selected Publications ([Full List](https://scholar.google.com/citations?user=ImWO7WYAAAAJ&hl=en))
\* denotes equal contribution, † denotes correspondence authorship.
<div class='paper-box'><div class='paper-box-image'><div><img src='images/Gaunt-Tensor-Product.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICLR 2024 <font color="#DC143C">Spotlight (top 4.96%)</font>**] [Enabling Efficient Equivariant Operations in the Fourier Basis via Gaunt Tensor Products](https://arxiv.org/abs/2401.10216)

**Shengjie Luo**\*, Tianlang Chen\*, Aditi S. Krishnapriyan

[**[Project]**](https://openreview.net/forum?id=mhyQXJ6JsK) [**[Code]**](https://github.com/lsj2408/Gaunt-Tensor-Product) 
- We develop a brandly new and systematic method to substantially improve the efficiency of the mainstream E(3) equivariant operations, tensor product of irreps, opening up a new opportunity to pushing the frontier of Geometric Deep Learning and its application in Science.
- A new perspective: we reveal the relationship between Clebsch-Gordan coefficients and Gaunt coefficients spherical harmonics, connecting tensor product of Gaunt coefficients with integrals of products between three spherical functions.
- A new opportunity: instead of using spherical harmonics, products between spherical functions expressed as 2D Fourier Basis can be accelerated.
- We introduce Gaunt Tensor Product, a principled approach to accelerate Tensor Product of Irreps, the complexity of which is reduced to just O(L^3) instead of O(L^6).
- Our method opens up a new pathway for revolutionizing modern E(3) Equivariant Neural Networks, and extensive experiments further demonstrate the efficiency and generality of our Gaunt Tensor Product approach.

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/GeoMFormer.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICML 2024**] [GeoMFormer: A General Architecture for Geometric Molecular Representation Learning](https://openreview.net/forum?id=xLRAQiqd9I)

Tianlang Chen\*, **Shengjie Luo**\*†, Di He, Shuxin Zheng, Tie-Yan Liu, Liwei Wang

[**[Project]**](https://openreview.net/forum?id=xLRAQiqd9I) [**[Code]**](https://openreview.net/forum?id=xLRAQiqd9I) 
- We develop a Transformer-based Geometric Molecular model called GeoMFormer, which can effectively perform both invariant and equivariant prediction with strong performance
at the same time.
- By allowing simultaneously and completely modeling interatomic interactions within/across feature spaces in a unified manner, GeoMFormer achieved strong performance covering diverse data modalities, scales and tasks with both invariant and equivariant targets, opening up a new pathway towards scientific AI generalist.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/BiPE.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICML 2024**] [Two Stones Hit One Bird: Bilevel Positional Encoding for Better Length Extrapolation](https://arxiv.org/abs/2401.16421)

Zhenyu He\*, Guhao Feng\*, **Shengjie Luo**\*, Kai Yang, Liwei Wang, Jingjing Xu, Zhi Zhang, Hongxia Yang, Di He

[**[Project]**](https://arxiv.org/abs/2401.16421) [**[Code]**](https://github.com/zhenyuhe00/BiPE) 
- We develop a bilevel positional encoding, which has superior length extrapolation capabilities across diverse text modalities and tasks.
- Leveraging the intrinsic segmentation of language sequences, our BiPE blends an intra-segment encoding and an inter-segment encoding.
- The intra-segment encoding identifies the locations within a segment and helps the model capture the semantic information therein via absolute PE.
- The inter-segment encoding specifies the segment index, models the relationships between segments, and aims to improve extrapolation capabilities via relative PE.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Graphormer-GD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICLR 2023 <font color="#DC143C">Outstanding Paper Award (top 4/4966)</font>**] [Rethinking the Expressive Power of GNNs via Graph Biconnectivity](https://arxiv.org/abs/2301.09505)

Bohang Zhang\*, **Shengjie Luo**\*, Liwei Wang, Di He

[**[Project]**](https://openreview.net/forum?id=r9hNv76KoT3) [**[Code]**](https://github.com/lsj2408/Graphormer-GD)
- Beyond the WL test, we propose a fundamentally different perspective, a novel class of expressivity metrics via 🚀**Graph Biconnectivity**🚀, to study the expressive power of GNNs.
- Through the lens of graph biconnectivity, we systematically investigate popular GNNs including classic MPNNs, Graph Substructure Networks (GSN) and its
variant, GNN with lifting transformations (MPSN and CWN), GraphSNN, and Subgraph GNNs. The thorough analysis provide a fine-grained understanding on the expressive power of existing GNNs.
- Based on the above theoretical analysis, we develop a principled and more efficient approach, called the Generalized Distance Weisfeiler-Lehman (GD-WL), which is provably expressive for all biconnectivity metrics. 
- We further develop Graphormer-GD to implement the GD-WL, which is a Transformer-like architecture that preserves expressiveness and enjoys full parallelizability. 
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Transformer-M.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICLR 2023**] [One Transformer Can Understand Both 2D & 3D Molecular Data](https://arxiv.org/abs/2210.01765)

**Shengjie Luo**, Tianlang Chen\*, Yixian Xu\*, Shuxin Zheng, Tie-Yan Liu, Liwei Wang, Di He

[**[Project]**](https://ogb.stanford.edu/docs/lsc/leaderboards/#pcqm4mv2) [**[Code]**](https://github.com/lsj2408/Transformer-M) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/one-transformer-can-understand-both-2d-3d/graph-regression-on-pcqm4mv2-lsc)](https://paperswithcode.com/sota/graph-regression-on-pcqm4mv2-lsc?p=one-transformer-can-understand-both-2d-3d)
- We develop a novel Transformer-based Molecular model called Transformer-M, which can take molecular data of 2D or 3D formats as input and generate meaningful semantic representations.
- Using the standard Transformer as the backbone architecture, Transformer-M develops two separated channels to encode 2D and 3D structural information and incorporate them with the atom features in the network modules. When the input data is in a particular format, the corresponding channel will be activated, and the other will be disabled.
- We conduct extensive experiments to show that Transformer-M can simultaneously achieve strong performance on 2D and 3D tasks (PCQM4Mv2 (2D), PDBBind (2D+3D), QM9 (3D)), suggesting its broad applicability.
- 🚀 Transformer-M has been used by **all Top-3 winners** in [**PCQM4Mv2 Track, 2nd OGB Large-Scale Challenge, NeurIPS 2022**](https://ogb.stanford.edu/neurips2022/results/#winners_pcqm4mv2)!
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/URPE.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**NeurIPS 2022**] [Your Transformer May Not be as Powerful as You Expect](https://arxiv.org/abs/2205.13401)

**Shengjie Luo**\*, Shanda Li\*, Shuxin Zheng, Tie-Yan Liu, Liwei Wang, Di He

[**[Project]**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ImWO7WYAAAAJ&citation_for_view=ImWO7WYAAAAJ:_FxGoFyzp5QC) [**[Code]**](https://github.com/lsj2408/URPE)
- We mathematically analyze the expressive power of RPE-based Transformers, and show that they are not universal approximators of continuous sequence-to-sequence functions.
- We then present sufficient conditions for RPE-based Transformers to achieve universal function approximation. With the theoretical guidance, we develop Universal RPE-based (URPE) Attention, which is easy to implement and parameter-efficient.
- Our URPE-based Transformers are verified to be universal approximators from both theoretical analysis and extensive experiments including synthetic tasks, language modeling and graph learning.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Graphormer.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**NeurIPS 2021**] [Do Transformers Really Perform Badly for Graph Representation?](https://proceedings.neurips.cc/paper/2021/hash/f1c1592588411002af340cbaedd6fc33-Abstract.html)

Chengxuan Ying, Tianle Cai, **Shengjie Luo**, Shuxin Zheng, Guolin Ke, Di He, Yanming Shen, Tie-Yan Liu

[**[Project]**](https://neurips.cc/virtual/2021/poster/27679) [**[Code]**](https://github.com/microsoft/Graphormer) [**[Technical Report]**](https://arxiv.org/abs/2106.08279) [**[Slides]**](https://neurips.cc/media/neurips-2021/Slides/27679_XmkCZkZ.pdf) [**[Video]**](https://slideslive.com/38967017/graphormer-a-generalpropose-backbone-for-graph-learning?ref=speaker-30327)
- Make Transformer great again on graph representation learning by introducing three graph structural encodings.
- Achieve SOTA performance on several benchmarks covering [OGB](https://ogb.stanford.edu/) and [Benchmarking GNNs](https://arxiv.org/abs/2203.04810).
- 1st place winner of [PCQM4M Track, OGB Large-Scale Challenge, KDD CUP 2021](https://ogb.stanford.edu/kddcup2021/results/#awardees-of-pcqm4m-lsc-track-leaderboard).
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/kernel_rpe.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**NeurIPS 2021**] [Stable, Fast and Accurate: Kernelized Attention with Relative Positional Encoding](https://proceedings.neurips.cc/paper/2021/hash/c0f168ce8900fa56e57789e2a2f2c9d0-Abstract.html)

**Shengjie Luo**\*, Shanda Li\*, Tianle Cai, Dinglan Peng, Di He, Shuxin Zheng, Guolin Ke, Liwei Wang, Tie-Yan Liu

[**[Project]**](https://neurips.cc/virtual/2021/poster/27095) [**[Code]**](https://openreview.net/forum?id=X7XNPor93uG) [**[Slides & Video]**](https://slideslive.com/38967015)
- We propose a novel way to accelerate attention calculation (O(nlog(n)) for Transformers with RPE on top of the kernelized attention.
- We mathematically show that kernelized attention with RPE can be calculated efficiently using Fast Fourier Transform (FFT), based on the Toeplitz matrix form of RPE.
- We further demonstrate that properly using RPE can mitigate the training instability problem of vanilla kernelized attention.
- Extensive experiments covering language pre-training, language modeling, Image Classification and Machine Translation are conducted to demonstrate the efficiency and effectiveness of our model.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/graphnorm.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICML 2021 <font color="#DC143C">Spotlight</font>**] [GraphNorm: A Principled Approach to Accelerating Graph Neural Network Training](https://proceedings.mlr.press/v139/cai21e)

Tianle Cai\*, **Shengjie Luo**\*, Keyulu Xu, Di He, Tie-Yan Liu, Liwei Wang

[**[Project]**](https://icml.cc/virtual/2021/poster/10655) [**[Slides]**](https://icml.cc/media/icml-2021/Slides/10655_KLtUTML.pdf) [**[Video]**](https://slideslive.com/38959667/graphnorm-a-principled-approach-to-accelerating-graph-neural-network-training?ref=search-presentations-GraphNorm)

[**[Code (Official)]**](https://github.com/lsj2408/GraphNorm) [**[Code (PyG)]**](https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.norm.GraphNorm) [**[Code (Microsoft ptgnn)]**](https://github.com/microsoft/ptgnn/blob/d30cb0d5858d026c6db2ec28bec840856c0d2d30/ptgnn/neuralmodels/gnn/messagepassing/graphnorm.py)
- We theoretically study the preconditioning effect of normalization methods on GNN training, and empirically observe that the batch noise of graph data is larger than data from other domain, e.g. image data.
- We further show that the shift operation in InstanceNorm can cause expressiveness degradation of GNNs for highly regular graphs.
- Based on these findings, we propose a principled normalization scheme, GraphNorm, and demonstrate its acceleration effect on graph learning benchmarks.
</div>
</div>

# 🎖 Honors and Awards
- *2023.03*, ICLR 2023 **<font color="#DC143C">Outstanding Paper Award</font>** (top 4/4966) [**[Link]**](https://blog.iclr.cc/2023/03/21/announcing-the-iclr-2023-outstanding-paper-award-recipients/).
- *2021.06*, 1st place Winner of PCQM4M Track, OGB Large Scale Challenge, KDD CUP 2021.
- *2018.12*, National Scholarship (Top 1%). 

# 📖 Educations
- *2022.09 - 2025.07 (expected)*, Ph.D. Student, School of Intelligence Science and Technology, Peking University.
- *2020.09 - 2022.07*,            Master Student, Center for Machine Learning Research, Peking University. 
- *2016.09 - 2020.07*,            Undergraduate Student, Shenyuan Honors College, Beihang University. 

# 💻 Internships
- *2021.12 - now*,     Machine Learning Group, Microsoft Research Asia, China.
- *2020.10 - 2021.06*, Machine Learning Group, Microsoft Research Asia, China.
- *2019.10 - 2020.06*, Natural Language Computing Group, Microsoft Research Asia, China.

# 💬 Invited Talks
- *2024.06*, [CCF TCS Outstanding Doctoral Student Forum](https://lsj2408.github.io). Towards Efficient and Effective Geometric Deep Learning.
- *2024.04*, [AI for Chemistry and Materials Science (AI4CM) Symposium, UC Berkeley \& MIT](https://lsj2408.github.io). Towards Efficient and Effective Geometric Deep Learning for Science. 
- *2024.03*, [FAI Seminar](https://www.fai-seminar.ac.cn/). Enabling Efficient Equivairant Operations in the Fourier Basis via Gaunt Tensor Products.
- *2023.06*, [FAI Seminar](https://www.fai-seminar.ac.cn/). One Transformer Can Understand Both 2D \& 3D Molecular Data.
- *2023.05*, [ICLR 2023 Oral Presentation](https://iclr.cc/Conferences/2023). Rethinking the Expressive Power of GNNs via Graph Biconnectivity.
- *2023.04*, [Scientific Machine Learning Webinar Series, Carnegie Mellon University](https://www.cmu.edu/aced/sciML.html). One Transformer Can Understand Both 2D \& 3D Molecular Data.
- *2022.11*, [Gaoling School of Artificial Intelligence, Renmin University of China](http://ai.ruc.edu.cn/). Your Transformer May Not be as Powerful as You Expect.
- *2022.11*, [AI Time](http://www.aitime.cn/). Your Transformer May Not be as Powerful as You Expect. \| [\[media\]](https://mp.weixin.qq.com/s/K14ASCTPrVpenPo95Ti3LA) 
- *2022.03*, [Huawei Technologies Noah's Ark Lab](https://noahlab.com.hk/#/home). Stable, Fast and Accurate: Kernelized Attention with Relative Positional Encoding.
- *2022.02*, [AI Time](http://www.aitime.cn/). Stable, Fast and Accurate: Kernelized Attention with Relative Positional Encoding. \| [\[media\]](https://mp.weixin.qq.com/s/EjPEwcvbl0xWAmjeVbPpNg) 

# 🏫 Professional Services
- Reviewer for ICLR 2022-2024, NeurIPS 2022-2024, ICML 2023-2024, LOG 2022-2023, CVPR 2024, COLM 2024.
- Reviewer for Nature Machine Intelligence and Transactions on Pattern Analysis and Machine Intelligence (TPAMI).

---
<center><sub>Visitor distribution </sub></center>
<center>
<script type="text/javascript" id="clustrmaps" src="//cdn.clustrmaps.com/map_v2.js?cl=b8d8f4&w=500&t=tt&d=dr5fouikEOHm7uz2Fbad0ouZVrWc6GgXdbKOPN3VGEs&co=ffffff&ct=110606&cmo=e073d6&cmn=53edcf"></script>
</center>
