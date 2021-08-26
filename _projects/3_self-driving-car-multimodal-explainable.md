---
title: "Self-Driving Cars using 2D/3D Action and Explanation Prediction"
excerpt: "📅 **Feb. 2021 - Present** • 🔎[More Info](https://b7leung.github.io/projects/self-driving-car-multimodal-explainable/)<br/> A neural network model currently in development for self-driving cars. Utilizes multimodal fusion with 2D images and 3D pointclouds to predict navigation actions. Additionally, 2D and 3D explanations are jointly predicted to provide intuitive explanations for model decisions. <br/><img src='/images/av_main_picture.png'>"
collection: projects
redirect_from: 
  - /projects/self-driving-car-multimodal-explainable/
---

📅 **Feb. 2021 - Present**

<img src='/images/av_main_picture.png'>

A currently ongoing project, where I am guiding the formulation and development of a new **neural network model for autonomous vehicle navigation**. Both **2D images** and **3D pointclouds** are utilized through **multimodal fusion**, to predict **actions** (such as move foward, turn left, etc). Unlike other methods in the literature however, we also predict intuitive **explanations** for these actions (such as "clear road" or "blocking object: pedestrian"). Furthermore, 2D and 3D detected bounding boxes (from Faster R-CNN and MVX-Net) are also provided to indicate specific **action-induced objects in 2D and 3D**. Annotations on Amazon Mechanical Turk are also currently being collected for action and explanation labels, to add to the [Waymo Open dataset](https://waymo.com/open/).

<figure>
  <img src="/images/AV/av1.png">
  <figcaption>A high level illustration of an approach we are experimenting with, utilizing SampleNet to choose action induced points.</figcaption>
</figure>

<figure>
  <img src="/images/AV/av2.png">
  <figcaption>A different approach we are also experimenting with, using a single multimodal selector.</figcaption>
</figure>

_Collaborators on this project: Arth Dharaskar, Allen Cheung, Chih-Hui Ho, Tz-Ying Wu._