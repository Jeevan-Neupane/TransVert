
# TransVert: 2D-to-3D Vertebrae Volume Reconstruction

**TransVert** is a deep learning model for reconstructing 3D vertebra volumes from sagittal and coronal 2D medical slices. It uses a dual-encoder architecture followed by a 3D volume expander and is trained with a custom Dice Loss function. This repository includes training, validation, evaluation, and interactive visualization tools.

---

## Features

-  Dual-view 2D input (sagittal + coronal) → 3D volume output
- Dice Loss-based optimization
- Training & validation loss tracking with `wandb`
- Inline evaluation loop with Dice Score logging
- 🖼Visual mid-slice predictions (wandb + matplotlib)
- Interactive 3D slice viewer with `ipywidgets`

---

## Dependencies

```bash
pip install torch torchvision matplotlib tqdm wandb ipywidgets scikit-image
