---
title: "Review and Unification of Current Unsupervised Domain Adaptation Methods"
excerpt: "📅 **Jul. 2020 - Nov. 2020** • 🔎[More Info](https://b7leung.github.io/projects/unsupervised_DA_review) • 📄 [Report](https://b7leung.github.io/files/Unsupervised_Domain_Adaptation.pdf) <br/> Proposes a unified taxonomy to generalize most of the current methods in unsupervised domain adaptation. Also takes a deep look into Contrastive Adaptation Networks, and ways to improve performance. <br/><img src='/images/da_review_main_picture.jpg'>"
collection: projects
redirect_from: 
  - /projects/unsupervised_DA_review/
---

📅 **Jul. 2020 - Nov. 2020** • 📄 [Report](https://b7leung.github.io/files/Unsupervised_Domain_Adaptation.pdf)

<img src='/images/da_review_main_picture.jpg'>

In supervised machine learning, a common paradigm is to use labeled data (the “training set”) to learn the weights of some model, and deploy it to unseen data at test time. Unfortunately, this is not always realistic in practice, because **labeled data can be hard to obtain**. Thus, we often find ourselves in a situation where we don’t have labeled data in the distribution we’re actually interested in (called the test distribution). In the test distribution, we only have **unlabeled data**. However, we do have labeled data in a similar distribution (called the **target distribution**). Note that there might be a gap between these two domains, and that some adaptation needs to occur for optimal performance.

In this project a survey of current methods in the **unsupervised domain adaptation** literature is performed, and a **unified taxonomy is proposed** to generalize the methods within one framework. A critical analysis is also taken at **Contrastive Adaptation Network (CAN)**, one of the state-of-the-art method which utilizes psuedolabels. Recommendations are made with regards to CAN, to further improve performance beyond what is stated by the original authors. For details, please refer to the full [report](https://b7leung.github.io/files/Unsupervised_Domain_Adaptation.pdf).


<figure>
  <img src="/images/da.png" >
  <figcaption>Some example unsupervised domain adaptation methods that are surveyed. From top to bottom: Deep CORAL, Contrastive Adaptation Networks, Domain Adversarial Neural Networks.</figcaption>
</figure>
