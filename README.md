# Sketch-Stream

# Live Webcam Sketching System  

An interactive application that enables real-time virtual drawing using computer vision. The system tracks a colored object through a webcam and overlays drawings on the live video feed.  

## Features  

### 1. **Real-time Color Tracking**  
- Uses HSV-based color detection for accurate marker tracking.  
- Allows dynamic adjustments with trackbars to adapt to different lighting conditions.  

### 2. **Multi-Color Drawing**  
- Supports multiple pen colors: **Red, Green, Blue, Yellow**.  
- Users can select colors by hovering over on-screen buttons.  

### 3. **Interactive GUI**  
- Provides buttons for **color selection** and **canvas clearing**.  
- Ensures smooth user experience with real-time visual feedback.  

### 4. **Noise Reduction & Smooth Drawing**  
- Uses **morphological transformations** to minimize false detections.  
- Implements **deque** data structure to maintain fluid motion while drawing.  

---  
## System Architecture  

1. **Input:** Captures a live video feed from the webcam.  
2. **Processing Pipeline:**  
   - Converts frames to **HSV color space**.  
   - Creates **binary masks** for marker isolation.  
   - Analyzes contours to determine marker position.  
3. **Interaction & Drawing:**  
   - Tracks marker movement to draw on the canvas.  
   - Clears the canvas when interacting with the **CLEAR** button.  
4. **Output:** Displays the augmented video feed with drawings overlaid.  

---  

## Requirements

1. **OpenCv** for real-time video processing
2. **Numpy** for numerical operations.
3. **Webcam** for live input
