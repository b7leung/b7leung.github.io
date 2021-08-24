---
title: "Drone Flight Dataset for Neural Network Classification Robustness"
excerpt: "📅 **Sep. 2018 - Present** • 🔎[More Info](https://b7leung.github.io/projects/drone-flight-dataset/) • 📄 [CVPR Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Ho_Catastrophic_Childs_Play_Easy_to_Perform_Hard_to_Defend_Adversarial_CVPR_2019_paper.pdf) • 🌐 [Main Website](http://www.svcl.ucsd.edu/projects/OOWL/CVPR2019_adversarial.html) <br/> A **drone flight system** to collect over 120,000 images. The dataset was used to conduct experiments showing severe vulnerabilities (30% drop) in neural networks to pose & camera shake. Findings published to CVPR 2019. <br/><img src='/images/OOWL_Main_Picture.jpg'>"
collection: projects
redirect_from: 
  - /projects/drone-flight-dataset/
---

📅 **Sep. 2018 - Present** • 📄 [CVPR Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Ho_Catastrophic_Childs_Play_Easy_to_Perform_Hard_to_Defend_Adversarial_CVPR_2019_paper.pdf) • 📄 [Dataset Paper](https://b7leung.github.io/files/OOWL_Dataset.pdf) • 📄 [Drone Algorithm Info](https://docs.google.com/presentation/d/15NlP05SLmo0Nyx40LU_9Uzq4h6xHTv1L-L0a8x-TYOY/edit?usp=sharing) <br/> 📄 [Poster](https://b7leung.github.io/files/cvpr19_adversarial_poster_final.pdf) • 🌐 [Main Website](http://www.svcl.ucsd.edu/projects/OOWL/CVPR2019_adversarial.html) • <img src="/images/github_icon.png" width="20" height="20"> [Github](https://github.com/b7leung/OOWL-Drone-Flight-System)



<figure>
  <img src='/images/OOWL_Main_Picture.jpg'>
  <figcaption>Left: The drone collecting images. Center: Example object from the phone class, in two different domains: in the lab, and in the wild. Right: Example of drone camera shake.</figcaption>
</figure>

In this project, I was the leader and main developer of a novel **drone flight system**, using the Parrot AR.Drone Quadricopter. With Python, OpenCV, and ROS, I used the **drone's low-level API, computer/machine vision techniques, and PID controls** to enable a new “in the lab“ data collection infrastructure is proposed consisting of a drone which captures images as it circles around objects. It's inexpensive and easily replicable nature may also potentially lead to a scalable data collection effort by the computer vision community. The procedure's usefulness is demonstrated by creating a **multiview image dataset of Objects Obtained With fLight (OOWL)**. Currently, OOWL contains 120,000 images of 500 objects and is the largest “in the lab“ image dataset available when both number of classes and objects per class are considered. Additional images were also obtained by placing the objects in real-world locations, enabling **multiple domains** to be studied.

The OOWL dataset was then used to study the robustness of modern neural network classification, in our [first dataset paper](https://b7leung.github.io/files/OOWL_Dataset.pdf). In particular, the hypothesis is that training on standard datasets like ImageNet can produce can produce **biased object recognizers**, e.g. preferring professional photography or certain viewing angles. With PyTorch, I helped conduct experiments which show that indeed, neural networks like ResNet, AlexNet, and VGG show severe vulnerabilities to pose & camera shake. This can also be framed as a type of semantic adversarial attack, as shown in our [second paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Ho_Catastrophic_Childs_Play_Easy_to_Perform_Hard_to_Defend_Adversarial_CVPR_2019_paper.pdf) (published to CVPR 2019). Instead of using the standard l2-norm, Amazon Mechanical Turk was used to annotate "indistingushable" images based on **human perception**.


<figure>
  <img src="/images/oowl_obj_example.png" width="50" height="50" >
  <figcaption>An example object from the dataset's lamp class.</figcaption>
</figure>

<figure>
  <img src="/images/oowl_dataset_compare.png" width="50" height="50" >
  <figcaption>A comparision with other datasets in the literature. Green are multiview, while red are not. Purple denotes a synthetic CAD dataset.</figcaption>
</figure>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/WdvkxDUGUz0?controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br/>

Citation Info
======

_Leung, B., Ho, C. H., Sandstrom, E., Chang, Y., & Vasconcelos, N. (2019). Catastrophic child's play: Easy to perform, hard to defend adversarial attacks. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (pp. 9229-9237)._

_Leung, B., Ho, C. H., Persekian, A., Orozco, D., Sandstrom, E., Chang, Y., & Vasconcelos, N. (2019). OOWL500: Overcoming Dataset Collection Bias in the Wild._