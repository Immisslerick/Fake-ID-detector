# PAN Card Tampering Detection (Educational Project)

Detect potential tampering in PAN card images using basic computer vision / ML-style checks (e.g., comparing key regions, flagging suspicious edits, and generating a “tampered vs. untampered” style result).

> **Note:** This is an educational project to learn image preprocessing, feature extraction, and simple classification logic. It is **not** production-grade identity verification.

---

## What this project does
- Loads two images (an “original/reference” and a “suspected” PAN card image)
- Preprocesses images (resize, grayscale, noise reduction as needed)
- Compares image regions to detect differences that may indicate edits/tampering
- Outputs:
  - a tamper score / similarity score (if implemented)
  - a classification result (tampered / not tampered)
  - optional visual outputs (difference map / highlighted areas)

---

## Why I built it
I wanted a hands-on project that combines:
- image preprocessing and normalization
- detecting meaningful differences vs. noise
- building an end-to-end script that produces an interpretable result

---

## Tech stack
- Python
- OpenCV (`cv2`)
- NumPy
- (Optional) scikit-learn for classification, if included

---

## Project structure
