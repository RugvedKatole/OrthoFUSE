---
layout: default
---

<!-- Hero Section -->
<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/images/Generative_Ortho_Overview.png" alt="Ortho-Fuse Framework Overview" style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

<!-- Action Buttons -->
<div style="text-align: center; margin: 2rem 0;">
  <a href="{{ site.download_links.code }}" class="btn" style="background: linear-gradient(120deg, #2c3e50 0%, #34495e 100%); color: white; padding: 15px 30px; margin: 10px; text-decoration: none; border-radius: 5px; display: inline-block; font-weight: bold; transition: transform 0.2s;">
    📁 View Code Repository
  </a>
  <a href="{{ site.download_links.dataset }}" class="btn" style="background: linear-gradient(120deg, #27ae60 0%, #2ecc71 100%); color: white; padding: 15px 30px; margin: 10px; text-decoration: none; border-radius: 5px; display: inline-block; font-weight: bold; transition: transform 0.2s;">
    💾 Download Dataset
  </a>
</div>

## 🔬 Abstract

AI-driven crop health mapping systems offer substantial advantages over conventional monitoring approaches through **accelerated data acquisition** and **cost reduction**. However, widespread farmer adoption remains constrained by technical limitations in orthomosaic generation from sparse aerial imagery datasets. 

Traditional photogrammetric reconstruction requires **70-80% inter-image overlap** to establish sufficient feature correspondences for accurate geometric registration. AI-driven systems operating under resource-constrained conditions cannot consistently achieve these overlap thresholds, resulting in degraded reconstruction quality that undermines user confidence in autonomous monitoring technologies.

> **Ortho-Fuse employs intermediate flow estimation to synthesize transitional imagery between consecutive aerial frames, artificially augmenting feature correspondences for improved geometric reconstruction.**

<div style="background: linear-gradient(120deg, #e74c3c 0%, #c0392b 100%); color: white; padding: 20px; border-radius: 10px; margin: 20px 0; text-align: center;">
  <h3 style="margin: 0; color: white;">🎯 Key Result</h3>
  <h2 style="margin: 10px 0; color: white;">20% Reduction in Minimum Overlap Requirements</h2>
</div>

## 🚀 Key Innovation

The core innovation lies in using the **Real-time Intermediate Flow Estimation (RIFE)** model for temporal interpolation of synthetic images between aerial images, enhancing overlapping features between sparse data samples.

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 30px 0;">
  <div style="background: #f8f9fa; padding: 20px; border-radius: 10px; border-left: 4px solid #3498db;">
    <h4>💡 Efficiency</h4>
    <p>Reduces data collection requirements by up to 20% while maintaining analytical accuracy</p>
  </div>
  <div style="background: #f8f9fa; padding: 20px; border-radius: 10px; border-left: 4px solid #e67e22;">
    <h4>🔧 Quality</h4>
    <p>Enables high-quality orthomosaics from reduced input data</p>
  </div>
  <div style="background: #f8f9fa; padding: 20px; border-radius: 10px; border-left: 4px solid #27ae60;">
    <h4>📊 Preservation</h4>
    <p>Preserves crop health analytical capabilities through NDVI analysis</p>
  </div>
  <div style="background: #f8f9fa; padding: 20px; border-radius: 10px; border-left: 4px solid #9b59b6;">
    <h4>🌱 Impact</h4>
    <p>Addresses the innovation-adoption gap in precision agriculture</p>
  </div>
</div>

## 🔬 Technical Framework

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/images/RIFE_PIPELINE.drawio.png" alt="RIFE Pipeline" style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

Ortho-Fuse addresses the fundamental limitation where traditional orthomosaic generation demands comprehensive coverage that negates AI efficiency gains. While AI models for crop health assessment can operate with coverage as low as **20% of a field** and achieve over **80% accuracy**, existing orthomosaic requirements demand extensive data collection.

### 🔧 Framework Components

1. **🌊 Optical Flow Estimation**: Uses RIFE model for generating synthetic intermediate frames
2. **✨ Feature Enhancement**: Artificially augments feature correspondences between sparse images  
3. **🔄 Hybrid Reconstruction**: Combines original and synthetic images for optimal results
4. **🎯 Quality Preservation**: Maintains visual fidelity essential for farmer adoption

## 📊 Experimental Results

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/images/orthomosaic_comparison.png" alt="Orthomosaic Quality Comparison" style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <p style="font-style: italic; margin-top: 10px;">Comparative orthomosaic quality: (a) Original 50% overlap, (b) Synthetic frames only, (c) Hybrid approach</p>
</div>

### 🎯 Quantitative Improvements

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin: 30px 0;">
  <div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 20px; border-radius: 10px; text-align: center;">
    <h3 style="margin: 0; color: white;">📏 GSD Improvement</h3>
    <h2 style="margin: 10px 0; color: white;">1.47cm</h2>
    <p style="margin: 0; color: white;">vs 1.55cm (original)</p>
  </div>
  <div style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); color: white; padding: 20px; border-radius: 10px; text-align: center;">
    <h3 style="margin: 0; color: white;">🎯 Overlap Reduction</h3>
    <h2 style="margin: 10px 0; color: white;">20%</h2>
    <p style="margin: 0; color: white;">Minimum requirements</p>
  </div>
  <div style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); color: white; padding: 20px; border-radius: 10px; text-align: center;">
    <h3 style="margin: 0; color: white;">🌱 NDVI Accuracy</h3>
    <h2 style="margin: 10px 0; color: white;">Preserved</h2>
    <p style="margin: 0; color: white;">Analytical capabilities</p>
  </div>
</div>

### 🌿 Crop Health Analysis

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/images/Health_map_comparison.png" alt="NDVI Health Map Comparison" style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <p style="font-style: italic; margin-top: 10px;">NDVI crop health maps: (a) Original orthomosaic NDVI, (b) Synthetic orthomosaic NDVI, (c) Hybrid orthomosaic NDVI</p>
</div>

## 🌍 Research Impact

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/images/innovation_vs_adoption_tred.png" alt="Innovation vs Adoption Trend" style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <p style="font-style: italic; margin-top: 10px;">Trends in AI innovations in Digital Agriculture vs. actual farmer adoption</p>
</div>

This work addresses the **critical disconnect** between AI system efficiency promises and traditional orthomosaic requirements, enabling practical deployment of cost-effective agricultural monitoring while ensuring trusted visualization outputs essential for widespread technology adoption.

## 👥 Research Team

<div style="background: #f8f9fa; padding: 30px; border-radius: 10px; margin: 30px 0;">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px;">
    <div style="text-align: center;">
      <h3>Rugved Katole</h3>
      <p style="color: #666;">Lead Researcher</p>
    </div>
    <div style="text-align: center;">
      <h3>Christopher Stewart</h3>
      <p style="color: #666;">Supervisor</p>
    </div>
  </div>
</div>

## 📝 Publication Status

<div style="background: linear-gradient(120deg, #a8edea 0%, #fed6e3 100%); padding: 20px; border-radius: 10px; margin: 20px 0; text-align: center;">
  <h3 style="margin: 0;">📄 Currently Under Review</h3>
  <p style="margin: 10px 0;">This framework represents a significant step toward resolving adoption barriers in precision agriculture by enabling reliable orthomosaic generation from sparse data while preserving the analytical accuracy farmers require for informed decision-making.</p>
</div>

---

<div style="text-align: center; margin: 40px 0; color: #666;">
  <p>🌱 <em>Bridging the gap between AI innovation and agricultural adoption</em> 🌱</p>
</div>