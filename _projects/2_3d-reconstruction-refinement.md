---
title: "Refining Single View 3D Reconstructions with Self-Supervised Machine Learning"
excerpt: "📅 **Jan. 2021 - Present** • 🔎[More Info](https://b7leung.github.io/projects/3d-reconstruction-refinement/) • 📄 [Paper](https://arxiv.org/pdf/2108.09911.pdf) <br/> A novel neural network refinement algorithm to generate 3D meshes from a single image. Used self-supervised learning & symmetry regularization; beats state-of-the-art (up to 47%), across many datasets. <br/><img src='/images/REFINE_Main_Picture.png'>"
collection: projects
redirect_from: 
  - /projects/3d-reconstruction-refinement/
---

📅 **Jan. 2021 - Present** • 📄 [Paper](https://arxiv.org/pdf/2108.09911.pdf) • <img src="/images/github_icon.png" width="20" height="20"> [Github](https://github.com/b7leung/3D-Mesh-REFINEment)

<img src='/images/REFINE_Main_Picture.png'>

This project proposes a novel neural network **refinement algorithm and paradigm to improve 3D mesh reconstructions** from any single-view reconstruction method. This is done by using **self-supervised learning** to exploit the silhouette of the input image, encouraging consistency between the mesh and the given object view by differentiable 3D rendering. In addition, several **symmetry** based losses are introduced to regularize the refinement. The use of the refinement at test time **beats state-of-the-art (up to 47%), across many datasets, metrics, and object classes**. The refinement step that can be easily integrated into the pipeline of any black-box method in the literature. Python, PyTorch, and PyTorch 3D are extensively used. For more details, please refer to the [full paper](https://arxiv.org/pdf/2108.09911.pdf).

<figure>
  <img src="/images/REFINE/refine_qual.png">
  <figcaption>Example mesh REFINEments for Pix3D dataset.</figcaption>
</figure>

<figure>
  <img src="/images/REFINE/refine_arch.png" width="50" height="50" >
  <figcaption>Refinement architecture.</figcaption>
</figure>

<figure>
  <img src="/images/REFINE/refine_quant.png" >
  <figcaption>Quantative results on the Pix3D dataset.</figcaption>
</figure>


Citation Info
======

_**Leung, B.**, Ho, C.H., & Vasconcelos, N. (2022). Black-box test-time shape refinement for single view 3d reconstruction. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshop on Learning with Limited Labelled Data_