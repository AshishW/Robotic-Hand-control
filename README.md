![Robot Hand Screenshot](./screenshot.png)
# Robotic-Hand-control

This project is a web-based, real-time 3D simulation of a robotic hand. It uses a webcam to track the user's hand movements and mirrors them on the 3D model.

## How it Works

1.  **Hand Tracking**: The application uses **MediaPipe Hand Landmarker** via the webcam to detect the 3D landmarks of the user's hand in real-time.
2.  **3D Rendering**: A detailed 3D model of a robotic hand is rendered using **Three.js**. The scene includes lighting, shadows, and interactive camera controls.
3.  **Animation**: The positional data from MediaPipe is used to calculate the angles of the finger joints. These angles are then applied to the corresponding joints of the 3D model. **GSAP** is used to animate the transitions smoothly.
4.  **Manual Controls**: The application provides an option to manually control the robotic hand using on-screen sliders for each finger joint. This allows for precise positioning and posing of the hand.
5.  **Pose Saving and Loading**: Users can save their hand poses and load them later, enabling easy replay of specific gestures or positions.
6.  **Gesture Recognition**: The application can recognize and respond to specific hand gestures, allowing for interactive control of the robotic hand.
7.  **Calibration**: A calibration routine is available to ensure accurate mapping between the user's hand and the robotic model, accommodating different hand sizes and shapes.
