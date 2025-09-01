# ✍️ Signature Verification System (Siamese Network + ORB Hybrid)

This project implements an **Signature verification system** using a **Siamese Neural Network (SNN)** combined with **ORB (Oriented FAST and Rotated BRIEF) feature matching**.  
The model takes a **pair of signature images** as input and predicts whether the second signature is **Genuine** or **Forged** compared to the first one.  

---

## 🔍 Features
- 🧠 **Deep Learning Approach (SNN):** Learns discriminative embeddings for signatures.  
- 🔑 **ORB Feature Matching:** Captures local keypoints & descriptors.  
- ⚡ **Hybrid Decision:** Combines deep embeddings + ORB similarity for robust verification.  
- 📊 **Benchmark Results after 10 Epochs:**
  - AUC: **0.9410**  
  - Accuracy: **87.12%**  
  - Precision: **85.44%**  
  - Recall: **89.50%**  
  - F1-score: **87.42%**  
- ✅ Works **offline** (once model is trained).  
- 📂 Built and trained entirely in **Google Colab**.  

---

## 📂 Dataset
- The project uses the **CEDAR Signature Dataset** (offline handwritten signatures).  
- Dataset contains **genuine** and **forged** signature images per subject.  
- Images are preprocessed:
  - Converted to grayscale
  - Resized to fixed dimensions
  - Normalized for CNN training


## 📂 Input & Output
### Input  
- A **pair of grayscale signature images** (`img1`, `img2`)  

### Output  
- **Decision:** `Genuine` or `Forged`  
- **Deep Distance (SNN):** embedding similarity score  
- **ORB Match %** (if hybrid is used)  
- **Final Score** (hybrid fusion metric)  


### 🔗 Open in Colab

Click the badge   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO_NAME/blob/main/MNIST_CNN.ipynb)   in the `Signature_Verification_system_02.ipynb` to run it directly in Colab.

## ⚙️ Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/Raunak22-Dev/Signature_Verification_System_USING_SNN.git
cd Signature_Verification_System_02
```

## 📜 License
- This project is licensed under the MIT License.
