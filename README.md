# Hand Gesture Calculator

## Overview
The **Hand Gesture Calculator** is an innovative project that uses a webcam and MediaPipe's hand tracking solution to recognize hand gestures as numbers and mathematical operators. It allows users to perform basic arithmetic operations and evaluate mathematical expressions by simply using gestures.

## Features
- **Number Gestures**: Recognizes numbers 0-9 using intuitive finger counting.
- **Operator Gestures**: Supports addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), power (`^`), modulo (`%`), square root (`√`), and parentheses (`(`, `)`).
- **Expression Evaluation**: Builds mathematical expressions from recognized gestures and evaluates them.
- **Clear and Equals**: Gestures for clearing expressions and calculating results.
- **User Feedback**: Displays the recognized gesture, the current mathematical expression, and the result on the screen.
- **Gesture Stability**: Ensures gestures are stable before recognizing them, reducing accidental inputs.

## Requirements
- Python 3.7 or higher
- OpenCV
- MediaPipe
- NumPy

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hand-gesture-calculator.git
   cd hand-gesture-calculator
   ```
2. Install the required dependencies:
   ```bash
   pip install opencv-python mediapipe numpy
   ```

## How It Works
### Gesture Recognition
- **Numbers 0-5**: Standard finger counting.
- **Numbers 6-9**: Special combinations of fingers.
- **Operators**: 
  - `+` (Add): Thumb up
  - `-` (Subtract): Pinky up
  - `*` (Multiply): Thumb, index, and pinky up
  - `/` (Divide): Thumb and pinky close together
  - `^` (Power): Thumb, index, middle, and pinky up
  - `%` (Modulo): Thumb, middle, and pinky up
  - `(` and `)`: Thumb, index, and ring; Thumb, index, ring, and pinky
  - `√` (Square Root): Thumb, middle, and ring

### Interface
- The program uses OpenCV to show the live webcam feed.
- Recognized gestures, current mathematical expression, and results are displayed on the screen.
- Instructions for gestures are overlaid on the interface for ease of use.

## Usage
1. Run the program:
   ```bash
   python hand_gesture_calculator.py
   ```
2. Position your hand in front of the webcam.
3. Use gestures to input numbers and operators.
4. Perform the following actions:
   - Use the `=` gesture to evaluate the expression.
   - Use the `C` gesture to clear the expression.
5. Press `ESC` to exit the program.

## Gesture Guide
| Gesture                  | Action          |
|--------------------------|-----------------|
| Fist                    | `0`             |
| Index Finger            | `1`             |
| Peace Sign              | `2`             |
| Three Fingers           | `3`             |
| Four Fingers            | `4`             |
| All Fingers             | `5`             |
| Thumb, Index, Pinky     | `*` (Multiply)  |
| Thumb, Pinky Close      | `/` (Divide)    |
| Thumb, Index, Ring      | `(` (Left Paren)|
| Thumb, Index, Ring, Pinky | `)` (Right Paren) |
| Thumb, Middle, Ring     | `√` (Square Root) |

## Future Enhancements
- Add support for complex mathematical functions.
- Integrate voice feedback for recognized gestures.
- Improve gesture recognition for better accuracy in varying lighting conditions.
- Add support for multiple hands and gestures.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your enhancements.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
- **MediaPipe** for the powerful hand tracking library.
- **OpenCV** for real-time image processing.

---
**Happy Calculating with Hand Gestures!**
