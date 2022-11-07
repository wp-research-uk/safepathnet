---
layout: home
title:   # unused
permalink: /
# subtitle: <a href='#'>Paper</a> <a href='#'>Code</a> <a href='#'>Video</a> <a href='#'>Poster</a>

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page

authors:
  - name: Stefano Pini
    affiliation: 1
  - name: Christian S. Perone
    affiliation: 1
  - name: Aayush Ahuja
    affiliation: 2
  - name: Ana Sofia Rufino Ferreira
    affiliation: 2
  - name: Moritz Niendorf
    affiliation: 2
  - name: Sergey Zagoruyko
    affiliation: 1

affiliations:
  - idx: 1
    name: Woven Planet United Kingdom Limited
  - idx: 2
    name: Woven Planet North America, Inc

links:
  - url: "https://arxiv.org/abs/2211.02131"
    text: Paper
    newtab: true
  - url: "https://github.com/woven-planet/l5kit"
    text: Code
    newtab: true
  - url: https://youtu.be/rLQXKcO20ck
    text: Video
    newtab: true
  # - url: "#"
  #   text: Poster
  #   newtab: true

main_image:
  path: method.svg
  caption: High-level overview of SafePathNet, a ML approach improving on-road safety of self-driving vehicles (SDVs).
---

## Abstract
<p class="text-justify">
  The goal of autonomous vehicles is to navigate public roads safely and comfortably. To enforce safety, traditional planning approaches rely on handcrafted rules to generate trajectories. Machine learning-based systems, on the other hand, scale with data and are able to learn more complex behaviors. However, they often ignore that agents and self-driving vehicle trajectory distributions can be leveraged to improve safety. In this paper, we propose modeling a distribution over multiple future trajectories for both the self-driving vehicle and other road agents, using a unified neural network architecture for prediction and planning. During inference, we select the planning trajectory that minimizes a cost taking into account safety and the predicted probabilities. Our approach does not depend on any rule-based planners for trajectory generation or optimization, improves with more training data and is simple to implement. We extensively evaluate our method through a realistic simulator and show that the predicted trajectory distribution corresponds to different driving profiles. We also successfully deploy it on a self-driving vehicle on urban public roads, confirming that it drives safely without compromising comfort. The code for training and testing our model on a public prediction dataset and the video of the road test are available at <a href="#">https://woven.mobi/safepathnet</a>.
</p>

## Road test
We evaluated our approach through a realistic simulator and tested it on a real SDV in both our private testing facility and on public roads. Results show that SafePathNet presents a better trade-off between comfort (discomfort braking, passiveness) and safety (collisions) and brings us another step closer to our goal of safe real-world autonomous driving.

<div class="video-container mb-3">
  <iframe src="https://www.youtube-nocookie.com/embed/rLQXKcO20ck" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## Citation
If you find our paper or code useful, please cite our work as:

<pre><code>@article{pini2022safe,
  title={Safe Real-World Autonomous Driving by Learning to Predict and Plan with a Mixture of Experts},
  author={Pini, Stefano and Perone, Christian S and Ahuja, Aayush and Ferreira, Ana Sofia Rufino and Niendorf, Moritz and Zagoruyko, Sergey},
  journal={arXiv preprint},
  year={2022}
}</code>
</pre>
