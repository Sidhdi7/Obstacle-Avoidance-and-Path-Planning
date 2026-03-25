# Autonomous Wheelchair Navigation: Obstacle Avoidance & Path Planning

## Overview
This project focuses on developing a perception and navigation pipeline for autonomous wheelchair systems in indoor environments. It integrates real-time object detection with path planning to enable safe and efficient navigation around static and dynamic obstacles.

## Key Features
- Real-time obstacle detection using YOLO-based computer vision models  
- Handling of both **static** (walls, furniture) and **dynamic** (people, moving objects) obstacles  
- Integration of **A\*** path planning for optimal route computation  
- Adaptive navigation in constrained indoor environments (e.g., corridors, hospital layouts)  

## Methodology
The system combines perception and planning in a modular pipeline:

1. **Perception Layer**  
   - YOLO-based object detection model trained on indoor datasets  
   - Detection of relevant obstacles with bounding boxes and confidence scores  

2. **Environment Mapping**  
   - Conversion of detections into a grid-based representation  
   - Marking occupied and free spaces for navigation  

3. **Path Planning**  
   - A* algorithm used to compute the shortest collision-free path  
   - Dynamic re-planning triggered when obstacles are detected in real-time  

4. **Execution (Simulation)**  
   - Navigation decisions validated in simulated indoor environments  

## Results
- Achieved **92% precision** for static obstacle detection  
- Achieved **88% precision** for dynamic obstacle detection  
- Demonstrated reliable navigation in corridor-like environments with moving obstacles  

## Tech Stack
- Python  
- YOLO (You Only Look Once)  
- OpenCV  
- A* Path Planning Algorithm  

## Demo / Output
(Add screenshots or videos here)
- Example: Detected obstacles with bounding boxes  
- Example: Planned path visualization on grid/map  
- Example: Navigation trajectory in simulation  

## Project Structure
