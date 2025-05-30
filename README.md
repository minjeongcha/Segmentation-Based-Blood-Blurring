# Segmentation-Based-Blood-Blurring
Segmentation-Based Blood Blurring: Examining Eye-Response Differences in Gory Video Viewing

<p align="">
    <h3>
        | <a href="https://doi.org/10.3390/s25072093" target="_blank"><b>Paper</b></a> |
    </h3>
</p>

**Segmentation-Based Blood Blurring** is a novel video processing technique that selectively blurs blood-related content based on semantic segmentation. This approach is designed to reduce viewer discomfort during gory video viewing, and our study evaluates its effectiveness using eye-tracking data.

This repository contains the full code and dataset used in our paper:

**Son, J.; Cha, M.; Park, S. Segmentation-Based Blood Blurring: Examining Eye-Response Differences in Gory Video Viewing.** *Sensors 2025, 25, 2093.*  [https://doi.org/10.3390/s25072093](https://doi.org/10.3390/s25072093)

---

## What is Blood Blurring?

We propose a **segmentation-based filtering approach** to detect and blur only blood regions in videos. By leveraging semantic segmentation models, we ensure that non-violent parts remain untouched. The goal is to reduce psychological aversion while maintaining content understanding.


# Experiment Overview: Blood Blur and Human Visual Response

This repository provides all the datasets, code, and processed files used in our study on how **selective blood blurring** in violent videos affects viewer responses. We conducted multimodal experiments using segmentation, eye-tracking, and EAR (Eye Aspect Ratio) analysis.

---

## Video Dataset

We selected **5 violent video clips** rated suitable for **15 years or older**, each containing visually intense bloody scenes. These were used to generate two versions:
- **Original videos**  
- **Blurred versions** where blood regions were obfuscated using **YOLO-based semantic segmentation**.

We have also uploaded:
- The **raw coordinate data** of detected blood regions.
- Post-processed versions adjusted for our lab environment.
- The **Python analysis scripts** used for processing and coordinate correction.

---

## EAR (Eye Aspect Ratio) Data Collection

We used a **laptop webcam** and an **EAR algorithm** to measure participants’ eye openness in real-time while watching the videos.

### Processing Details:
- EAR values were collected at **0.1s intervals** for consistency.
- We defined an **eye blink** as a drop below an EAR threshold of **0.25**, followed by a rise above it, based on prior research.
- Blink detection and EAR smoothing were performed using our uploaded analysis scripts.

### Shared Files:
- Raw and processed EAR data  
- Blink count results  
- Python code for processing and visualization

---

## Eye-Tracking with Tobii Eye Tracker 5

We tracked participants’ gaze coordinates while watching the videos using **Tobii Eye Tracker 5**.

### Gaze vs. Blur Region Comparison:
- Gaze points were normalized.
- Each gaze point was checked against the **blurred blood region coordinates**.
- We marked whether each gaze point **entered (✔)** or **did not enter (✖)** a blurred area.

### Shared Files:
- Raw Tobii gaze data  
- Normalized gaze coordinates  
- Code for comparing gaze vs. blur regions  
- Binary labels for gaze-inside-blur detection

---

## Summary of Collected Data

| Data Type                     | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
|    Video Files               | Original + Blood-blurred versions of 5 clips                                |
|    Blur Region Coordinates   | YOLO-detected + post-processed bounding boxes                              |
|    EAR Data                  | Eye openness values at 0.1s intervals, blink detection                      |
|    Eye-Tracking              | Gaze points + overlap detection with blurred regions                        |
|    Level of gore              | Per-video ratings of perceived violence (1–7 Likert scale)                  |
|    MBPI Questionnaire        | Pre-experiment fear sensitivity to blood and injury                        |
|    Correlation Analysis      | Blink count, gaze ratio vs. MBPI score visualization                        |

Each participant's experiment data is in a separate folder.<br>
**"A-Z 데이터"** is the data from participants 1-26. <br>
A-Z(1-26), 27-37 is data from a total of **37 experiment participants.**
<br><br>
The **MBPI Questionnaire** and **Level of gore** collection data is organized in **Total Data Cleanup.**
<br><br>
The data graph and analysis code for correlating the **MBPI Questionnaire** data with the **Eye Openness Ratio, Blink Frequency, and Eye Fixations** data can be found in **Figure3.ipynb.**

## Reproducibility

All data files and scripts mentioned above are included in this repository for full reproducibility. If you're looking for a specific file, just ask — we’ll gladly direct you.

---

## Citation

Son, J.; Cha, M.; Park, S. Segmentation-Based Blood Blurring: Examining Eye-Response Differences in Gory Video Viewing. Sensors 2025, 25, 2093.
```
@article{son2025segmentation,
  title={Segmentation-Based Blood Blurring: Examining Eye-Response Differences in Gory Video Viewing},
  author={Son, Jiwon and Cha, Minjeong and Park, Sangkeun},
  journal={Sensors},
  volume={25},
  number={7},
  pages={2093},
  year={2025},
  publisher={MDPI}
}
```

---

## Questions?

Feel free to open an issue or contact [minjeongcha@khu.ac.kr] if you have questions about reproducing our experiments or using the dataset.

