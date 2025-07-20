# OrthoFUSE: Generative Orthomosaics with Enhanced Frame Interpolation

OrthoFUSE is an advanced research project that leverages state-of-the-art frame interpolation techniques for generating high-quality orthomosaic imagery. This project builds upon the robust foundation of [Practical-RIFE](https://github.com/hzwer/Practical-RIFE) to create innovative solutions for aerial imagery processing and orthomosaic generation.

## 🚀 Features

- **Enhanced Frame Interpolation**: Utilizes the latest RIFE (Real-time Intermediate Flow Estimation) models for superior video frame interpolation
- **Orthomosaic Generation**: Specialized algorithms for creating seamless orthomosaic images from aerial footage
- **Multi-Scale Processing**: Support for various resolution inputs including 4K video processing
- **Batch Processing**: Efficient handling of large datasets with optimized workflows
- **Video Enhancement**: Advanced video super-resolution capabilities using SAFA (Scale-Adaptive Feature Aggregation)

## 📋 Requirements

- Python <= 3.11
- CUDA-compatible GPU (recommended for optimal performance)
- See `requirements.txt` for detailed dependencies

## 🛠️ Installation

```bash
git clone https://github.com/RugvedKatole/OrthoFUSE.git
cd OrthoFUSE
pip3 install -r requirements.txt
```

Download the latest model from the [trained models section](#trained-models) and place the model files in the `train_log/` directory.

## 🎯 Usage

### Basic Frame Interpolation

Generate 2X interpolated video:
```bash
python3 inference_video.py --multi=2 --video=input_video.mp4
```

Generate 4X interpolated video:
```bash
python3 inference_video.py --multi=4 --video=input_video.mp4
```

For high-resolution videos (4K):
```bash
python3 inference_video.py --multi=2 --video=input_video.mp4 --scale=0.5
```

### Processing Image Sequences

Process PNG sequences for orthomosaic generation:
```bash
python3 inference_video.py --multi=4 --img=input_images/
```

### Video Enhancement

Apply video super-resolution:
```bash
python3 inference_video_enhance.py --video=input_video.mp4
```

### Parameter Reference

- `--img` / `--video`: Input file or directory path
- `--output`: Output video filename (e.g., 'processed_video.mp4')
- `--model`: Directory containing trained model files
- `--UHD`: Equivalent to setting scale=0.5 for ultra-high definition
- `--montage`: Create side-by-side comparison with original
- `--fps`: Manually set output frame rate
- `--ext`: Output video format (default: mp4)
- `--multi`: Frame rate interpolation multiplier
- `--exp`: Set --multi to 2^(--exp)
- `--scale`: Resolution scaling factor (default: 1.0)

## 📊 Trained Models

### Latest Recommended Models

**4.26** - 2024.09.21 | [Google Drive](https://drive.google.com/file/d/1gViYvvQrtETBgU1w8axZSsr7YUuw31uy/view?usp=sharing)

**4.25** - 2024.09.19 | [Google Drive](https://drive.google.com/file/d/1ZKjcbmt1hypiFprJPIKW0Tt0lr_2i7bg/view?usp=sharing) | Enhanced anime scene processing

**4.22** - 2024.08.08 | [Google Drive](https://drive.google.com/file/d/1qh2DSA9a1eZUTtZG9U9RQKO7N7OaUJ0_/view?usp=share_link) | Optimized for general use

For the complete model history and additional versions, please refer to the [original Practical-RIFE repository](https://github.com/hzwer/Practical-RIFE).

## 🔬 Research Applications

OrthoFUSE is designed for:
- Aerial survey data processing
- Drone footage enhancement
- Agricultural monitoring systems
- Environmental research applications
- Geographic information systems (GIS)
- Remote sensing data analysis

## 🏗️ Architecture

This project incorporates cutting-edge research from:
- **RIFE**: Real-Time Intermediate Flow Estimation for Video Frame Interpolation
- **SAFA**: Scale-Adaptive Feature Aggregation for Video Super-Resolution
- Custom orthomosaic generation algorithms optimized for aerial imagery

## 📚 Citation

If you use OrthoFUSE in your research, please cite this work along with the original RIFE and SAFA papers:

```bibtex
@misc{orthofuse2024,
  title={OrthoFUSE: Generative Orthomosaics with Enhanced Frame Interpolation},
  author={Rugved Katole},
  year={2024},
  url={https://github.com/RugvedKatole/OrthoFUSE}
}

@inproceedings{huang2022rife,
  title={Real-Time Intermediate Flow Estimation for Video Frame Interpolation},
  author={Huang, Zhewei and Zhang, Tianyuan and Heng, Wen and Shi, Boxin and Zhou, Shuchang},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  year={2022}
}

@inproceedings{huang2024safa,
  title={Scale-Adaptive Feature Aggregation for Efficient Space-Time Video Super-Resolution},
  author={Huang, Zhewei and Huang, Ailin and Hu, Xiaotao and Hu, Chen and Xu, Jun and Zhou, Shuchang},
  booktitle={Winter Conference on Applications of Computer Vision (WACV)},
  year={2024}
}
```

## 🤝 Contributing

We welcome contributions to OrthoFUSE! Please feel free to submit issues, feature requests, or pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Practical-RIFE](https://github.com/hzwer/Practical-RIFE) for the foundational frame interpolation framework
- [SAFA](https://github.com/megvii-research/WACV2024-SAFA) for video enhancement capabilities
- The computer vision research community for advancing the field of video processing

## 📞 Contact

For questions, suggestions, or collaboration opportunities, please open an issue on this repository.

---

**Note**: This project builds upon existing open-source research. All original licensing terms and attributions are preserved and respected.