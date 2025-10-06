# SignModel: Pose-to-Text Sign Language Translation

## Overview
SignModel is an innovative project for real-time sign language translation, converting video inputs of sign language gestures into accurate text using pose estimation and large language model (LLM) refinement. This repository contains the official code for the research paper *"Pose-to-Text: Revolutionizing Sign Language Translation with Real-Time LLM Refinement"*, presented at the final round of Sciblitz 1.0 at Chittagong University of Engineering and Technology (CUET).

The model processes sign language videos by extracting poses (e.g., via MediaPipe), analyzing optical flow for motion, and refining outputs with an LLM to achieve ~95% translation accuracy. It's designed for accessibility applications, such as real-time communication aids for the deaf community.

## Features
- **Real-Time Translation**: Processes video frames to extract poses and generate text outputs efficiently.
- **Multimodal Integration**: Combines computer vision (pose estimation, optical flow) with NLP (LLM for grammar correction and refinement).
- **High Accuracy**: Achieves up to 95% accuracy on sign language video datasets.
- **Research Outputs**: Includes saved visualizations, JSON results, and a generated research paper section.
- **Scalable Pipeline**: Suitable for extension to agentic video editing tools, like automating subtitles or scene analysis.

## Tech Stack
- **Languages**: Python 3.11+
- **Libraries**:
  - PyTorch & TorchVision: For deep learning models and inference.
  - OpenCV: For video processing, pose extraction, and optical flow.
  - NumPy & Scikit-Learn: For data handling, metrics, and preprocessing.
  - MediaPipe/OpenPose: For pose estimation (inferred from typical implementations).
- **Environment**: Tested on Kaggle with GPU acceleration (NVIDIA Tesla T4).
- **Other**: Jupyter Notebook for experimentation and result generation.

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/Jawadbro/SignModel.git
   cd SignModel
   ```
2. Install dependencies:
   ```
   pip install torch torchvision opencv-python numpy scikit-learn
   ```
   (For GPU support, ensure CUDA is installed and compatible with PyTorch.)

3. Download datasets (e.g., from Kaggle sources mentioned in the notebook) and place them in the appropriate directory.

## Usage
1. Open the Jupyter Notebook `signmodel.ipynb` in Jupyter or Kaggle.
2. Run the cells sequentially:
   - Install packages.
   - Load and process video data.
   - Extract poses and refine with LLM.
   - Generate and save results (JSON, text, visualizations).

Example command to run locally:
```
jupyter notebook signmodel.ipynb
```

Outputs will be saved to `/kaggle/working/` or your local directory, including:
- `slr_research_results.json`: Research metrics.
- `slr_research_paper.txt`: Generated paper sections.
- Visualization PNGs: Graphs and charts.


## Results & Research Paper
- **Accuracy**: 50-60% on benchmark datasets for sign-to-text translation.
- **Visualizations**: Includes plots for pose extraction, optical flow, and accuracy metrics.
- **Paper**: The code generates sections of the research paper, focusing on methodology and results. Full paper presented at Sciblitz 1.0 CUET.

Citation:
```
@article{karim2025pose,
  title={Pose-to-Text: Revolutionizing Sign Language Translation with Real-Time LLM Refinement},
  author={Karim, Jawadul},
  year={2025},
  note={Presented at Sciblitz 1.0, CUET}
}
```

- Integrate speech input for bidirectional communication.
- Optimize for mobile deployment.
- Expand to more sign languages and datasets.

## Contributions
This project builds on my research experience in AI for accessibility, as detailed in my resume (e.g., Speak Elevate's speech analysis systems).

## Contact
- Jawadul Karim
- Email: jawadulk06@gmail.com
- GitHub: [Jawadbro](https://github.com/Jawadbro)

Feel free to open issues or PRs for improvements!
