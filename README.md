# Sahil MTP Project: Single-Image 3D Reconstruction

## Overview

**Sahil MTP (Major Technical Project)** is an advanced computer vision system that reconstructs complete 3D models from single 2D input images. This project leverages state-of-the-art deep learning techniques to generate high-resolution 3D meshes with full 360-degree coverage and texture preservation.

## What Does It Do?

### Input
- A single 2D photograph or image of an object/scene

### Process
1. **Multi-view Synthesis**: Generates 12 photorealistic viewpoints from different angles
2. **Geometric Reasoning**: Applies epipolar geometry constraints for consistency
3. **3D Reconstruction**: Fuses all views into a unified 3D model
4. **Surface Refinement**: Smooths and optimizes the final mesh

### Output
- Complete 3D textured mesh (OBJ format)
- Preserved colors and texture from original image
- Clean, artifact-free surfaces
- Ready for visualization, animation, or 3D printing

## Technical Approach

### Core Technique: Diffusion-based Multi-view Generation

Instead of traditional stereo reconstruction, this project employs **conditional diffusion models** to intelligently imagine what the object looks like from different viewpoints:

