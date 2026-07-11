# MediVision AI

MediVision AI is an AI-powered healthcare assistance platform that combines Generative AI, Computer Vision, and Voice Technology to provide an interactive healthcare support experience.

The application allows users to describe health concerns through voice input and upload medical or skin-related images for AI-assisted analysis. It generates preliminary health-related information and provides responses in both text and speech formats.

The project also explores brain tumor detection using YOLOv8 and integrates speech recognition, artificial intelligence, medical image analysis, and text-to-speech technologies within a unified Gradio-based interface.

> **Medical Disclaimer:** MediVision AI is developed solely for educational, research, and demonstration purposes. It does not provide a confirmed medical diagnosis and should not be considered a substitute for professional medical advice, diagnosis, or treatment. Users should consult qualified healthcare professionals regarding medical concerns.

---

## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Key Features](#key-features)
- [System Workflow](#system-workflow)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Environment Configuration](#environment-configuration)
- [Running the Application](#running-the-application)
- [Brain Tumor Detection](#brain-tumor-detection)
- [Voice Interaction](#voice-interaction)
- [Future Enhancements](#future-enhancements)
- [Ethical Considerations](#ethical-considerations)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [Author](#author)
- [License](#license)

---

## Overview

MediVision AI explores the application of artificial intelligence in building accessible and interactive healthcare-support systems.

The platform combines multiple AI technologies to support:

- Voice-based patient interaction
- AI-assisted healthcare conversations
- Medical and skin-image analysis
- Brain tumor detection using YOLOv8
- Speech-to-text processing
- AI-generated healthcare information
- Text-to-speech response generation
- Interactive web-based access using Gradio

The application is designed as an educational and research-oriented healthcare support system. It is not intended to replace medical professionals or clinical diagnostic procedures.

---

## Problem Statement

Access to immediate healthcare information may be limited by geographical, financial, or time-related constraints. Many existing healthcare applications also lack support for multimodal interaction involving voice, text, and images.

MediVision AI explores an intelligent healthcare-assistance platform capable of accepting patient input through voice, processing health-related information using artificial intelligence, analysing uploaded images, and presenting preliminary information in an understandable format.

The system aims to improve the accessibility of general healthcare information while maintaining transparency regarding the limitations of AI-generated responses.

---

## Objectives

The primary objectives of MediVision AI are:

- To develop an interactive AI-powered virtual healthcare assistant
- To enable voice-based interaction for improved accessibility
- To integrate computer-vision techniques for image analysis
- To explore brain tumor detection using YOLOv8
- To support preliminary analysis of skin-related images
- To generate understandable AI-assisted healthcare information
- To convert generated responses into speech
- To provide a simple and accessible interface using Gradio
- To promote responsible and transparent use of artificial intelligence in healthcare

---

## Key Features

### AI-Powered Healthcare Assistant

- Accepts health-related descriptions from users
- Processes user input using artificial intelligence
- Generates understandable preliminary healthcare information
- Supports conversational interaction

### Voice-Based Interaction

- Accepts patient voice input
- Converts speech into text
- Processes the transcribed information
- Generates voice-based responses
- Supports text-to-speech technologies such as ElevenLabs and gTTS

### Medical Image Analysis

- Accepts image input through the application interface
- Processes uploaded images using computer-vision techniques
- Generates AI-assisted observations
- Supports experimental analysis of selected medical and skin-related images

### Brain Tumor Detection

- Uses YOLOv8 for experimental brain tumor detection
- Processes medical imaging data
- Identifies potential regions of interest
- Visualises model predictions

### Interactive User Interface

- Developed using Gradio
- Provides support for voice and image input
- Displays generated text responses
- Provides audio output for improved accessibility

---

## System Workflow

```text
User
  |
  |-- Voice Input
  |       |
  |       v
  |   Speech-to-Text
  |
  |-- Image Input
          |
          v
   Image Preprocessing
          |
          v
Artificial Intelligence Processing
          |
          v
Preliminary Information Generation
          |
          v
Text Response
          |
          v
Text-to-Speech Conversion
          |
          v
Voice Response
```

The general processing workflow consists of the following stages:

1. The user provides health-related information through voice or image input.
2. Voice input is converted into text using speech-recognition technology.
3. Uploaded images are prepared for AI-assisted analysis.
4. The AI system processes the available information.
5. A preliminary informational response is generated.
6. The response is displayed as text.
7. The generated text is converted into speech.
8. The user receives both textual and audio output.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core application development |
| Gradio | Interactive web-based user interface |
| YOLOv8 | Experimental brain tumor detection |
| Computer Vision | Medical and skin-image processing |
| Generative AI | Healthcare-related response generation |
| Speech Recognition | Conversion of patient voice input into text |
| ElevenLabs | AI-generated voice responses |
| gTTS | Text-to-speech conversion |
| Jupyter Notebook | Model experimentation and development |
| Git | Source-code version control |
| GitHub | Repository hosting and project collaboration |

---

## Project Structure

```text
MediVision-AI/
|
└── Ai doctor/
    |
    ├── brain-tumor-detection-with-yolov8.ipynb
    ├── brain_of_the_doctor.py
    ├── gradio_app.py
    ├── dataset_skin/
    ├── acne.jpg
    ├── dandruff-optimized.webp
    ├── elevenlabs_testing.mp3
    ├── elevenlabs_testing_autoplay.mp3
    ├── gtts_testing.mp3
    ├── gtts_testing_autoplay.mp3
    ├── patient_voice_test.mp3
    ├── patient_voice_test_for_patient.mp3
    ├── final.mp3
    ├── ai-doctor-voicebit-ppt.pdf
    ├── Pipfile.lock
    └── README.md
```

### Important Files

| File | Description |
|---|---|
| `gradio_app.py` | Contains the Gradio-based application interface |
| `brain_of_the_doctor.py` | Contains the core AI healthcare-assistant functionality |
| `brain-tumor-detection-with-yolov8.ipynb` | Contains experiments related to brain tumor detection using YOLOv8 |
| `dataset_skin/` | Contains resources used for skin-image analysis |
| `Pipfile.lock` | Stores locked project dependency versions |
| `ai-doctor-voicebit-ppt.pdf` | Contains project presentation material |

---

## Installation

### Prerequisites

Ensure that the following software is installed:

- Python 3.9 or later
- Git
- Pip
- Pipenv, if the project uses a Pipfile
- Jupyter Notebook, for running the model-development notebook

### Step 1: Clone the Repository

```bash
git clone <repository-url>
```

Replace `<repository-url>` with the URL of the GitHub repository.

### Step 2: Navigate to the Project Directory

```bash
cd MediVision-AI
```

Navigate to the application folder:

```bash
cd "Ai doctor"
```

### Step 3: Create a Virtual Environment

```bash
python -m venv venv
```

### Step 4: Activate the Virtual Environment

For Windows:

```bash
venv\Scripts\activate
```

For Linux or macOS:

```bash
source venv/bin/activate
```

### Step 5: Install Dependencies

If the project uses Pipenv:

```bash
pip install pipenv
```

```bash
pipenv install
```

If a `requirements.txt` file is added later, dependencies can be installed using:

```bash
pip install -r requirements.txt
```

---

## Environment Configuration

Create a `.env` file inside the application directory and add the required API credentials.

Example:

```env
ELEVENLABS_API_KEY=your_elevenlabs_api_key
```

Additional API credentials may be required depending on the AI services configured in the application.

Do not commit API keys or other sensitive credentials to GitHub.

Add the following entries to the `.gitignore` file:

```text
.env
venv/
__pycache__/
*.pyc
```

---

## Running the Application

Activate the virtual environment and run the Gradio application:

```bash
python gradio_app.py
```

After the application starts, Gradio displays a local URL in the terminal.

Example:

```text
http://127.0.0.1:7860
```

Open the displayed URL in a web browser to access the application.

---

## Brain Tumor Detection

The project includes a Jupyter Notebook that explores brain tumor detection using YOLOv8.

Notebook:

```text
brain-tumor-detection-with-yolov8.ipynb
```

The experimental workflow includes:

1. Medical image collection
2. Image preprocessing
3. Dataset preparation
4. YOLOv8 model configuration
5. Model training or inference
6. Detection of potential regions of interest
7. Prediction visualisation
8. Evaluation of model performance

The generated predictions are experimental and should not be interpreted as clinical diagnoses.

---

## Voice Interaction

The voice-interaction module enables users to communicate with the application using speech.

The voice-processing workflow is:

```text
Patient Voice Input
        |
        v
Speech Recognition
        |
        v
Text Transcription
        |
        v
AI-Based Processing
        |
        v
Healthcare Information Generation
        |
        v
Text-to-Speech Conversion
        |
        v
Voice Response
```

The application explores the use of ElevenLabs and gTTS for generating audio responses.

---

## Future Enhancements

Potential future improvements include:

- Integration of additional medical image-analysis models
- Support for additional skin conditions
- Improved brain tumor classification
- Multilingual voice interaction
- Secure user authentication
- Patient-controlled history management
- Improved model explainability
- Cloud-based deployment
- Mobile application support
- Integration with healthcare professionals
- Improved accessibility features
- Enhanced data privacy and security
- Model-performance monitoring
- Support for additional medical datasets

---

## Ethical Considerations

Healthcare-related AI systems require responsible design and usage.

The following principles should be considered:

- User information should be handled securely.
- Health-related data should not be collected without informed consent.
- AI-generated responses should be clearly identified.
- Model predictions should not be presented as confirmed diagnoses.
- Users should be informed about the limitations of the system.
- Medical decisions should remain under the supervision of qualified healthcare professionals.
- Bias and performance limitations should be evaluated before real-world deployment.
- Sensitive information should not be exposed through source code, logs, or public repositories.

---

## Limitations

MediVision AI has the following limitations:

- AI-generated information may be incomplete or inaccurate.
- Model predictions depend on the quality and diversity of the training data.
- Medical-image predictions are experimental.
- The system has not been validated for clinical use.
- Voice recognition may be affected by background noise, pronunciation, or audio quality.
- The application cannot replace physical examinations, laboratory tests, medical imaging assessments, or professional clinical judgment.

---

## Medical Disclaimer

MediVision AI is intended exclusively for educational, academic, research, and demonstration purposes.

The information and predictions generated by the application:

- Do not constitute professional medical advice
- Do not represent a confirmed medical diagnosis
- Should not be used to determine treatment
- Should not replace consultation with a qualified healthcare professional
- Should not be used for emergency medical decisions

Users should consult qualified healthcare professionals regarding symptoms, diagnoses, medications, or treatment decisions.

---

## Contributing

Contributions that improve the functionality, documentation, accessibility, security, or responsible use of the project are welcome.

### Contribution Steps

1. Fork the repository.

2. Clone the forked repository:

```bash
git clone <forked-repository-url>
```

3. Create a new feature branch:

```bash
git checkout -b feature/feature-name
```

4. Make the required changes.

5. Add the modified files:

```bash
git add .
```

6. Commit the changes:

```bash
git commit -m "feat: add feature description"
```

7. Push the branch:

```bash
git push origin feature/feature-name
```

8. Open a pull request and provide a clear description of the changes.

---

## Author

**Gideon Samuel**

B.Tech in Computer Science and Business Systems  
Thiagarajar College of Engineering

---

## License

This project is intended for educational and research purposes.

If the repository is released as an open-source project, an appropriate license should be added to define the permitted use, modification, and distribution of the source code.
