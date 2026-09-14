# RGB Image Processing Library & k-NN Image Classifier

**Course:** DSC 20 (Programming and Basic Data Structures for Data Science), UC San Diego — Mid-Quarter Project
**Team:** Sai Poornasree Balamurugan, Catherine Back

## Overview
An object-oriented image-processing library built from scratch in Python, plus a k-nearest-neighbors image classifier implemented without any machine learning libraries.

## Features
- **`RGBImage`** — core data structure representing an image as pixel data across 3 color channels.
- **Standard image processing:** negate, grayscale, rotate 180°.
- **Premium image processing:** chroma-key compositing (green-screen style background replacement), sticker overlay.
- Processing methods are organized using a template-method class hierarchy (`StandardImageProcessing` vs. `PremiumImageProcessing`), so shared logic lives in one place and each tier only implements what's different.
- **k-NN image classifier** — implemented from scratch (no scikit-learn) to classify images by comparing them against labeled training examples.

## Tech
Python, NumPy, PIL

## Files
- `midqtr_project.py` — core library: `RGBImage`, image processing classes, k-NN classifier
- `midqtr_project_runner.py` — example/runner script
- `*.png` — sample images used for testing processing methods and the classifier (gradients, chroma-key backgrounds, sticker assets)

## Skills demonstrated
Object-oriented design (template method pattern), algorithm implementation from scratch, machine learning fundamentals (k-NN), unit testing/doctests
