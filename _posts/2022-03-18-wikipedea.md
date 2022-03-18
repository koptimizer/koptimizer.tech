---
layout: post
read_time: true
show_date: true
title: "Paper Review - Can Wikipedia Help Offline Reinforcement Learning?"
date: 2022-03-18
img: posts/20220318/main.png
tags: [Reinforcement Learning, Machine Learning, Paper Review]
category: opinion
author: Koptimizer
description: "Fine-tuning reinforcement learning (RL) models has been challenging because of a lack of large scale off-the-shelf datasets as well as high variance in transferability among different environments."
---
22년 3월 기준으로 최신 RL 논문 중 가장 충격적인 논문을 한 편 뽑으라고 하면 단언코 이 논문을 고를 수 있을 것이다.

can wikipedia help offline reinforcement learning?

abstract
```
Fine-tuning reinforcement learning (RL) models has been challenging because of a lack of large scale off-the-shelf datasets as well as high variance in transferability among different environments. Recent work has looked at tackling offline RL from the perspective of sequence modeling with improved results as result of the introduction of the Transformer architecture. However, when the model is trained from scratch, it suffers from slow convergence speeds. In this paper, we look to take advantage of this formulation of reinforcement learning as sequence modeling and investigate the transferability of pre-trained sequence models on other domains (vision, language) when finetuned on offline RL tasks (control, games). To this end, we also propose techniques to improve transfer between these domains. Results show consistent performance gains in terms of both convergence speed and reward on a variety of environments, accelerating training by 3-6x and achieving state-of-the-art performance in a variety of tasks using Wikipedia-pretrained and GPT2 language models. We hope that this work not only brings light to the potentials of leveraging generic sequence modeling techniques and pre-trained models for RL, but also inspires future work on sharing knowledge between generative modeling tasks of completely different domains.
```

작성중

