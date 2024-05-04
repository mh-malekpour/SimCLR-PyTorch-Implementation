# SimCLR PyTorch Implementation

This project is part of the IFT 6135B - H2024 course under Prof. Aaron Courville. This repository contains a PyTorch implementation of the self-supervised contrastive learning algorithm, SimCLR. The goal is to apply SimCLR on the [STL-10 dataset](https://cs.stanford.edu/~acoates/stl10/), although the training duration is limited to 70 epochs due to resource constraints.

## Self-supervised Learning: SimCLR

SimCLR (Simple Contrastive Learning of Visual Representations) is a self-supervised learning framework for learning visual representations from unlabeled data. It follows the principles of self-supervised learning:
1. Design an auxiliary task.
2. Train the base network on the auxiliary task.
3. Evaluate on the downstream task: Train a new decoder based on the trained encoder.

SimCLR maximizes agreement between differently augmented views of the same image and minimizes agreement between views of different images. This is achieved through a contrastive loss function that encourages the model to learn representations that are invariant to transformations while maintaining discriminative information.

For more details, refer to the main paper: [SimCLR: A Simple Framework for Contrastive Learning of Visual Representations](https://arxiv.org/abs/2002.05709).

![SimCLR Overview](https://camo.githubusercontent.com/35af3432fbe91c56a934b5ee58931b4848ab35043830c9dd6f08fa41e6eadbe7/68747470733a2f2f312e62702e626c6f6773706f742e636f6d2f2d2d764834504b704539596f2f586f3461324259657276492f414141414141414146704d2f766146447750584f79416f6b4143385868383532447a4f67457332324e68625877434c63424741735948512f73313630302f696d616765342e676966)

Thank you for your interest in this SimCLR implementation!
