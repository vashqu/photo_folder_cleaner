# 🧹 Image Cleanup Pipeline

This repository contains a Jupyter notebook that helps you automatically clean up folders of images.  
It combines duplicate detection with AI-powered classification (OpenAI’s CLIP model) to flag unwanted images such as screenshots, memes, tickets, and product photos, while keeping personal photos like portraits, selfies, and travel shots safe.

---

## ✨ Features
- Detects duplicate images using fast MD5 hashing.
- Classifies images with OpenAI CLIP using natural text prompts.
- Supports both **delete categories** (e.g., memes, screenshots, tickets) and **keep categories** (e.g., portraits, selfies, landscapes).
- Previews up to 3 sample images per category with similarity scores before any deletion.
- Uses progress bars (`tqdm`) and summary reports for clarity.
- Safely moves flagged images into a `trash/` folder instead of deleting permanently.

---
## 🚀 How to Use

Follow these steps to clean up your image folder:

1. **Clone this repository**
   ```bash
   git clone https://github.com/vashqu/image-cleanup-pipeline.git
   cd image-cleanup-pipeline

2. **Install dependencies**
   pip install -r requirements.txt

3. **Place clear_photos.ipynb inside the folder where your images are stored.**
4. **Run the cells in order**
5. **Take a quick look on the resulting trash folder: The model isn't perfect**
