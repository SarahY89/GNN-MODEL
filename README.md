# GNN-MODEL
A bit of technical background on an AI compiler will help you get started! An AI model can be represented as a graph, where a node is a tensor operation (e.g. matrix multiplication, convolution, etc), and an edge represents a tensor. A compilation configuration controls how the compiler transforms the graph for a specific optimization pass. In particular, Alice can control two types of configurations/optimizations:

A layout configuration control how tensors in the graph are laid out in the physical memory, by specifying the dimension order of each input and output of an operation node.
A tile configuration controls the tile size of each fused subgraph.

![image](https://github.com/SarahY89/GNN-MODEL/assets/92030964/c1901df6-3d6d-434c-ac20-368f2374a0a4)


![image](https://github.com/SarahY89/GNN-MODEL/assets/92030964/98a301e4-b0cb-4ec9-8f99-442b22e52eb3)



Being able to predict an optimal configuration for a given graph will not only help Alice's team but also improve the compiler's heuristic to select the best configuration without human's intervention. This will make AI models run more efficiently, consuming less time and resources overall!

In this competition, your aim is to train a machine learning model based on the runtime data provided to you in the training dataset and further predict the runtime of graphs and configurations in the test dataset.
