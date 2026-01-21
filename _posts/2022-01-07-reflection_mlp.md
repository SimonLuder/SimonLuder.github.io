---
title: Multilayer Perceptron from Scratch
tags: [Algorithms, Machine Learning]
style: 
color: 
description: Implementation of a multilayer perceptron with python.
---

{% include elements/figure.html image="https://github.com/SimonLuder/SimonLuder.github.io/blob/main/pictures/mlp.png?raw=true" caption="" %}


As part of the foundations of machine learning study module, I was tasked with designing and implementing a custom Multilayer Perceptron (MLP) from scratch. The objective was to use this neural network to classify car brands based on structured features such as fuel capacity, vehicle price, and paint color. The implementation was required to be written in Python, with library usage restricted to NumPy and Pandas to ensure a strong focus on the underlying mechanics rather than high-level frameworks.

At the time, my experience with multilayer perceptrons and neural networks was quite limited. While I had previously implemented a single-layer perceptron, the scope and complexity of this task were significantly greater than anything I had worked on before.

The task specifications deliberately constrained the available methods. I suppose the idea behind this was that we could focus more on the actual implementation and didn't have to worry too much about the pros and cons of the different methods. For instance, optimization was required to be performed by implementing Gradient Descent, and the network had to employ the logistic sigmoid as its activation function. These constraints allowed to focus on correctly implementing and understanding the algorithmic foundations of an MLP without being distracted by design choices between alternative approaches.

During implementation, a number of challenges had to be faced. The biggest challenge for me was the implementation of the backpropagation and it was very rewarding when it finally worked. Although the final classification accuracy did not outperform simpler classification methods, i still leaned a lot from it.

Overall, the task of implementation turned out to be much more time-consuming than expected. However, this effort was worth it, as it improved my understanding of neural networks in general more than would have been possible with my previous training material on this topic.