# # Ball Tracking and Event Logging
This project tracks colored balls in a video, determines the quadrant they are in, detects entry/exit events, and outputs analysis data.
## Overview
-   Loads video file
-   Detects balls based on color ranges
-   Determines quadrant for each ball
-   Labels balls and quadrants in output video
-   Logs entry/exit events to a text file with timestamps
-   Converts processed AVI video to shareable MP4 format
## Usage
To process a video:

1.  Update  `video_path`  to point to the input video file
2.  Run the Python script:

 `python object tracking.py`

3.  The outputs will be saved to the same folder:
-   `processed_video.avi`: Video with ball tracking visualizations
-   `event_records.txt`: Entry/exit events and timestamps
-   `processed_video.mp4`: MP4 version of the processed video

## Configuration

The color ranges for detection can be configured by modifying the `color_ranges` dictionary. Tune these ranges to accurately detect each colored ball in the video.

Logic for determining entry vs exit events should also be customized based on the specific setup.
## Installation

Requires OpenCV and Python. Can be installed via:

    pip install opencv-python numpy moviepy



## Customization

Possible ways to expand this:

-   Track other object types (vehicles, animals etc)
-   Integrate with IP cameras for live processing
-   Perform more complex analytics on ball events
-   Create graphical dashboards and reports

## License

MIT license - free to use, modify and distribute this code.

Let me know if any sections need additional detail or if you have other ideas for the README!
