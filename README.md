# Vehicle Speed Detection System

This Python script detects and tracks vehicles in a video feed, calculates their speed, and identifies vehicles exceeding the speed limit. It utilizes background subtraction techniques, contour detection, and basic physics principles to estimate vehicle speed.

## Features

- **Speed Detection**: Calculates the speed of vehicles passing through designated lanes.
- **Overspeed Detection**: Identifies vehicles exceeding the speed limit.
- **ROI Saving**: Saves regions of interest (ROIs) for overspeeding vehicles.
- **Frame Saving**: Saves frames with overspeeding vehicles for further analysis.

## Prerequisites

- Python 3.x
- OpenCV (`pip install opencv-python`)
- NumPy (`pip install numpy`)

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/SrijanSadhu/vehicle-speed-detection.git
   ```

2. Navigate to the project directory:

   ```bash
   cd vehicle-speed-detection
   ```

3. Place your video file (e.g., `Test1.mp4`) in the project directory.

4. Create two mask images (`m1.jpeg` and `m2.jpeg`) for defining regions of interest (ROIs) for each lane. The masks should be grayscale images where white represents the areas of interest.

5. Run the script:

   ```bash
   python vehicle_speed_detection.py
   ```

6. Follow the prompts to enter the speed limit.

7. Press 'x' to stop the script and view the results.

## Configuration

- `speed_limit`: Set the speed limit for vehicles.
- `method`: Choose the background subtraction method (0 for MOG, 1 for MOG2, others for GMG).
- Adjust parameters like kernel sizes, thresholds, and ROI dimensions as needed.

## Output

- Overspeeding frames are saved as `overspeed_frame_<index>.jpeg`.
- ROIs for overspeeding vehicles are saved in the main directory.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
