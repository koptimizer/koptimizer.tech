---
layout: post
read_time: true
show_date: true
title: "Particle Swarm Optimization"
date: 2022-03-18
img: posts/20220318/main2.jpg
tags: [Metaheuristic]
category: review
author: Koptimizer
description: "입자 군집 최적화"
mathjax: yes
---

입자 군집 최적화(particle swarm optimization)는 [Kennedy and Ebergart(1995)](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=488968&casa_token=sAtJffqCtHcAAAAA:Zrxnhv4yrmgdc0P6R61_ebomVMzFXcR0pYounK8SqDT2lvat2OYq8KGuaANbDhCobhdaH2b8LQ&tag=1)에서 제안되었으며, 새나 벌레 등이 무리를 지어 행동하는 패턴에서 착안된 메타휴리스틱 알고리즘이다. 이하 PSO라고 표현하겠다.

메타휴리스틱은 [다른 글]()에서도 설명했듯이, 자연이나 물리법칙에서 발견되는 "크고 아름다운 현상"들을 기저로 한다. PSO에서 사용되는 크고 아름다운 현상이란 무엇일까? 우리 함께 한국의 대표적인 도시형 조류, 비둘기 무리를 생각해보자. 보통 다음과 같을 것이다.
<center><img src = "./assets/img/posts/20220318/pig.jpg"></center>

비둘기 무리는 왜 이렇게 역전에 모여드는 것일까? 비둘기는 원래 절벽에서 서식하는 동물이다. 역전은 보통 탁 트인 광장과 약간의 녹지를 함께 가지고 있고, 주변에는 상권이 발달하여 높은 건물이 많다. 유동인구도 많으므로 쓰레기가 많이 발생하여 비둘기가 간접적으로 먹이를 획득할 가능성도 높다. 비둘기에게는 적절한 서식지인 것이다.

그렇다면 비둘기는 서로 말을 할줄 아는 것도 아닌데 어떻게 역전에 집결하는 것일까? 새들은 생존을 위한 진화로 무리를 형성하게 되었기 때문에 개인의 행동이 무리 전체에 영향을 끼친다. 비둘기 무리 옆에서 땅을 발로 꽝 박차면 가장 가까운 곳에 있던 비둘기부터 하나 둘씩 날아올라 모든 비둘기가 날아오른다. 각각의 비둘기는 내 주변의 많은 비둘기 형제가 급하게 날아올랐으니 위험한 상황이 발생했다고 생각하고 날아오른 것인데, 이것이 연쇄적으로 발생하여 모든 비둘기가 날아오르게 한 것이다. 역전에 집결할 수 있었던 것 또한, 서식지로 적합한 환경을 찾아 도착한 일부 비둘기들 때문에 다른 비둘기도 모여들게 되었고, 결과적으로 역전에 이 세상 모든 비둘기가 모인 것 같은 모습이 된 것이다. 

PSO는 이처럼 개인(particle)과 무리(swarm) 상호작용을 이용하여 최적해를 찾아나가는 방법이다. PSO의 장점은 군집 지능(swarm intelligence)에서 발현되는 강력한 수렴력을 지녔으면서 지역 최적해의 교착을 피할 수 있기 때문이다. 

이제 PSO는 어떻게 작동되는 것인지, 어떻게 쓰이는 것인지 심층적으로 살펴보자.

## 어떻게 작동하는가?

단일의 해 x_i로 이루어진 해집합 \P


