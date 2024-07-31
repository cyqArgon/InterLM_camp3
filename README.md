# InterLM_camp3
一个基于InterLM的武术评分器
# Martial Arts Scoring System Based on InterLM

Welcome to the Martial Arts Scoring System, a project designed to recognize and evaluate martial arts movements using advanced machine learning models. This system leverages the power of the YOLO (You Only Look Once) model for action recognition and a fine-tuned InterLM language model for scoring and feedback generation.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to provide an automated scoring and evaluation system for martial arts movements. By using YOLO for real-time action recognition and a fine-tuned InterLM model, the system can assess the quality of the movements and provide detailed feedback. For more information, visit the [InterLM Tutorial](https://github.com/InternLM/Tutorial) on GitHub.

## Features

- **Action Recognition**: Utilizes YOLO to detect and recognize various martial arts movements.
- **Scoring System**: Employs a fine-tuned InterLM model to score the movements based on predefined criteria.
- **Feedback Generation**: Provides detailed feedback on the movements to help practitioners improve their techniques.
- **Real-time Processing**: Capable of processing video feeds in real-time for immediate evaluation.

## Installation

To get started with the Martial Arts Scoring System, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/martial-arts-scoring-system.git
    cd martial-arts-scoring-system
    ```

2. **Set up the environment:**
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    pip install -r requirements.txt
    ```

3. **Download the YOLO weights and InterLM model:**
    - Follow the instructions in the `models/` directory to download the necessary model weights.

## Usage

1. **Run the Action Recognition Module:**
    ```bash
    python yolo_action_recognition.py --video path_to_video
    ```

2. **Evaluate the Actions:**
    ```bash
    python evaluate_actions.py --input recognized_actions.json
    ```

3. **Generate Feedback:**
    ```bash
    python generate_feedback.py --input scores.json
    ```

## Model Details

### YOLO Model
YOLO (You Only Look Once) is a state-of-the-art, real-time object detection system. In this project, it has been adapted for recognizing various martial arts movements from video feeds.

### InterLM
InterLM is a powerful language model that has been fine-tuned specifically for evaluating martial arts movements. It takes recognized actions as input and generates scores and feedback based on a set of predefined criteria.

## Contributing

We welcome contributions to improve the Martial Arts Scoring System. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

We hope this system helps martial arts practitioners improve their skills through detailed and accurate feedback. If you have any questions or suggestions, feel free to open an issue or contact us directly. Happy training!
