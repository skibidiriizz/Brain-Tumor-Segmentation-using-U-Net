# Brain Tumor Segmentation using U-Net

This project implements a brain tumor segmentation pipeline using a U-Net architecture. The goal is to accurately segment tumor regions from brain MRI scans.

## 📁 Project Structure

- `brain-segmentation-unet.ipynb`: Main Jupyter notebook for training, evaluating, and visualizing the segmentation model.
- `ground vs predicted.png`: Comparison visualization of model predictions vs. ground truth masks for test samples.

## 🧠 Dataset

The model is trained and evaluated on a brain MRI dataset with corresponding tumor masks. Each sample consists of:

- **Original Image**: MRI scan of a brain.
- **Ground Truth Mask**: Manually annotated mask indicating tumor regions.
- **Predicted Mask**: Output of the U-Net model.

## 🧬 Model Architecture

The segmentation model is based on a U-Net architecture, which is well-suited for biomedical image segmentation tasks due to its encoder-decoder structure with skip connections.

## 🔍 Evaluation

The performance is measured using the **Dice Coefficient**, a metric that quantifies the overlap between predicted and true masks. A Dice score closer to 1 indicates better performance.

### Example Results

| Sample | Dice Score |
|--------|------------|
| 1      | 0.8645     |
| 2      | 0.8554     |
| 3      | 0.8472     |
| 4      | 0.8363     |

See `ground vs predicted.png` for visual comparisons.

## 🚀 How to Run

1. Clone the repository.
2. Open `brain-segmentation-unet.ipynb` in Jupyter Notebook or Google Colab.
3. Install necessary packages (e.g., `tensorflow`, `numpy`, `matplotlib`).
4. Train the model or load pretrained weights.
5. Run the evaluation cells to generate predictions and metrics.

## 🖼️ Visualization

The notebook includes visualization utilities to compare:
- Input MRI scan
- Ground truth mask
- Predicted segmentation mask

This allows for qualitative assessment alongside Dice score evaluation.

## 📌 Requirements

- Python 3.7+
- TensorFlow 2.x
- NumPy
- OpenCV
- Matplotlib

Install via pip:

```bash
pip install tensorflow numpy opencv-python matplotlib
