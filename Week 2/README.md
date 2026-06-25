## Week 2: Image Preprocessing with OpenCV

Load two images and perform grayscale conversion, histogram visualization, resizing, edge detection, and noise addition/removal.

### Images used:

Brain MRI — a medical grayscale scan used to demonstrate image processing on real-world healthcare data
Panda — a natural image used as a general-purpose visual counterpart


### Libraries used:

OpenCV (cv2) — image loading, grayscale conversion, resizing, edge detection
NumPy — array operations and noise generation
Matplotlib — visualization
scikit-image (skimage) — image filters
scipy.ndimage — Gaussian denoising filter


### Subtasks:

Subtask 1: Grayscale Conversion

- Both images are converted from BGR (OpenCV default) to grayscale using cv2.COLOR_BGR2GRAY.

Subtask 2: Histogram Visualization

- Pixel intensity histograms are plotted (256 bins, range 0–255) for both grayscale images, showing the distribution of dark and light regions.

Subtask 3: Image Resizing

- Both images are resized to 256×256 pixels using cv2.resize(), standardizing them for downstream processing.

Subtask 4: Edge Detection

- Edges are detected using the Canny edge detector with:


  - Low threshold: 50
  - High threshold: 150


Subtask 5: Noise Addition & Removal


- Noise added: Gaussian noise with mean=0, sigma=25
- Noise removed: Gaussian filter from scipy.ndimage with sigma=2
