# PAN Card Tampering Detection (Educational Project)

Detects potential tampering in PAN card images using basic computer vision checks (e.g., alignment + difference scoring + highlighting suspicious regions).

> **Disclaimer:** Educational/demo project only. Not production identity verification.

## Demo (recommended)
- Add 1–2 screenshots/GIFs here:
  - Original vs Suspected
  - Output with highlighted differences + score

## How it works (high level)
1. Load **reference** image and **suspected** image  
2. Preprocess (resize, grayscale, blur/denoise)
3. Align images (optional but strongly recommended)
4. Compute difference map + similarity score (e.g., SSIM or pixel diff)
5. Threshold + contour detection to highlight changed regions
6. Output score + “tampered / not tampered” decision

## Tech Stack
- Python
- OpenCV (cv2)
- NumPy
- (Optional) scikit-image for SSIM
- (Optional) scikit-learn for classification

## Project Structure
pancard-tampering-main/
  app.py (or main.py)
  utils/
  sample_data/
  requirements.txt
  README.md

## Setup
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
pip install -r requirements.txt
