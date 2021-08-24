---
title: "Refining Single View 3D Reconstructions with Self-Supervised Machine Learning"
excerpt: "📅 **Jan. 2021 - Present** • 🔎[More Info](https://b7leung.github.io/projects/3d-reconstruction-refinement/) • 📄 [Paper](https://arxiv.org/pdf/2108.09911.pdf) <br/> Developed a novel neural network refinement algorithm to generate 3D meshes from a single image. Used self-supervised learning & symmetry regularization; beats state-of-the-art (up to 47%), across many datasets. <br/><img src='/images/REFINE_Main_Picture.png'>"
collection: projects
redirect_from: 
  - /projects/3d-reconstruction-refinement/
---

📅 **Jan. 2021 - Present** • 📄 [Paper](https://arxiv.org/pdf/2108.09911.pdf) • <img src="/images/github_icon.png" width="20" height="20"> [Github](https://github.com/b7leung/3D-Mesh-REFINEment)

<img src='/images/REFINE_Main_Picture.png'>

This project proposes a novel neural network **refinement algorithm to improve 3D mesh reconstructions** from any single-view reconstruction method. This is done by using **self-supervised learning** exploiting the silhouette of the input image, realized by differentiable 3D rendering. In addition, several **symmetry** based losses are introduced to regularize the refinement. The use of the refinement **beats state-of-the-art (up to 47%), across many datasets, metrics, and object classes**. Python, PyTorch, and PyTorch 3D are extensively used. For more details, please refer to the [full paper](https://arxiv.org/pdf/2108.09911.pdf).


**Abstract:** Much recent progress has been made in reconstructing the 3D shape of an object from an image of it, i.e. single view 3D reconstruction. However, it has been suggested that current methods simply adopt a “nearest-neighbor” strategy, instead of genuinely understanding the shape behind the input image. In this paper, we rigorously show that for many state of the art methods, this issue manifests as (1) inconsistencies between coarse reconstructions and input images, and (2) inability to generalize across domains. We thus propose REFINE, a postprocessing mesh refinement step that can be easily integrated into the pipeline of any black-box method in the literature. At test time, REFINE optimizes a network per mesh instance, to encourage consistency between the mesh and the given object view. This, along with a novel combination of regularizing losses, reduces the domain gap and achieves state of the art performance. We believe that this novel paradigm is an important step towards robust, accurate reconstructions, remaining relevant as new reconstruction networks are introduced.


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

_Leung, B., Ho, C.-H., & Vasconcelos, N. (2021). Black-box test-time shape refinement for single view 3d reconstruction. ArXiv:2108.09911 [Cs]. http://arxiv.org/abs/2108.09911_
