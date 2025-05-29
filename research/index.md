---
title: Research in the Chitra lab
layout: default
group: research
---

# Research
We develop the next generation of machine learning (ML) methods for addressing fundamental problems in biology. 

Our major motivation is the rapid development of new biological technologies -- including single-cell/spatial sequencing and CRISPR -- which measure diverse molecular modalities at unprecedented throughput and resolution. ML methods are essential for analyzing and interpreting these large, high-dimensional, and multi-modal biological datasets. However, **standard "off-the-shelf" ML methods are severely challenged by the high noise, sparsity, heterogeneity, and other limitations of modern technologies**. 

We address these challenges by developing ML methods that can extract meaningful biological insights from noisy biomedical data. Our methods draw on techniques from many different disciplines including deep learning, graph theory, statistical inference, and complex analysis. Our research involes developing both new **mathematical theory** and **practical algorithms**.

-------------------

### ML for spatial biology
<table>
<tr>
<td width="70%" markdown="1">
Spatial sequencing technologies measure both high-throughput cellular measurements (e.g. gene expression) and the spatial location of measured cells. We develop spatial ML methodologies for learning the **latent geometric structure**  and **cellular interactions** in healthy and diseased biological tissues.

* **Gene expression topography**: a new mathematical and deep learning framework for learning *topographic maps* of 2-D tissue slices which reveal spatial gradients and tissue geometry.
    * [**GASTON**](https://www.nature.com/articles/s41592-024-02503-3): a neural field-based approach 
    * [**GASTON-Mix**](https://www.biorxiv.org/content/10.1101/2025.01.31.635955v1): spatial mixture-of-experts (MoE)
    * Builds on previous method [**Belayer**](https://www.sciencedirect.com/science/article/pii/S2405471222003544) which **introduced complex analysis to spatial biology**.
* Learning **cellular interactions** with statistical/causal inference methods.
    * [**Copulacci**](https://academic.oup.com/bioinformatics/article/40/Supplement_1/i481/7700859): using bivariate copula distributions to learn **local** cellular interactions.
    * [**GLACIER**](https://www.biorxiv.org/content/10.1101/2025.03.19.644241v2.abstract) (w/ [Rohit Singh lab](https://singhlab.net/)): DAG-based Granger causality and gene expression topography to identify **global** cellular interactions.
</td>
<td width="40%">
<img src="/static/img/research/gene_expression_topography.png" width="100%">
</td>
</tr>
</table>

-------------------

### Biological networks
<table>
<tr>
<td width="70%" markdown="1">
Biological interaction networks underlie many aspects of human health and disease, but existing networks are highly incomplete (missing ≈90% of edges). We develop statistical methodologies for learning interaction networks from noisy biological data.

* [**DIALECT**](https://www.biorxiv.org/content/10.1101/2024.04.24.590995v1): a **latent variable model** for learning interactions between cancer driver genes using somatic mutation data.
* A [**multivariate Bernoulli-based framework**](https://www.nature.com/articles/s41467-025-56986-5) that unifies the different approaches for quantifying higher-order (>3-way) genetic interactions (*epistasis*).
</td>
<td width="40%">
<img src="/static/img/research/biological_networks.png" width="82%">
</td>
</tr>
</table>

-------------------

### Graph-based anomaly detection

<table>
<tr>
<td width="70%" markdown="1">
Anomalous interactions between genes/proteins underlie many complex diseases. We develop methodologies for anomaly detection in networks and other structured data (e.g. time series, matrices).

* [**NetMix**](https://www.liebertpub.com/doi/full/10.1089/cmb.2020.0435) and [**NetMix2**](https://www.liebertpub.com/doi/full/10.1089/cmb.2022.0336): asymptotically unbiased combinatorial optimization algorithms for anomaly detection in protein-protein interaction (PPI) networks.
    * We prove that many existing network anomaly detection methods are *statistically biased*. By correcting this bias, we achieve state-of-the-art performance in disease gene identification.
* A [**statistical framework for structured anomaly detection**](https://proceedings.mlr.press/v139/chitra21a.html) that unifies existing anomaly detection methods in biology, statistics, and epidemiology.
</td>
<td width="40%">
<img src="/static/img/research/anomaly_detection.png" width="100%">
</td>
</tr>
</table>

