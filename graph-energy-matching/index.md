---
layout: project
title: Graph Energy Matching
---

# Graph Energy Matching

**Transport-Aligned Energy-Based Modeling for Graph Generation**

<p class="project-authors"><a href="https://michalbalcerak.ai/">Michal Balcerak</a>, Suprosana Shit, Chinmay Prabhakar, Sebastian Kaltenbach, Michael S. Albergo, Yilun Du, Bjoern Menze</p>

<p class="project-links"><strong>Preprint 2026</strong> / <a href="https://arxiv.org/abs/2603.23398">arXiv</a> / <span class="resource-status">Code coming soon</span></p>

<img class="project-hero-image" src="{{ '/assets/news/gem_higher.png' | relative_url }}" alt="Graph Energy Matching sampling overview">

## Abstract

Generative modeling of discrete data, such as graphs, underpins many scientific and industrial applications, including molecular discovery and materials design. In these domains, probabilistic inference is particularly valuable, as it enables composable generation and principled incorporation of desired constraints, such as structural or functional properties. Energy-based models naturally support this goal by capturing relative likelihoods and enabling composable inference by directly enforcing constraints during inference. However, discrete energy-based models typically struggle with efficient and high-quality sampling, as off-support regions often contain spurious local minima, trapping samplers and causing training instabilities, resulting in a fidelity gap compared to discrete diffusion models. To address this gap, we introduce <em>Graph Energy Matching (GEM)</em>, a discrete generative framework inspired by the Jordan&ndash;Kinderlehrer&ndash;Otto (JKO) transport-map optimization perspective. GEM learns a permutation-invariant potential energy that simultaneously guides discrete transport from noise toward high-likelihood graph regions and refines samples within these regions. We further introduce a sampling protocol leveraging an energy-based switching strategy, seamlessly bridging rapid, gradient-guided transport and a local mixing regime for effective exploration. On molecular graph benchmarks, GEM matches or surpasses strong discrete diffusion baselines on most reported metrics. Beyond improving generation quality, GEM's relative likelihood modeling enables targeted exploration, facilitating compositional generation, property-constrained sampling, and interpolation between graphs.

## Resources

<p class="project-links"><a href="https://arxiv.org/abs/2603.23398">arXiv</a> / <span class="resource-status">Code coming soon</span></p>

## Citation

```bibtex
@article{balcerak2026graphenergymatching,
  title={Graph Energy Matching: Transport-Aligned Energy-Based Modeling for Graph Generation},
  author={Balcerak, Michal and Shit, Suprosana and Prabhakar, Chinmay and Kaltenbach, Sebastian and Albergo, Michael S. and Du, Yilun and Menze, Bjoern},
  journal={arXiv preprint arXiv:2603.23398},
  year={2026}
}
```
