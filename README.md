# PCD Assignment 01 - Image Sampling

This repository contains our first Digital Image Processing assignment about down sampling and up sampling.
The sampling algorithms are implemented manually. We only use NumPy for array operations, Pillow for loading/saving images, and Matplotlib for displaying the results.

## Methods

For down sampling, we implement:

- Max
- Average
- Median

For up sampling, we implement:

- Nearest Neighbor
- Bilinear
- Bicubic

We use the same sampling factor for all images so the results can be compared more easily.

## Images

We use 10 test images:

```text
images/
├── brick.png
├── camera.png
├── chelsea.png
├── clock_motion.png
├── coffee.png
├── coins.png
├── moon.png
├── page.png
├── rocket.jpg
└── text.png
```

The images include both grayscale and RGB images, with different characteristics such as texture, text, edges, smooth areas, and natural objects.

## Comparison

Besides looking at the visual result, we also use Mean Squared Error (MSE) to compare the reconstructed image with the original image.
A smaller MSE means the reconstructed image is closer to the original.

For comparing the down-sampling methods, the results from Max, Average, and Median are enlarged again using the same Bicubic method.

For comparing the up-sampling methods, Nearest Neighbor, Bilinear, and Bicubic use the same low-resolution image produced by Average down sampling.