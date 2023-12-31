# Human Activity Recognition(HAR) using body-worn sensors and Deep Learning

This repository contains some of the code I used on the development of my M.Sc. in Telecommunications Engineering' dissertation thesis a while ago (2020), and allowed me to write and present a research paper on the ASPAI'20 Conference (Advances in Signal Processing and Artificial Intelligence) called 'Deep learning model for upper-body action recognition using body-worn sensors'.

The idea behind this project is to classify different human activities such as walking, running, jumping, etc. using the signals from body-worn sensors. Specifically, these sensors were composed by accelerometers and magnetometers among others, but the dataset used, called REALDISP, also contained the quaternions calculated from these. Quaternions are hypercomlpex numbers that allows us to represent the body orientations in the 3 three dimensions, and are really useful when representing them with a parametrized skeleton, as I did.

However, not only the evolution of quaternions were used, but also their 2D-DFT (2D Discrete Fourier Transform) computed using the FFT (Fast Fourier Transform). This unusual feature engineering task in Deep Learning world remarkably helped to improve the performance of the network, outperforming state-of-the-art results.

In [this link]([url](https://www.researchgate.net/publication/344949079_Deep_learning_model_for_upper-body_action_recognition_using_body-worn_sensors)) you can find the full research paper in case you are interested in a more detailed and in-depth explanation. Additionally, in this git repository you will find some notebooks regarding GANs (Generative Adversarial Networks), whihc are not referrenced in the research paper. This is because they were only included in the MSc dissertation thesis, as it was also explored (introductory) the generation of human movements (quaternion signals) and their representation in a 3D Unity avatar, as it can be seen in this [YouTube video (Spanish)]([url](https://youtu.be/hxi8GaB1LDo?si=CNv7qOu-0QDtlMjm)https://youtu.be/hxi8GaB1LDo?si=CNv7qOu-0QDtlMjm).

The structure of the repository is as follows:
- 00 - data: Contains all the files from the dataset and the ones I generated in different ways.
- 01 - CLASSIFICATION: Neural networks (CNNS and CNN+RNNs) used for classification and their results.
- 02 - GANs: Generative Adversarial networks I tried for data augmentation.
- 03 - PREDICTION: Movements generation, this is, quaternions generation.
- 04 - Videos: The videos with 3D avatars for classification and generation at different stages.

PD: The notebooks are quite messy (sorry for that!). I am uploading them to this repository more than 3 years after I wrote them, so it is not easy to fix it. I will try to make them clean throughout the time. Thanks for understanding!
