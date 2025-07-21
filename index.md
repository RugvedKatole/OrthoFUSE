---
layout: default
---

<div style="max-width: 900px; margin: 0 auto; padding: 20px; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;">

<div style="text-align: center; margin-bottom: 40px;">
  <h1 style="font-size: 2.5em; color: #333; margin-bottom: 10px;">Ortho-Fuse</h1>
  <h2 style="font-size: 1.5em; color: #666; font-weight: normal; margin-bottom: 20px;">Orthomosaic Generation for Sparse High-Resolution AI-driven Health Maps through Optical Flow Estimation</h2>
</div>

<div style="text-align: center; margin: 30px 0;">
  <h3 style="color: #444; margin-bottom: 15px;">Authors</h3>
  <p style="font-size: 1.1em; margin-bottom: 20px;">
    <strong>Rugved Katole</strong>, <strong>Christopher Stewart</strong>
  </p>
</div>

<div style="text-align: center; margin: 30px 0;">
  <h3 style="color: #444; margin-bottom: 15px;">Links</h3>
  <p>
    <a href="https://arxiv.org/abs/your-paper-id" style="color: #1a73e8; text-decoration: none; margin: 0 15px;">Paper</a> |
    <a href="https://github.com/rugvedkatole/OrthoFUSE-Code" style="color: #1a73e8; text-decoration: none; margin: 0 15px;">Code</a> |
    <a href="https://drive.google.com/file/d/your-dataset-id/view" style="color: #1a73e8; text-decoration: none; margin: 0 15px;">Dataset</a>
  </p>
</div>

<div style="text-align: center; margin: 40px 0;">
  <img src="/assets/images/Generative_Ortho_Overview.png" alt="Ortho-Fuse Framework Overview" style="max-width: 100%; height: auto;">
  <p style="font-style: italic; color: #666; margin-top: 10px;">Framework Overview: Ortho-Fuse optical flow-based orthomosaic generation</p>
</div>

<div style="margin: 40px 0;">
  <h3 style="color: #333; border-bottom: 2px solid #eee; padding-bottom: 10px;">Abstract</h3>
  <p style="text-align: justify; line-height: 1.6; color: #444;">
    AI-driven crop health mapping systems offer substantial advantages over conventional monitoring approaches through accelerated data acquisition and cost reduction. However, widespread farmer adoption remains constrained by technical limitations in orthomosaic generation from sparse aerial imagery datasets. Traditional photogrammetric reconstruction requires 70-80% inter-image overlap to establish sufficient feature correspondences for accurate geometric registration. AI-driven systems operating under resource-constrained conditions cannot consistently achieve these overlap thresholds, resulting in degraded reconstruction quality that undermines user confidence in autonomous monitoring technologies.
  </p>
  <p style="text-align: justify; line-height: 1.6; color: #444;">
    In this paper we present Ortho-Fuse, an optical flow-based framework that enables reliable orthomosaic generation with reduced overlap requirements. Our approach employs intermediate flow estimation to synthesize transitional imagery between consecutive aerial frames, artificially augmenting feature correspondences for improved geometric reconstruction. Experimental validation demonstrates a <strong>20% reduction in minimum overlap requirements</strong>. We further analyze adoption barriers in precision agriculture to identify pathways for enhanced integration of AI-driven monitoring systems.
  </p>
</div>

<div style="text-align: center; margin: 40px 0;">
  <img src="/assets/images/RIFE_PIPELINE.drawio.png" alt="RIFE Pipeline Architecture" style="max-width: 100%; height: auto;">
  <p style="font-style: italic; color: #666; margin-top: 10px;">RIFE Pipeline: Real-time Intermediate Flow Estimation for synthetic frame generation</p>
</div>

<div style="margin: 40px 0;">
  <h3 style="color: #333; border-bottom: 2px solid #eee; padding-bottom: 10px;">Approach</h3>
  <p style="text-align: justify; line-height: 1.6; color: #444;">
    Our approach leverages the Real-time Intermediate Flow Estimation (RIFE) model to generate synthetic intermediate frames between consecutive aerial images. This process artificially increases the effective overlap between images, enabling standard orthomosaic reconstruction pipelines to operate successfully with reduced initial overlap requirements.
  </p>
  <p style="text-align: justify; line-height: 1.6; color: #444;">
    The framework consists of four key components: (1) <strong>Optical Flow Estimation</strong> using RIFE for synthetic frame generation, (2) <strong>Feature Enhancement</strong> to augment correspondences between sparse images, (3) <strong>Hybrid Reconstruction</strong> combining original and synthetic images, and (4) <strong>Quality Preservation</strong> maintaining visual fidelity essential for agricultural analysis.
  </p>
</div>

<div style="text-align: center; margin: 40px 0;">
  <img src="/assets/images/orthomosaic_comparison.png" alt="Orthomosaic Quality Comparison" style="max-width: 100%; height: auto;">
  <p style="font-style: italic; color: #666; margin-top: 10px;">Comparative orthomosaic quality: (a) Original 50% overlap, (b) Synthetic frames only, (c) Hybrid approach</p>
</div>

<div style="margin: 40px 0;">
  <h3 style="color: #333; border-bottom: 2px solid #eee; padding-bottom: 10px;">Results</h3>
  <p style="text-align: justify; line-height: 1.6; color: #444;">
    Experimental validation demonstrates superior reconstruction quality with our hybrid approach. The Ground Sample Distance (GSD) improved from 1.55cm (original) to 1.47cm (hybrid), while maintaining analytical accuracy for crop health assessment through NDVI analysis. Our method achieves a 20% reduction in minimum overlap requirements while preserving the visual reliability essential for farmer adoption.
  </p>
</div>

<div style="text-align: center; margin: 40px 0;">
  <img src="/assets/images/Health_map_comparison.png" alt="NDVI Health Map Comparison" style="max-width: 100%; height: auto;">
  <p style="font-style: italic; color: #666; margin-top: 10px;">NDVI crop health maps: (a) Original orthomosaic NDVI, (b) Synthetic orthomosaic NDVI, (c) Hybrid orthomosaic NDVI</p>
</div>

<div style="text-align: center; margin: 40px 0;">
  <img src="/assets/images/innovation_vs_adoption_tred.png" alt="Innovation vs Adoption Trend" style="max-width: 100%; height: auto;">
  <p style="font-style: italic; color: #666; margin-top: 10px;">Trends in AI innovations in Digital Agriculture vs. actual farmer adoption</p>
</div>

<div style="margin: 40px 0;">
  <h3 style="color: #333; border-bottom: 2px solid #eee; padding-bottom: 10px;">BibTeX</h3>
  <pre style="background-color: #f5f5f5; padding: 15px; border-radius: 5px; overflow-x: auto; font-family: 'Courier New', monospace; font-size: 0.9em;">
@article{katole2025orthofuse,
  title={Ortho-Fuse: Orthomosaic Generation for Sparse High-Resolution AI-driven Health Maps through Optical Flow Estimation},
  author={Katole, Rugved and Stewart, Christopher},
  journal={Under Review},
  year={2025}
}
  </pre>
</div>

</div>