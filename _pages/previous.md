---
title: "Previous Efforts"
classes: wide
layouy: single
permalink: /previous/
author_profile: true
---

<style>
h2 {
    font-family: "Garamond", serif;
    font-style: normal;
    font-size: 38px;
    font-weight: bold;
    color: #95bff3;
}
h3 {
    font-size: 30px;
    color: #5c6eb0;
}
h5 {
    color: #5c6eb0;
}
body {
    font-size: 18px;
}
p:has(+ ul) {   
  margin-bottom: 0;
}
p + ul {
  margin-top: 0;
}
</style>


## Doctorate at IMT Atlantique

Focused on ocean data processing, my Ph.D. Thesis aimed to answer the question:
> "How can we exploit the complementary information conveyed by diverse, multi-sensor and spatio-temporally heterogeneous data to improve the characterization of the sea surface state?"

This problem was framed as a geophysical inverse problem. That is, to retrieve a bigger picture from its partial observations. In this case, the bigger picture is the dynamical behavior of sea-surface wind speed and the partial observations are the output of the measurement methods that can be use to gauge the phenomenon. Wind speed at the sea surface is an important parameter for a vast range of anthropic activities. The spatial extent of the sea surface and the strong spatio-temporal variability of wind speed makes each individual measurement method undercomplete and uncapable of capturing all of wind speed complexity.

The methodological approach involved an end-to-end trainable framework, the 4DVarNet. See [the *core* 4DVarNet official repo](https://github.com/CIA-Oceanix/4dvarnet-core), [the *started* 4DVarNet official repo](https://github.com/CIA-Oceanix/4dvarnet-starter) and [the original paper](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021MS002572) for details*. This framework bridges traditional physics-based geophysical inversion schemes and deep learning modelling. The objective is to make the most of theoretical foundations, the flexibility and representation power of deep learning and the availability of large data sets.

*I did not contribute to the development of 4DVarNet. The original authors are listed in the repository and in the publication mentioned above.

**Contributions**: We contributed with two original papers and one conference proceeding. In the following, a brief description of the main work axes.

##### <i class="fa-regular fa-file-lines"></i> Multimodal Learning-based Reconstruction of High-resolution Spatial Wind Speed Fields
Published in January 2025, the work has been done between 2022 and 2023.\
<i class="fa-solid fa-angles-right"></i> [Original article](https://www.cambridge.org/core/journals/environmental-data-science/article/multimodal-learningbased-reconstruction-of-highresolution-spatial-wind-speed-fields/18946D2FE8B1B72A9334DD2C2FF68909) in Environmental Data Science.\
<i class="fa-solid fa-angles-right"></i> [Arxiv preprint](https://arxiv.org/abs/2312.08933), posted in December 2023.

In this work, we used the 4DVarNet framework to reconstruct high-resolution sea-surface wind speed fields. Our goal was to leverage wind speed data across multiple spatiotemporal scales to maximize the contribution of each input source. Using simulated data, we integrated diverse pseudo-observations—including satellite images, in situ measurements, and reanalysis products—to capture wind speed variability more effectively. Extensive numerical experiments show that this multimodal approach outperforms traditional deep learning inversion methods by successfully combining complementary information from various inputs. We also prove that the scheme may benefice of further capacity by processing separately the automatically learned features of the heterogeneous partial observations.  

##### <i class="fa-regular fa-file-lines"></i> Learning-Based Temporal Estimation of In-Situ Wind Speed From Underwater Passive Acoustics
Published in August 2023, the work has been done in 2022.\
<i class="fa-solid fa-angles-right"></i> [Original article](https://ieeexplore.ieee.org/abstract/document/10229988) in IEEE Journal of Oceanic Engineering.

In this work, we aimed to reconstruct the sea-surface wind speed using underwater passive acoustics. This problem is, unlike the one presented above, local in space. We build on previous work that leveraged machine learning techniques to invert underwater acoustics to estimate wind speed. The novelty proposed by our work consisted in the reconstruction of the wind speed time-related dynamical patterns. The 4DVarNet scheme represents a suitable choice given its physical foundations. Our experiments on real data demonstrate that the our proposed approach outperforms existing data-driven techniques, achieving up to a 16% reduction in RMSE on wind speed reconstruction. The study emphasizes the role of temporal dynamics in underwater acoustic data and suggests that incorporating multimodal information can further enhance robustness, particularly in cases of missing acoustic data.


## Research Fellowship at CCNL UniPD

