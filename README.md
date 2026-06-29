# clinical-vision-sandbox
# Visceral Vision v1.0: Core Diagnostic Radiological Matrix

An interactive, client-side web application designed to simulate real-time computer vision processing and feature map visualization for cross-sectional diagnostic imaging arrays, such as CT and MRI scans. Version 1.0 establishes a local pixel-manipulation pipeline, demonstrating how radiological data can be parsed into parallel tensor, contrast, and activation maps directly within a browser environment without backend dependencies.

Live Demo: https://miymiy8880.github.io/clinical-vision-sandbox/

## Project Objective
The goal of Visceral Vision v1.0 is to provide a lightweight, zero-latency prototype interface for multi-slice diagnostic visualization. By leveraging the HTML5 Canvas API, this project demonstrates real-time algorithmic filtering to simulate edge detection kernels, tissue contrast isolation, and neural network feature activation layers on radiological matrices.

## Key Features
- Zero-Dependency Pipeline: Powered entirely by native vanilla JavaScript and standard canvas rendering. No heavy machine learning frameworks or server-side rendering required for the UI simulation.
- Local Diagnostic Scan Ingestion: Features an interactive local file dropzone utilizing a FileReader architecture, allowing users to upload and test custom cross-sectional CT or MRI frames safely and instantly.
- Static Asset Fallback: Built-in error boundary handling to catch and resolve server pathing issues during deployment.

## The Architecture
The interface ingests a raw radiological scan input and splits it into three parallel image processing streams:

1. Layer 1.1 Edge Tensor Expansion (Sobel Kernel): Computes spatial gradients across the scan matrix to isolate organ boundaries, skeletal structures, and fine anatomical contours using a simulated Sobel convolution filter.
2. Layer 2.3 Contrast Map Highlight: Applies an intensity-thresholding layer to isolate specific tissue densities or contrast-enhanced pathways, outputting a high-contrast magenta binary segmentation overlay.
3. Layer 3.0 Feature Activation Density Map: Visualizes simulated deep learning layer activations as a multi-color density heatmap, highlighting high-frequency structural zones in red and yellow to track region-of-interest focus points.

## Getting Started

## Prerequisites
A modern web browser such as Chrome, Firefox, Safari, or Edge.

## Running Locally
1. Clone the repository to your machine.
2. Open index.html directly in your browser.
3. Drag and drop any cross-sectional CT or MRI frame into the Select Frame area to see the processing matrix extract the feature layers instantly.

## Getting Started

## Prerequisites
A modern web browser such as Chrome, Firefox, Safari, or Edge.

## Running Locally
1. Clone the repository to your machine.
2. Open index.html directly in your browser.
3. Drag and drop any diagnostic CT or MRI frame into the Select Frame area to see the pipeline process the pixels instantly.
