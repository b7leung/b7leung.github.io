---
title: "Domain Adaptation for Real-World Single View 3D Reconstruction"
excerpt: "📅 **Jun. 2020 - Dec. 2020** • 🔎[More Info](https://b7leung.github.io/projects/da-for-sv-reconstruction/) • 📄 [Paper](http://arxiv.org/pdf/2108.10972.pdf) <br/> Studies the application of several domain adaptation techniques (MMD, Deep CORAL, DANN) to enable unsupervised transfer from CAD ShapeNet data to real world data, for the task of single view 3D reconstruction. <br/><img src='/images/DA_For_SVR_Main_Picture.png'>"
collection: projects
redirect_from: 
  - /projects/da-for-sv-reconstruction/
---

📅 **Jun. 2020 - Dec. 2020** • 📄 [Paper](http://arxiv.org/pdf/2108.10972.pdf) • <img src="/images/github_icon.png" width="20" height="20"> [Github](https://github.com/b7leung/Domain-Adaptation-Single-View-Reconstruction)

<figure>
  <img src="/images/DA_For_SVR_Main_Picture.png" >
  <figcaption>The proposed architecture, which is based off the pix2vox framework. We provide two additions: 1) incorporating domain adaptation in the style of DANN through a domain classifier and a gradient reversal layer, and 2) since we have classification labels for both the source and target domain, we also classify the produced voxel.</figcaption>
</figure>

In this project, several **unsupervised domain adaptation** methods were applied to the task of **single view 3D reconstruction**, including MMD, Deep CORAL, and DANN. The source domain is ShapeNet which is synthetic, while the target domain is OOWL which is in the real domain (I helped design OOWL, see [here](https://b7leung.github.io/projects/drone-flight-dataset/) for more details). Overall, we found that our proposed **DANN with a multitask learning voxel classification branch** led to the best results. For details, please refer to the [paper](http://arxiv.org/pdf/2108.10972.pdf).


<figure>
  <img src="/images/da_svr/oowl.png" >
  <figcaption>An example object (lamp) from datasets used for our project. OWILD, OOWL, and OOWLSeg are part of the ODDS dataset, and are real. Meanwhile, ShapeNet is synthetic.</figcaption>
</figure>

<figure>
  <img src="/images/da_svr/qual.png" >
  <figcaption>Reconstruction results when domain adaptation is used with OOWL as the target domain. We compare domain adaptation using Deep CORAL, DANN, and our proposed architecture (DANN + Voxel Classify).</figcaption>
</figure>

<figure>
  <img src="/images/da_svr/tsne.png" >
  <figcaption>Learned feature map embeddings visualized with t-SNE. Purple denotes the source domain (ShapeNet), yellow denotes the target domain (OOWL). On the left we show the result when domain adaptation is not used. On the center and right, we show results achieved by applying domain adaptation (DANN or CORAL) to the vanilla pix2vox model.</figcaption>
</figure>


Citation Info
======

_**Leung, B.**, Singh, S., & Horodniceanu, A. (2020). Domain adaptation for real-world single view 3d reconstruction. ArXiv:2108.10972 [Cs]. http://arxiv.org/abs/2108.10972_


