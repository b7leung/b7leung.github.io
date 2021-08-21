---
title: "Domain Adaptation for Real-World Single View 3D Reconstruction"
excerpt: "📅 **Jun. 2020 - Dec. 2020** • 📄 [Paper](https://b7leung.github.io/files/DA_For_SVR.pdf) <br/> Applied several domain adaptation techniques (MMD, Deep CORAL, DANN) to enable unsupervised transfer from CAD ShapeNet data to real world data, for the task of single view 3D reconstruction. [More info.](https://b7leung.github.io/projects/da-for-sv-reconstruction/) <br/><img src='/images/DA_For_SVR_Main_Picture.png'>"
collection: projects
redirect_from: 
  - /projects/da-for-sv-reconstruction/
---

📅 **Jun. 2020 - Dec. 2020** • 📄 [Paper](https://b7leung.github.io/files/DA_For_SVR.pdf) • <img src="/images/github_icon.png" width="20" height="20"> [Github](https://github.com/b7leung/Domain-Adaptation-Single-View-Reconstruction)

<img src='/images/DA_For_SVR_Main_Picture.png'>

Deep learning-based object reconstruction algorithms
have shown remarkable improvements over classical methods. However, supervised learning based methods perform
poorly when the training data and the test data have different distributions. Indeed, most current works perform
satisfactorily on the synthetic ShapeNet dataset, but dramatically fail in when presented with real world images. To
address this issue, unsupervised domain adaptation can be
used transfer knowledge from the label