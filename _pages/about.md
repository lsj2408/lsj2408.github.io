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

Hi! I am Shengjie Luo (罗胜杰), a first-year Ph.D. student at School of Intelligence Science and Technology in Peking University, advised by [Prof.Liwei Wang](http://www.liweiwang-pku.com/) and [Prof.Di He](https://dihe-pku.github.io/). Before that, I finished my undergraduate study at ShenYuan Honors College in Beihang University, majoring in Computer Science. I have been a research intern at [Microsoft Research Asia](https://www.msra.cn/).

My main research area lies in machine learning, with special interests in models and algorithms inspired by theoretical insights. Recently, my works focus on representation learning on structured data (e.g., graphs and sequences) and provide comprehensive analysis on base architectures (Transformers, GNNs) covering their expressiveness, efficiency and effectiveness, as well as apply them to Graph Learning, AI for Science and Natural Language Processing. I have published several papers and been reviewers at the top machine learning and artificial intelligence conferences such as NeurIPS, ICML and ICLR.

If you are interested in collaborating with me or want to have a chat, always feel free to contact me through e-mail or WeChat :)



# 🔥 News
- *2022.09*: One paper is accepted at NeurIPS 2022! 
- *2021.09*: Two papers are accepted at NeurIPS 2021!
- *2021.06*: Graphormer won the 1st place in [PCQM4M Track, OGB Large-Scale Challenge, KDD CUP 2021](https://ogb.stanford.edu/kddcup2021/results/#awardees-of-pcqm4m-lsc-track-leaderboard)!
- *2021.05*: One paper is accepted at ICML 2021!

# 📝 Selected Publications 
<div class='paper-box'><div class='paper-box-image'><div><img src='images/Transformer-M.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**Preprint**] [One Transformer Can Understand Both 2D & 3D Molecular Data](https://arxiv.org/abs/2210.01765)

**Shengjie Luo**, Tianlang Chen\*, Yixian Xu\*, Shuxin Zheng, Tie-Yan Liu, Liwei Wang, Di He

[**[Project]**](https://arxiv.org/abs/2210.01765) [**[Code]**](https://github.com/lsj2408/Transformer-M) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/one-transformer-can-understand-both-2d-3d/graph-regression-on-pcqm4mv2-lsc)](https://paperswithcode.com/sota/graph-regression-on-pcqm4mv2-lsc?p=one-transformer-can-understand-both-2d-3d)
- We develop a novel Transformer-based Molecular model called Transformer-M, which can take molecular data of 2D or 3D formats as input and generate meaningful semantic representations.
- Using the standard Transformer as the backbone architecture, Transformer-M develops two separated channels to encode 2D and 3D structural information and incorporate them with the atom features in the network modules. When the input data is in a particular format, the corresponding channel will be activated, and the other will be disabled.
- We conduct extensive experiments to show that Transformer-M can simultaneously achieve strong performance on 2D and 3D tasks (PCQM4Mv2 (2D), PDBBind (2D+3D), QM9 (3D)), suggesting its broad applicability.
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/URPE.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**NeurIPS 2022**] [Your Transformer May Not be as Powerful as You Expect](https://arxiv.org/abs/2205.13401)

**Shengjie Luo**\*, Shanda Li\*, Shuxin Zheng, Tie-Yan Liu, Liwei Wang, Di He

[**[Project]**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ImWO7WYAAAAJ&citation_for_view=ImWO7WYAAAAJ:_FxGoFyzp5QC)
- We mathematically analyze the expressive power of RPE-based Transformers, and show that they are not universal approximators of continuous sequence-to-sequence functions.
- We then present sufficient conditions for RPE-based Transformers to achieve universal function approximation. With the theoretical guidance, we develop Universal RPE-based (URPE) Attention, which is easy to implement and parameter-efficient.
- Our URPE-based Transformers are verified to be universal approximators from both theoretical analysis and extensive experiments including synthetic tasks, language modeling and graph learning.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Graphormer.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**NeurIPS 2021**] [Do Transformers Really Perform Badly for Graph Representation?](https://proceedings.neurips.cc/paper/2021/hash/f1c1592588411002af340cbaedd6fc33-Abstract.html)

Chengxuan Ying, Tianle Cai, **Shengjie Luo**, Shuxin Zheng, Guolin Ke, Di He, Yanming Shen, Tie-Yan Liu

[**[Project]**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ImWO7WYAAAAJ&citation_for_view=ImWO7WYAAAAJ:zYLM7Y9cAGgC) [**[Code]**](https://github.com/microsoft/Graphormer) [**[Technical Report]**](https://arxiv.org/abs/2106.08279)
- Make Transformer great again on graph classification by introducing three graph structural encodings.
- Achieve SOTA performance on several benchmarks covering [OGB](https://ogb.stanford.edu/) and [Benchmarking GNNs](https://arxiv.org/abs/2203.04810).
- [1st place winner of PCQM4M Track, OGB Large-Scale Challenge, KDD CUP 2021](https://ogb.stanford.edu/kddcup2021/results/#awardees-of-pcqm4m-lsc-track-leaderboard).
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/kernel_rpe.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**NeurIPS 2021**] [Stable, Fast and Accurate: Kernelized Attention with Relative Positional Encoding](https://proceedings.neurips.cc/paper/2021/hash/c0f168ce8900fa56e57789e2a2f2c9d0-Abstract.html)

**Shengjie Luo**\*, Shanda Li\*, Tianle Cai, Dinglan Peng, Di He, Shuxin Zheng, Guolin Ke, Liwei Wang, Tie-Yan Liu

[**[Project]**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ImWO7WYAAAAJ&citation_for_view=ImWO7WYAAAAJ:UeHWp8X0CEIC) [**[Code]**](https://openreview.net/forum?id=X7XNPor93uG)
- We propose a novel way to accelerate attention calculation (O(nlog(n)) for Transformers with RPE on top of the kernelized attention.
- We mathematically show that kernelized attention with RPE can be calculated efficiently using Fast Fourier Transform (FFT), based on the Toeplitz matrix form of RPE.
- We further demonstrate that properly using RPE can mitigate the training instability problem of vanilla kernelized attention.
- Extensive experiments covering language pre-training, language modeling, Image Classification and Machine Translation are conducted to demonstrate the efficiency and effectiveness of our model.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/graphnorm.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**ICML 2021**] [GraphNorm: A Principled Approach to Accelerating Graph Neural Network Training](https://proceedings.mlr.press/v139/cai21e)

Tianle Cai\*, **Shengjie Luo**\*, Keyulu Xu, Di He, Tie-Yan Liu, Liwei Wang

[**[Project]**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ImWO7WYAAAAJ&citation_for_view=ImWO7WYAAAAJ:IjCSPb-OGe4C) [**[Code (Official)]**](https://github.com/lsj2408/GraphNorm) [**[Code (PyG)]**](https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.norm.GraphNorm) [**[Code (Microsoft ptgnn)]**](https://github.com/microsoft/ptgnn/blob/d30cb0d5858d026c6db2ec28bec840856c0d2d30/ptgnn/neuralmodels/gnn/messagepassing/graphnorm.py)
- We theoretically study the preconditioning effect of normalization methods on GNN training, and empirically observe that the batch noise of graph data is larger than data from other domain, e.g. image data.
- We further show that the shift operation in InstanceNorm can cause expressiveness degradation of GNNs for highly regular graphs.
- Based on these findings, we propose a principled normalization scheme, GraphNorm, and demonstrate its acceleration effect on graph classification benchmarks.
</div>
</div>

# 🎖 Honors and Awards
- *2021.06*, 1st place Winner of PCQM4M Track, OGB Large Scale Challenge, KDD CUP 2021.
- *2018.12*, National Scholarship (Top 1%). 

# 📖 Educations
- *2022.09 - 2025.07 (expected)*, Ph.D. Student, School of Intelligence Science and Technology, Peking University.
- *2020.09 - 2022.07*,            Master Student, Academy for Advanced Interdisciplinary Studies, Peking University. 
- *2016.09 - 2020.07*,            Undergraduate Student, Shenyuan Honors College, Beihang University. 

# 💬 Invited Talks
- *2022.03*, [Huawei Technologies Noah's Ark Lab](https://noahlab.com.hk/#/home). Stable, Fast and Accurate: Kernelized Attention with Relative Positional Encoding.
- *2022.02*, [AI Time](http://www.aitime.cn/). Stable, Fast and Accurate: Kernelized Attention with Relative Positional Encoding. \| [\[media\]](https://mp.weixin.qq.com/s/EjPEwcvbl0xWAmjeVbPpNg) 

# 💻 Internships
- *2021.12 - now*,     Machine Learning Group, Microsoft Research Asia, China.
- *2020.10 - 2021.06*, Machine Learning Group, Microsoft Research Asia, China.
- *2019.10 - 2020.06*, Natural Language Computing Group, Microsoft Research Asia, China.

# 🏫 Professional Services
- Reviewer for ICLR 2022, NeurIPS 2022, LOG 2022.

---
<center><sub>Visitor distribution </sub></center>
<center>
<script type="text/javascript" id="clustrmaps" src="//cdn.clustrmaps.com/map_v2.js?cl=b8d8f4&w=500&t=tt&d=dr5fouikEOHm7uz2Fbad0ouZVrWc6GgXdbKOPN3VGEs&co=ffffff&ct=110606&cmo=e073d6&cmn=53edcf"></script>
</center>
