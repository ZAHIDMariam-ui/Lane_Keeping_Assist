# Lane Keeping Assist (LKA) – Video Analysis

A computer vision project implementing the perception component of a Lane Keeping Assist (LKA) system. The application processes forward-facing driving videos to detect lane boundaries, estimate the vehicle's position within the lane, and visualize the results.

## Features

- Left and right lane boundary detection.
- Lane centre estimation.
- Vehicle lateral position estimation.
- Detection confidence and uncertainty handling.
- Temporal smoothing across video frames.
- Visual lane overlay on road videos.
- Analysis of detection performance under different road conditions.

## Processing Pipeline

1. **Video Input:** Read forward-facing road videos frame by frame.
2. **Region of Interest:** Focus on the relevant road area.
3. **Image Processing:** Apply colour filtering and edge detection to identify lane markings.
4. **Lane Detection:** Extract and identify candidate lane boundaries.
5. **Boundary Estimation:** Fit lane boundaries and calculate the lane centre.
6. **Position Analysis:** Estimate the vehicle's position relative to the lane centre.
7. **Temporal Processing:** Improve detection stability and handle uncertain boundaries.
8. **Visualization:** Display lane boundaries, vehicle position, and confidence information on the output video.

## Technologies

- Python
- OpenCV
- NumPy
- Matplotlib

## Execution

Open the Jupyter Notebook and execute the cells to process the input video and generate the lane detection results.

## Limitations and ODD

The system is designed for offline road video analysis. Its performance depends on road visibility and lane marking quality.

Challenging conditions include:

- Sharp curves and changing road geometry.
- Shadows and variable lighting.
- Faded or missing lane markings.
- Complex road layouts and ambiguous boundaries.

The system uses uncertainty handling to avoid presenting unreliable lane detections as confident results.

## Author

Mariam Zahid

**Course:** Vehicles and Sensors  
**Institution:** Eötvös Loránd University (ELTE)
