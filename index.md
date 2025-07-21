---
layout: home
---

# Ortho-Fuse: Orthomosaic Generation for Sparse High Resolution AI-driven Health Maps

Welcome to the Ortho-Fuse project! This research presents an optical flow-based framework that enables reliable orthomosaic generation with reduced overlap requirements for agricultural monitoring applications.

## Abstract

AI-driven crop health mapping systems offer substantial advantages over conventional monitoring approaches through accelerated data acquisition and cost reduction. However, widespread farmer adoption remains constrained by technical limitations in orthomosaic generation from sparse aerial imagery datasets. Traditional photogrammetric reconstruction requires 70-80% inter-image overlap to establish sufficient feature correspondences for accurate geometric registration. AI-driven systems operating under resource-constrained conditions cannot consistently achieve these overlap thresholds, resulting in degraded reconstruction quality that undermines user confidence in autonomous monitoring technologies.

Ortho-Fuse employs intermediate flow estimation to synthesize transitional imagery between consecutive aerial frames, artificially augmenting feature correspondences for improved geometric reconstruction. Experimental validation demonstrates a **20% reduction in minimum overlap requirements**.

## Key Innovation

The core innovation lies in using the Real-time Intermediate Flow Estimation (RIFE) model for temporal interpolation of synthetic images between aerial images, enhancing overlapping features between sparse data samples. This approach:

- **Reduces data collection requirements** by up to 20% while maintaining analytical accuracy
- **Enables high-quality orthomosaics** from reduced input data
- **Preserves crop health analytical capabilities** through NDVI analysis
- **Addresses the innovation-adoption gap** in precision agriculture

## Technical Approach

Ortho-Fuse addresses the fundamental limitation where traditional orthomosaic generation demands comprehensive coverage that negates AI efficiency gains. While AI models for crop health assessment can operate with coverage as low as 20% of a field and achieve over 80% accuracy, existing orthomosaic requirements demand extensive data collection.

### Framework Components

1. **Optical Flow Estimation**: Uses RIFE model for generating synthetic intermediate frames
2. **Feature Enhancement**: Artificially augments feature correspondences between sparse images  
3. **Hybrid Reconstruction**: Combines original and synthetic images for optimal results
4. **Quality Preservation**: Maintains visual fidelity essential for farmer adoption

## Results

Experimental validation using agricultural datasets demonstrates:

- **Improved Ground Sample Distance (GSD)**: 1.47cm (hybrid) vs 1.55cm (original)
- **Superior reconstruction quality** with reduced artifacts and better seamline integration
- **Preserved analytical accuracy** in NDVI-based crop health assessments
- **Enhanced adoption potential** by bridging efficiency and reliability requirements

## Research Impact

This work addresses the critical disconnect between AI system efficiency promises and traditional orthomosaic requirements, enabling practical deployment of cost-effective agricultural monitoring while ensuring trusted visualization outputs essential for widespread technology adoption.

## Authors

**Rugved Katole**, **Christopher Stewart**

## Publication

This research is currently under review. The framework represents a significant step toward resolving adoption barriers in precision agriculture by enabling reliable orthomosaic generation from sparse data while preserving the analytical accuracy farmers require for informed decision-making.