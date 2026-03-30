# Coronary Artery Segmentation

**Research project**: Development of computational methods for semi-automatic segmentation of coronary arteries from dynamic CT imaging (INEGI, 2022-2025).

## Technical Implementation

**1. DICOM Processing Interface**
- Simple Tkinter GUI for DICOM file upload and preprocessing
- pydicom for metadata extraction and multi-frame handling

**2. Aortic Root Detection** 
- ML-free algorithm for automatic aortic root seed point prediction
- Geometric + intensity-based initialization

**3. Region Growing Segmentation**
- Primary aorta + coronary arteries segmentation using `skimage` region growing
- `scipy.ndimage` for distance transforms and connectivity analysis

**4. Coronary Separation**
- Skeletonization (`skimage.morphology`) for centerline extraction
- Bifurcation detection + pruning algorithm for individual coronary identification
- Strategic cut-points based on anatomical branching patterns

**5. Segmentation Refinement**
- Multi-stage region growing with adaptive thresholds
- Edge enhancement using Canny + morphological operations
- Iterative boundary refinement with active contours

**6. 3D Model Generation**
- VMTK pipeline for hemodynamic simulation preparation:
  * Centerline extraction with bifurcation detection
  * Model expansion to hyperemia conditions (30% vessel dilation)
  * Surface mesh generation and smoothing

## Tech Stack
Python | pydicom | Tkinter | scikit-image | scipy | VMTK | OpenCV | matplotlib


## Outcome
- Supported 3 master's theses in cardiac segmentation
- Presented at ICEM20, ESB2023, ECCOMAS 2024
- Clinical validation with cardiologists
