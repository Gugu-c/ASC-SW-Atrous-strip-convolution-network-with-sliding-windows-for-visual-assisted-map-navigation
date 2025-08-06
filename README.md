# ASC SW Atrous strip convolution network with sliding windows for visual assisted map navigation
Paper link: https://arxiv.org/abs/2507.12744

Abstract

With the rapid development of lightweight visual neural network architectures, traditional high-performance vision models have undergone significant compression, greatly improving their computational efficiency and energy consumption ratio. This makes them feasible for deployment on resource-constrained edge computing devices.

We propose a visual-assisted navigation framework called Atrous Strip Convolution–Sliding Window (ASC-SW), which leverages a depth camera and a lightweight visual neural network to assist map-based mobile robot navigation. This framework compensates for the inability of traditional light detection and range (LiDAR) sensors to detect ground-level obstacles such as ground-level wires.
We introduce a lightweight and efficient segmentation model, Atrous Strip Convolution Network (ASCnet), for detecting deformable linear objects (DLOs). MobileNetV2 is used as the backbone network, and Atrous Strip Convolution Spatial Pyramid Pooling (ASCSPP) is designed to extract DLO features more effectively. Atrous Strip Convolution is integrated into ASCSPP to accurately identify the linear structure of DLOs with low computational cost.

Additionally, a Sliding Window (SW) post-processing module is proposed to denoise the output in complex environments, improving recognition accuracy.

Our method strikes a balance between inference speed and segmentation performance. It achieves a mean Intersection over Union (Miou) score of 75.3\% on a self-built dataset and reaches 9.3 FPS inference speed on the Jetson Orin Nano edge device. Overall, our approach outperforms existing DLO detection models and has been successfully validated on a physical robotic platform.

The demostration is as followed:

![demo.gif](https://github.com/Gugu-c/ASC-SW-Atrous-strip-convolution-network-with-sliding-windows-for-visual-assisted-map-navigation/blob/main/asc-sw.gif)
