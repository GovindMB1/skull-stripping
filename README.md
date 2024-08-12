# Skull Stripping and Feature Extraction Methods

This repository contains implementations of various methods for skull stripping and feature extraction used in medical image processing. Below are the details of each method:

## Region Growth Morphological Operations

### Erosion
Erosion is a morphological operation that erodes the boundaries of foreground objects in an image. It is useful for removing small-scale noise and refining object shapes by shrinking the foreground. Erosion is applied using a structuring element that moves across the image.

### Dilation
Dilation is the counterpart to erosion. It adds pixels to the boundaries of objects in the image, helping to fill small holes and gaps in the foreground. Dilation expands the foreground by applying a structuring element, which improves object continuity and connectivity.

## Level Set Methods with Chan-Vese for Brain Extraction

### Level Set Methods
Level set methods are numerical techniques used for tracking interfaces and shapes within images. They evolve an initial contour to separate different regions based on intensity values. The Chan-Vese model is a specific level set method that facilitates accurate brain extraction from MRI scans by segmenting the brain tissue from the surrounding areas.

## Hybrid Method

The Hybrid Method combines multiple techniques for skull stripping to enhance accuracy. It integrates various approaches such as morphological operations, level set methods, and thresholding. This combined approach leverages the strengths of each individual technique to produce a more robust and precise skull stripping process.

## Brain Extraction Using Otsu's Thresholding with Noise Removal

### Otsu's Thresholding
Otsu's Thresholding is an automatic method for binarizing images by finding an optimal threshold value that separates the foreground (brain) from the background. This method minimizes intra-class variance of pixel intensity values, which enhances the distinction between brain tissue and non-brain regions.

### Noise Removal
Post-thresholding noise removal is applied to eliminate small artifacts and noise from the binary image. This step improves the clarity of brain extraction by removing unwanted small-scale variations, resulting in a cleaner and more accurate representation of brain tissue.

---
