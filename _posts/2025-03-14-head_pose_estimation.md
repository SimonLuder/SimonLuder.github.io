---
title: Head Pose Estimation
tags: [Computer Vision, OpenCV]
style: 
color: 
description: Implementation of head pose estimation with MediaPipe and OpenCV.
---

This work was carried out as part of the Werteorientierter Schweizer Roboter project at the Institute for Microcomputer Systems (IMVS). The project focuses on developing an assistive robot for retirement homes that can accompany residents to therapy sessions. A key objective is to enable safe and meaningful interaction between robots and humans in everyday care environments. To make this possible, the robot needs to be able to reliably recognize and identify people.

Modern face recognition systems typically operate by encoding a facial image into a compact numerical representation (embedding). This embedding captures distinctive facial features such that images of the same person are mapped close together in the embedding space, while images of different individuals are mapped farther apart. Identity matching is then performed by comparing distances between embeddings rather than raw images.

An interediate goal was to obtain multiple head poses per individual in order to enrich diverse reference points within the embedding space. Instead of relying on a single frontal image for identification, the system captures pictures of the face from multiple angles. This helps reduce errors caused by changes in pose or perspective that the face encoder model might not handle well. These pose-specific references help compensate for the representational gaps in the embedding model and leads to more stable identity matching under non-ideal and real-world conditions.

Head orientation can be estimated in real time using facial landmarks which allows reference images to be captured at different yaw, pitch, and roll angles. These pose-specific embeddings better represent how a face appears from multiple viewpoints, making the system more robust to changes in head rotation, camera alignment, and viewing perspective.

{% include elements/figure.html image="https://github.com/SimonLuder/SimonLuder.github.io/blob/main/pictures/pitch_yaw_roll.gif?raw=true"  caption="pitch, roll and yaw" %}


A simplified implementation of the used approach is available on my GitHub. The repository contains an example of real-time multi-face head pose estimation with visualized orientation axes, built using Python, OpenCV and MediaPipe.

<p class="text-center">
{% include elements/button.html link="https://github.com/SimonLuder/head_pose_estimation" text="Check it out on GitHub" %}
</p>