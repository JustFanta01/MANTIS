## [IPCV] Development of a computer vision system aimed at intrusion detection

Repository structure:
- `src/` folder: <br>
  it contains the main algorithm used for the Motion Detection. It is a combination of Temporal Median algorithm and the OpenCV MOG2 (Mixture of Gaussians).
  - `IntrusionDetection.ipynb`: **main file**
- `experiments/` folder:<br>
  it contains experiments to qualitatively understand which algorithm or configuration works the best for our scenario.
  - `IntrusionDetectionComparison.ipynb`<br>
    MOG2 vs. CNT vs. TemporalMedian
  - `MaskedArray.ipynb`<br>
    Selective update for the Temporal Median
  - `PostProcessing.ipynb`:<br>
    Comparison among postprocessing techniques for enhancing the segmentation.
- `video/` folder:<br>
  it contains the specific video of our challenge.
- `requirements.txt`<br>
  file containing all the external libraries used in the project.
  ```
  $ python -m venv venv_motion_detection
  $ source venv_motion_detection/bin
  $ pip install -r requirements.txt
  ```