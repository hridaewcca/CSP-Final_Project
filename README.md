# TINY HAND!
Tiny hand is a project that aims to make it easier to work with smaller tools and objects like when repairing a small device or working with a small electronics project.

# Inspiration
Linus attempts to fix a cpu with dead pins - https://www.youtube.com/watch?v=yh2XYkRwtBQ

Google Mediapipe hand tracking - https://github.com/google/mediapipe/blob/master/mediapipe/docs/hand_tracking_mobile_gpu.md

# Physical parts / Components

Hand tracking
- Camera
- Processing device

Mechanism
- Servos
- Wires (tendons)
- Rubber fingers

# Deconstruction

|      Data        |     Render      |  Simulation   |     Events    |
|------------------|-----------------| ------------- | ------------- |
| Hand XY          | Hand presence   |               | Hand movement |
| Hand Rotation    | Enable tracking |               | Switch on/off |
| Finger position  | Tracking points |               |               |
| Hand tilt        |                 |               |               |
| Camera Input     |                 |               |               |

# What's going to be hard?
Understanding how MediaPipe works
Mapping hand movement from how Mediapipe understands it to something that Servos can execute
Creating a small hand that actually works
