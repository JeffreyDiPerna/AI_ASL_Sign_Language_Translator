
<div align="center">

<h1>ASL Sign Translator</h1>

<h1>🏆 First Place — Microsoft Firm Day Hackathon</h1>
<h1>🌟 Social Impact Award — Canadian Undergraduate Conference for Artificial Intelligence (CUCAI)</h1>


</div>


## Description
**ASL Sign Translator** takes user video input and identifies the **sign** the user is performing. Built in **Python** on **Google Colab**, it leverages **convolutional neural networks (CNNs)** to process frames and classify signs.

**Why it’s useful**
- **Advances accessibility** — bridges communication between signing and non‑signing users.
- **Runs easily in Colab** — minimal setup; adaptable to local environments if preferred.
- **Model‑driven reliability** — CNN feature extraction with robust evaluation metrics.

**Core capabilities**
- **Video ingestion** across common formats (e.g., `.mp4`, `.mov`).
- **Frame processing & aggregation** with standardized transforms and majority voting.
- **Evaluation suite** including Accuracy, Precision, Recall, F1, and Confusion Matrix.

---

## Getting Started / Installation

### Prerequisites
- **Runtime:** Python ≥ 3.9 (Google Colab recommended; GPU optional)
- **Tools:** Git, pip (FFmpeg optional for video conversion)

### Dependencies
- `torch`, `torchvision`
- `opencv-python`
- `numpy`, `pandas`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `Pillow`
- `google-colab` *(available in Colab runtime)*  
- Standard libs: `os`, `collections.Counter`

### Option A — Run in Google Colab (Recommended)
1. Open the notebook (e.g., **`ASL_Sign_Translator.ipynb`**) in **Google Colab**.  
2. Runtime → **Change runtime type** → select **GPU** (if available).  
3. (Optional) **Mount Google Drive** to access data/models.  
4. Place videos under `/content/drive/MyDrive/.../data/videos/` and run the notebook cells.

### Option B — Run Locally
1. Clone the repository and create a virtual environment.  
2. Install the dependencies listed above with `pip`.  
3. Add your videos to `data/videos/` and (optionally) your trained model to `models/model.pt`.  
4. Run the notebook (e.g., Jupyter) or your minimal inference script.

---

## Usage

- **Inference (Notebook):**  
  Upload a video → run the **Predict** cell → view the **predicted sign** (and confidence, if available).

- **Evaluation (Notebook):**  
  Run the **Evaluate** cell → see **Accuracy, Precision, Recall, F1**, and a **Confusion Matrix** visualization.
