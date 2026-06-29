# clinical-vision-sandbox
# Visceral Vision v1.0: Core Diagnostic Radiological Matrix

An interactive, client-side web application designed to simulate real-time computer vision processing for multi-slice diagnostic imaging arrays, including CT and MRI scans. Version 1.0 establishes the fundamental pixel-manipulation matrix, demonstrating how cross-sectional radiological inputs can be parsed into actionable semantic layers directly within a browser environment without backend dependencies.

Live Demo: https://miymiy8880.github.io/clinical-vision-sandbox/

## Project Objective
The goal of Visceral Vision v1.0 is to provide a lightweight, zero-latency prototype interface for multi-task neuroimaging and body diagnostics. By leveraging the HTML5 Canvas API, this project demonstrates real-time algorithmic filtering to simulate three critical diagnostic AI tasks: tissue/lesion boundary segmentation, structural criticality mapping, and automated trajectory planning.

## Key Features
- Zero-Dependency Pipeline: Powered entirely by native vanilla JavaScript and standard canvas rendering. No heavy machine learning frameworks or server-side rendering required for the UI simulation.
- Local Diagnostic Scan Ingestion: Features an interactive local file dropzone utilizing a FileReader architecture, allowing users to upload and test custom CT or MRI frames safely and instantly.
- Static Asset Fallback: Built-in error boundary handling to catch and resolve server pathing issues during deployment.

## The Architecture
The interface ingests a raw cross-sectional scan input and splits it into three parallel diagnostic streams:

1. Task 1: Tissue Segmentation. Simulates semantic segmentation via intensity-threshold parsing to isolate pathological margins, organ structures, or target zones.
2. Task 2: Structural Criticality Map. Generates a simulated depth and safety heatmap highlighting high-risk anatomical boundaries, vital organs, or major vascular pathways nearby.
3. Task 3: Vector Route Prediction. Automatically superimposes an optimized, AI-predicted trajectory for biopsy routes, radiation targeting, or surgical entry planes.

## Getting Started

## Prerequisites
A modern web browser such as Chrome, Firefox, Safari, or Edge.

## Running Locally
1. Clone the repository to your machine.
2. Open index.html directly in your browser.
3. Drag and drop any diagnostic CT or MRI frame into the Select Frame area to see the pipeline process the pixels instantly.
