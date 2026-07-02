---
layout: project
title: Graph Energy Matching
---

# Graph Energy Matching

**Transport-Aligned Energy-Based Modeling for Graph Generation**

<p class="project-authors"><a href="https://michalbalcerak.ai/">Michal Balcerak</a><sup>1</sup>, <a href="https://www.dqbm.uzh.ch/en/research/menze/team/team-supro.html">Suprosanna Shit</a><sup>1</sup>, <a href="https://www.dqbm.uzh.ch/en/research/menze/team/team-chinmay.html">Chinmay Prabhakar</a><sup>1</sup>, <a href="https://seas.harvard.edu/person/sebastian-kaltenbach">Sebastian Kaltenbach</a><sup>2</sup>, <a href="https://malbergo.me/">Michael S. Albergo</a><sup>2,3</sup>, <a href="https://yilundu.github.io/">Yilun Du</a><sup>2,3,†</sup>, <a href="https://www.dqbm.uzh.ch/en/research/menze.html">Bjoern Menze</a><sup>1,†</sup></p>

<p class="project-affiliations"><sup>1</sup> University of Zurich · <sup>2</sup> Harvard University · <sup>3</sup> Kempner Institute</p>
<p class="project-author-note"><sup>†</sup> equal advising.</p>

<p class="project-venue"><strong>Preprint 2026</strong></p>
<div class="project-actions" aria-label="Graph Energy Matching resources">
  <a class="project-action" href="https://arxiv.org/pdf/2603.23398" aria-label="Read the Graph Energy Matching paper PDF on arXiv">
    <span class="project-action-icon project-action-icon--text" aria-hidden="true">arXiv</span>
    <span><strong>Paper</strong><small>arXiv PDF</small></span>
  </a>
  <a class="project-action" href="https://github.com/m1balcerak/GraphEnergyMatching" aria-label="View the Graph Energy Matching code on GitHub">
    <svg class="project-action-icon" viewBox="0 0 16 16" aria-hidden="true">
      <path fill="currentColor" d="M8 0C3.58 0 0 3.67 0 8.2c0 3.63 2.29 6.7 5.47 7.79.4.08.55-.18.55-.4 0-.2-.01-.86-.01-1.56-2.01.38-2.53-.5-2.69-.96-.09-.24-.48-.96-.82-1.16-.28-.16-.68-.56-.01-.57.63-.01 1.08.59 1.23.84.72 1.24 1.87.89 2.33.68.07-.53.28-.89.51-1.09-1.78-.21-3.64-.91-3.64-4.04 0-.89.31-1.62.82-2.19-.08-.21-.36-1.04.08-2.16 0 0 .67-.22 2.2.84A7.35 7.35 0 0 1 8 3.94c.68 0 1.36.09 2 .28 1.53-1.06 2.2-.84 2.2-.84.44 1.12.16 1.95.08 2.16.51.57.82 1.3.82 2.19 0 3.14-1.87 3.83-3.65 4.04.29.26.54.75.54 1.52 0 1.09-.01 1.97-.01 2.24 0 .22.15.48.55.4A8.13 8.13 0 0 0 16 8.2C16 3.67 12.42 0 8 0Z"/>
    </svg>
    <span><strong>Code</strong><small>GitHub</small></span>
  </a>
</div>

<img class="project-hero-image" src="{{ '/assets/news/gem_moses_animation.gif' | relative_url }}" alt="Graph Energy Matching MOSES sampling animation">

<figure class="project-method-figure">
  <a href="{{ '/assets/news/gem_higher.png' | relative_url }}" target="_blank" rel="noopener" aria-label="Open the Graph Energy Matching sampling overview figure at full resolution">
    <img src="{{ '/assets/news/gem_higher.png' | relative_url }}" alt="Graph Energy Matching sampling overview showing the transport phase and mixing phase">
  </a>
  <figcaption>GEM sampling overview: transport toward the data manifold followed by local energy-guided mixing.</figcaption>
</figure>

## Abstract

Generative modeling of discrete data, such as graphs, underpins many scientific and industrial applications, including molecular discovery and materials design. In these domains, probabilistic inference is particularly valuable, as it enables composable generation and principled incorporation of desired constraints, such as structural or functional properties. Energy-based models naturally support this goal by capturing relative likelihoods and enabling composable inference by directly enforcing constraints during inference. However, discrete energy-based models typically struggle with efficient and high-quality sampling, as off-support regions often contain spurious local minima, trapping samplers and causing training instabilities, resulting in a fidelity gap compared to discrete diffusion models. To address this gap, we introduce <em>Graph Energy Matching (GEM)</em>, a discrete generative framework inspired by the Jordan&ndash;Kinderlehrer&ndash;Otto (JKO) transport-map optimization perspective. GEM learns a permutation-invariant potential energy that simultaneously guides discrete transport from noise toward high-likelihood graph regions and refines samples within these regions. We further introduce a sampling protocol leveraging an energy-based switching strategy, seamlessly bridging rapid, gradient-guided transport and a local mixing regime for effective exploration. On molecular graph benchmarks, GEM matches or surpasses strong discrete diffusion baselines on most reported metrics. Beyond improving generation quality, GEM's relative likelihood modeling enables targeted exploration, facilitating compositional generation, property-constrained sampling, and interpolation between graphs.

## Citation

```bibtex
@article{balcerak2026graphenergymatching,
  title={Graph Energy Matching: Transport-Aligned Energy-Based Modeling for Graph Generation},
  author={Balcerak, Michal and Shit, Suprosanna and Prabhakar, Chinmay and Kaltenbach, Sebastian and Albergo, Michael S. and Du, Yilun and Menze, Bjoern},
  journal={arXiv preprint arXiv:2603.23398},
  year={2026}
}
```
