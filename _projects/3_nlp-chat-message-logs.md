---
title: "Statistical Linguistic Analysis for User Chat Message Logs"
excerpt: "📅 **Feb. 2021 - Jul. 2021** • 🔎[More Info](https://b7leung.github.io/projects/nlp-chat-message-logs/) • 📰 [Slides](https://docs.google.com/presentation/d/1535V6VRLe-EIapHYMRdnkyu12eVziLMKEp6QLmh0_8M/edit#slide=id.p) <br/> An interactive dashboard to analyze user chat logs and describe their linguistic behavior. NLP transformer models (RoBERTa, GPT-2) are utilized for sentiment analysis, clustering, style transfer, & generative modeling. <br/><img src='/images/nlp_chat_logs_Main_Picture.png'>"
collection: projects
redirect_from: 
  - /projects/nlp-chat-message-logs/
---

📅 **Feb. 2021 - Jul. 2021** • 📰 [Slides](https://docs.google.com/presentation/d/1535V6VRLe-EIapHYMRdnkyu12eVziLMKEp6QLmh0_8M/edit#slide=id.p) • <img src="/images/github_icon.png" width="20" height="20"> [Github](https://github.com/b7leung/Chat-Log-Statistical-Linguistic-Analysis)

<img src='/images/nlp_chat_logs_Main_Picture.png'>

In this project, I worked in a group of 5 to develop an **interactive dashboard** to **analyze user chat logs** and describe their linguistic behavior. It is meant for smaller companies and organizations to easily understand the **linguistic patterns** of their user base. Many applications are integrated with social chatting systems, including video games, dating apps, and social media. With this dashboard, even verbose chatters with thousands of logged chat messages can be summarized, evaluated, and compared with other users at a glance. Then, downstream use cases include flagging/suspending/banning toxic users, recommending advertisements or posts to users, and even using their “virtual” chatbot counterpart to predict their behavior to new inputs. The dashboard is powered with Jupyter Notebooks and Voilà, tested with pytest, documented with Sphinx, and deployed using AWS (EC2 and S3).

I mainly worked on the UI, deployment, and generative modeling. The generative modeling utilizes the [BlenderBot](https://arxiv.org/pdf/2004.13637.pdf) chatbot , along with [unsupervised style transfer](https://arxiv.org/pdf/2010.05700.pdf) based on a Seq2Seq Transformer from Krishna Et. al. As a proof of concept, a [Discord chat](https://www.kaggle.com/jef1056/discord-data) dataset was used.


<figure>
  <img src="/images/NLP_suite/deployment_arch.png" >
  <figcaption>The deployment architecture for the dashboard.</figcaption>
</figure>

<figure>
  <img src="/images/NLP_suite/example_chat.png" >
  <figcaption>Example generative modeling from the stylized chatbot.</figcaption>
</figure>
