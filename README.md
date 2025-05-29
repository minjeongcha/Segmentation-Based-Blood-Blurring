# Segmentation-Based-Blood-Blurring
Segmentation-Based Blood Blurring: Examining Eye-Response Differences in Gory Video Viewing

<p align="">
    <h3>
        | <a href="https://doi.org/10.3390/s25072093" target="_blank"><b>Paper</b></a> |
    </h3>
</p>

**Segmentation-Based Blood Blurring** is a novel video processing technique that selectively blurs blood-related content based on semantic segmentation. This approach is designed to reduce viewer discomfort during gory video viewing, and our study evaluates its effectiveness using eye-tracking data.

This repository contains the full code and dataset used in our paper:

**Son, J.; Cha, M.; Park, S. Segmentation-Based Blood Blurring: Examining Eye-Response Differences in Gory Video Viewing.** *Sensors 2025, 25, 2093.*  
[https://doi.org/10.3390/s25072093](https://doi.org/10.3390/s25072093)

<p align="center">
  <img src="./assets/teaser.png" alt="Segmentation-Based Blood Blurring Teaser" width="100%">
</p>

---

## 🧪 What is Blood Blurring?

We propose a **segmentation-based filtering approach** to detect and blur only blood regions in videos. By leveraging semantic segmentation models, we ensure that non-violent parts remain untouched. The goal is to reduce psychological aversion while maintaining content understanding.

We evaluate this method through **eye-tracking experiments**, comparing:
- Raw gory videos
- Conventional blurring (whole-frame)
- Our segmentation-based blood blurring

---

## 🚀 Getting Started

Clone the repository and follow the instructions below:

```bash
git clone https://github.com/your-username/blood-blurring-demo.git
cd blood-blurring-demo

