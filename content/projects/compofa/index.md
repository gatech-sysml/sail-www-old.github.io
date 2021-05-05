---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "CompOFA: Compound Once-For-All Networks for Faster Multi-Platform Deployment"
subtitle: "At International Conference on Learning Representations (ICLR), 2021"
summary: "CompOFA improves the speed, cost, and usability of jointly training models for many deployment targets. By highlighting insights on model design and system deployment, we try to address an important problem for real-world usability of DNNs."
authors:
- manas
- shreya 
- alind
- alexey
# tags: []
# categories: []
date: 2021-04-24T15:55:22-04:00

# Optional external URL for project (replaces project detail page).
# external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Custom links (optional).
links:
- name: ICLR 2021
  url: "https://iclr.cc/virtual/2021/poster/3296"
  icon_pack: fas
  icon: globe

- name: ArXiv
  url: "https://arxiv.org/abs/2104.12642"
  icon_pack: ai
  icon: arxiv

- name: GitHub
  url: "https://github.com/gatech-sysml/compofa"
  icon_pack: fab
  icon: github

- name: Poster
  url: "https://iclr.cc/media/PosterPDFs/ICLR%202021/2c3ddf4bf13852db711dd1901fb517fa.png"
  icon_pack: fas
  icon: image

- name: Video
  url: "https://youtu.be/DAi20CfDCfg"
  icon_pack: fas
  icon: film

- name: Blog
  url: "/post/compofa"
  icon_pack: fas
  icon: newspaper

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

commentable: false
---

{{<figure src="./img/overview.png" width="100%" caption="Conventional training, current SOTA, and CompOFA">}}

The emergence of CNNs in mainstream deployment has necessitated methods to design and train efficient architectures tailored to maximize the accuracy under diverse hardware & latency constraints.


Designing and training DNN architectures for each deployment target is not feasible. Each deployment costs training time, compute dollars, system expertise, ML expertise, CO2 emissions.

In *CompOFA*, we propose a cost-effective and faster technique to build model families that support multiple deployment platforms. Using insights from model design and system deployment, we build upon the current best methods that take 40-50 GPU days of computation and make their training and searching processes **faster by 2x and 200x**, respectively – all while building a family of equally efficient and diverse models!

### CompOFA matches efficiency and diversity of SOTA methods...

{{<figure src="./img/pareto-results.png" caption="Efficient model families for diverse hardwares -- from mobile phones to GPUs">}}

### ...with *2x* faster training and *216x* faster searching

{{<figure src="./img/table.png" width="40%">}}

### Better overall average accuracy
At a population level, CompOFA has a higher concentration of accurate models

{{<figure src="./img/avg_accuracy.png" width="70%">}}

# Learn more

Please check out our [paper](https://arxiv.org/abs/2104.12642) and [poster](https://iclr.cc/media/PosterPDFs/ICLR%202021/2c3ddf4bf13852db711dd1901fb517fa.png) at ICLR 2021! Our code and pretrained models are also available on our [Github repository](https://github.com/gatech-sysml/compofa). Also check out our [blog post](/compofa/blog)!

## Citation

```bibtex
@inproceedings{compofa-iclr21,
  author    = {Manas Sahni and Shreya Varshini and Alind Khare and
               Alexey Tumanov},
  title     = {{C}omp{OFA}: Compound Once-For-All Networks for Faster Multi-Platform Deployment},
  month     = {May},
  booktitle = {Proc. of the 9th International Conference on Learning Representations},
  series = {ICLR '21},
  year = {2021},
  url       = {https://openreview.net/forum?id=IgIk8RRT-Z}
}
```
