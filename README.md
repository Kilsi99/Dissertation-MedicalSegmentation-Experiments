# Enhancing Medical Image Segmentation with Localized Attention Mechanisms

### Project overview 
This prject aims to investigate about specalised or localised attention mechanisms can reweight salients features of medical segmentations models receptive fields to capture suble or fine details 
anatomical details, these attention mechanisms aim to improve segmentation accuracy and increase clinical utility across datasets of varying anatomical structures.

### Datasets 
The project uses publicly available, anonymised datasets
Medical Decathalon Hippocampus - 260 3D MRI scans of left and right hippocampus (35x35x35).
ISIC 2016 Challenge (skin lesions) - 1279 dermoscopic images with segmentation masks (256x256).
CVC-ClinicDB (polyps) - 612 colonoscopy images with polyp segmentation masks (256x256).
notes: Raw datasets are not included into the repo.

### Models
Implemented models include:
1. Baseline U-net - Standard enccoder-decoder structure.
2. CBAM U-net - U-net augmented with attention, channel attention and spacial attention
3. Baseline Vision Transformer (ViT) - Patch-based transformer for image segmentation using global attention
4. local Attention ViT - ViT with window-based local attention for local feature focus
5. 3D variants - for hippocampus datastet (U-Net and CBAM adapted to 3D).

### Experiments

Training scripts for each model and dataset.
Hyperparameters: Adam optimizer, weighted Dice + Cross-Entropy loss, learning rate scheduling, batch size 8, 25 epochs.
Data preprocessing and augmentation scripts for each dataset.

### Evaluation
Metrics: Dice coefficient, Hausdorff distance, Volume Similarity, pixel-wise accuracy.
Evaluation scripts generate metrics and plots for model performance comparison.
Example usage included in evaluate.py or Jupyter notebooks.

### License 
Private academic use only - for thess=is assessment
