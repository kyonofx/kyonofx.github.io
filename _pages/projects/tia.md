---
layout: project_clean
permalink: /tia
# author_profile: true
# sidebar:
  # nav: "mymain"
gallery:
  - url: /assets/projects/tia/dmc_cheetah/gt.gif
    image_path: /assets/projects/tia/dmc_cheetah/gt.gif
    alt: "placeholder image 1"
  - url: /assets/projects/tia/dmc_cheetah/pred.gif
    image_path: /assets/projects/tia/dmc_cheetah/pred.gif
    alt: "placeholder image 2"
  - url: /assets/projects/tia/dmc_cheetah/joint.gif
    image_path: /assets/projects/tia/dmc_cheetah/joint.gif
    alt: "placeholder image 3"
  - url: /assets/projects/tia/dmc_cheetah/main.gif
    image_path: /assets/projects/tia/dmc_cheetah/main.gif
    alt: "placeholder image 4"
  - url: /assets/projects/tia/dmc_cheetah/disen.gif
    image_path: /assets/projects/tia/dmc_cheetah/disen.gif
    alt: "placeholder image 5"
  - url: /assets/projects/tia/dmc_hopper/gt.gif
    image_path: /assets/projects/tia/dmc_hopper/gt.gif
    alt: "placeholder image 1"
  - url: /assets/projects/tia/dmc_hopper/pred.gif
    image_path: /assets/projects/tia/dmc_hopper/pred.gif
    alt: "placeholder image 2"
  - url: /assets/projects/tia/dmc_hopper/joint.gif
    image_path: /assets/projects/tia/dmc_hopper/joint.gif
    alt: "placeholder image 3"
  - url: /assets/projects/tia/dmc_hopper/main.gif
    image_path: /assets/projects/tia/dmc_hopper/main.gif
    alt: "placeholder image 4"
  - url: /assets/projects/tia/dmc_hopper/disen.gif
    image_path: /assets/projects/tia/dmc_hopper/disen.gif
    alt: "placeholder image 5"
  - url: /assets/projects/tia/manyworld/gt.gif
    image_path: /assets/projects/tia/manyworld/gt.gif
    alt: "placeholder image 1"
  - url: /assets/projects/tia/manyworld/pred.gif
    image_path: /assets/projects/tia/manyworld/pred.gif
    alt: "placeholder image 2"
  - url: /assets/projects/tia/manyworld/joint.gif
    image_path: /assets/projects/tia/manyworld/joint.gif
    alt: "placeholder image 3"
  - url: /assets/projects/tia/manyworld/main.gif
    image_path: /assets/projects/tia/manyworld/main.gif
    alt: "placeholder image 4"
  - url: /assets/projects/tia/manyworld/disen.gif
    image_path: /assets/projects/tia/manyworld/disen.gif
    alt: "placeholder image 5"
---


<h1 align="center">
Learning Task Informed Abstractions
</h1>
<div class="post-date-header">June 2021</div>


<h4>
Abstract 
</h4>

Current model-based reinforcement learning methods struggle when operating from complex visual scenes due to their inability to prioritize task-relevant features. To mitigate this problem, we propose learning **Task Informed Abstractions** (TIA) that explicitly separates reward-correlated visual features from distractors. For learning TIA, we introduce the formalism of Task Informed MDP (TiMDP) that is realized by training two models that learn visual features via cooperative reconstruction, but one model is adversarially dissociated from the reward signal. Empirical evaluation shows that TIA leads to significant performance gains over state-of-the-art methods on many visual control tasks where natural and unconstrained visual distractions pose a formidable challenge. 

<h4>
Qualitative Results 
</h4>

{% include gallery class="fifth" caption="Top to Bottom: Cheetah Run, Hopper Hop, ManyWorld. Left to Right: (1) Raw Observation (2) Dreamer Reconstruction (3) TIA Joint Reconstruction (4) TIA Task Model Reconstruction (5) TIA Distractor Model Reconstruction. Dreamer does not distinguish task-relevant vs task-irrelevant information and mix the two in its state representation. In DMC domains, Dreamer tries to reconstruct background videos that it memorized during training. On the other hand, TIA disentangles the state space into a task stream and a distractor stream through reward, and is able to the task-relevant information much better than vanilla Dreamer."%}