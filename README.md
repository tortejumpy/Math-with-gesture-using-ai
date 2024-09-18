### README.md

```markdown
# Math Problem Solver Using Hand Gestures and AI

This project is a **hand gesture-based math problem solver** that uses a webcam to capture hand gestures and integrates Google's generative AI to solve math problems drawn in the air. The project leverages **OpenCV**, **cvzone**, and **Google's Gemini model** to interpret hand gestures, track hand movements, and interact with an AI to recognize and solve the drawn problems.

## Features
- **Hand Tracking**: Detects and tracks hand gestures using the webcam.
- **Drawing Math Problems**: You can draw a math problem in the air using specific hand gestures.
- **AI Problem Solving**: Sends the drawn math problem to Google's Gemini model for solution.
- **Real-Time Output**: Displays the answer in real-time on the GUI.
- **Gesture Controls**:
  - **Draw**: Raise your **index finger** to draw.
  - **Clear Canvas**: Raise your **thumb** to clear the canvas.
  - **Send to AI**: Raise your **thumb, index, and middle fingers** to send the drawing to the AI.

## Prerequisites

To run this project, you need the following installed:

- Python 3.x
- A webcam
- An active internet connection for AI integration

## Setup and Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/math-gesture-ai.git
   cd math-gesture-ai
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python main.py
   ```

## Usage

1. When the application starts, it opens a webcam feed and displays a drawing canvas.
2. Use your **index finger** to draw the math problem on the screen.
3. To clear the canvas, raise your **thumb**.
4. Once you're done drawing, raise your **thumb, index, and middle fingers** to send the problem to the AI.
5. The AI will interpret the drawing, solve the math problem, and display the answer on the screen.

## Requirements

- A webcam for gesture tracking
- API access to **Google Generative AI** for math problem solving

## API Configuration

The project uses Google's Gemini model for problem-solving. Make sure to add your **Google API key** in the `main.py` file:

```python
genai.configure(api_key="YOUR_API_KEY")
```

Replace `"YOUR_API_KEY"` with your actual Google API key.

## Dependencies

- **OpenCV**: For webcam input and image processing.
- **cvzone**: Simplifies hand detection using MediaPipe.
- **numpy**: For array manipulation.
- **Pillow**: For image processing.
- **streamlit**: For creating the web-based user interface.
- **google-generativeai**: API to interact with Google's generative AI for solving math problems.



This `README.md` explains how to set up and use the project, while the `requirements.txt` lists all the necessary Python packages.