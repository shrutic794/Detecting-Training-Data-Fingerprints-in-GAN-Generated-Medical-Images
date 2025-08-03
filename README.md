#  Detecting Training Data Fingerprints in GAN-Generated Medical Images

##  Overview
This project explores the **privacy risks and data leakage potential** in medical image synthesis using **Generative Adversarial Networks (GANs)**. Specifically, it investigates whether **"fingerprints"** from training data—such as distinctive patterns or artifacts—persist in GAN-generated outputs and can be traced back to real patient data. The work aligns with the growing concern around **model memorization**, **synthetic data reuse**, and **regulatory compliance in medical AI**.

---

##  Objectives
- Assess whether GANs unintentionally retain identifiable patterns from their training images.
- Detect and visualize **fingerprints** using statistical, perceptual, and deep feature similarity metrics.
- Evaluate potential privacy risks associated with publishing synthetic medical datasets.

---

##  Methodology
- **GAN Models**: Use or fine-tune models like StyleGAN, DCGAN on medical datasets (e.g., chest X-rays, skin lesions).
- **Feature Extraction**:
  - Structural Similarity Index (SSIM)
  - L2 pixel-level distance
  - Deep embeddings (VGG, ResNet-based)
- **Fingerprint Matching**:
  - Compare synthetic images to the training set using cosine similarity in embedding space
  - Identify overrepresented or memorized samples
- **Visualization**: t-SNE/PCA plots for clustering of real vs. synthetic data

---

