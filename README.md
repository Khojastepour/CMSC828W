# CMSC828W Project
Stationarity of Crucial Gradients in Deep Neural Networks
\\ Modern deep learning models trained under federated learning setting contain hundreds of millions of parameters. This leads to considerable storage space consumption on mobile systems, and  significant communication bandwidth requirements for exchanging gradients between edge devices and central server. Recently many pruning methods attempting to learn a sparse model have been suggested to tackle the memory concerns. To control the communication overhead, many gradient sparsification techniques have been suggested based on the sparse distribution of local gradients vectors. Such sparsification techniques like top-k and rTop-k transmit only few large-magnitude gradients, referred to in this paper as the "crucial gradients". Our work aims to connect the model pruning literature and gradient sparsfication literature, by making the important observation that the positions of crucial gradients in deep neural networks is static, which leads to bulk of the model parameters never getting updated under such sparsification techniques. We apply this observation to MNIST image classifiers to prune up to 99\% network, causing considerable reduction in storage space requirement. We also study the tradeoff between exploration and  exploitation in large gradient vectors for obtaining high model accuracy. Numerical experiments show that our pruning approach does not damage the final accuracy of the global model under top-k and rTop-k sparsification techniques.
