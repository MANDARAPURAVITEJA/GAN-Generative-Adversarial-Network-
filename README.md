# GAN - Generative Adversarial Network
### Definition:
A Generative Adversarial Network (GAN) is a deep learning architecture that consists of two neural networks competing against each other in a zero-sum game framework. The goal of GANs is to generate new, synthetic data that resembles some known data distribution.

### How do GANs work?
Generative Adversarial Networks (GANs) can be broken down into three parts:
* Generative: To learn a generative model, which describes how data is generated in terms of a probabilistic model.
* Adversarial: The training of a model is done in an adversarial setting.
* Networks: Use deep neural networks as artificial intelligence (AI) algorithms for training purposes.

In GANs, there is a Generator and a Discriminator. The Generator generates fake samples of data(be it an image, audio, etc.) and tries to fool the Discriminator. The Discriminator, on the other hand, tries to distinguish between the real and fake samples. The Generator and the Discriminator are both Neural Networks and they both run in competition with each other in the training phase. The steps are repeated several times and in this, the Generator and Discriminator get better and better in their respective jobs after each repetition. The work can be visualized by the diagram given below: 

![image](https://github.com/MANDARAPURAVITEJA/GAN-Generative-Adversarial-Network-/assets/63329006/d5ff4f51-748c-4c81-b57b-efccae8e56f0)

### Generator Model
The Generator is trained while the Discriminator is idle. After the Discriminator is trained by the generated fake data of the Generator, we can get its predictions and use the results for training the Generator and get better from the previous state to try and fool the Discriminator.

### Discriminator Model
The Discriminator is trained while the Generator is idle. In this phase, the network is only forward propagated and no back-propagation is done. The Discriminator is trained on real data for n epochs and sees if it can correctly predict them as real. Also, in this phase, the Discriminator is also trained on the fake generated data from the Generator and see if it can correctly predict them as fake.
