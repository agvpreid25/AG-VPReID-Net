<div align="center">
<h1>AG-VPReID: A Challenging Large-Scale Benchmark for Aerial-Ground Video-based Person Re-Identification</h1>

<div>
<a href="https://openreview.net/profile?id=~Huy_Nguyen7" target="_blank">Huy Nguyen</a><sup>1</sup>,
<a href="https://openreview.net/profile?id=~Kien_Nguyen1" target="_blank">Kien Nguyen</a><sup>1</sup>,
<a href="https://openreview.net/profile?id=~Akila_Pemasiri1" target="_blank">Akila Pemasiri</a><sup>1</sup>,
<a href="https://openreview.net/profile?id=~Feng_Liu7" target="_blank">Feng Liu</a><sup>2</sup>,
<a href="https://openreview.net/profile?id=~Sridha_Sridharan1" target="_blank">Sridha Sridharan</a><sup>1</sup>,
<a href="https://openreview.net/profile?id=~Clinton_Fookes1" target="_blank">Clinton Fookes</a><sup>1</sup>
</div>

<div>
<sup>1</sup>School of Electrical Engineering and Robotics, Queensland University of Technology&emsp;
<sup>2</sup>Department of Electrical and Computer Engineering, Drexel University
</div>

**CVPR 2025**

<img src="assets/dataset_preview.png" width="75%"/>

AG-VPReID is a comprehensive benchmark dataset for aerial-ground video-based person re-identification, offering unprecedented scale and diversity with footage from drones (15-120m altitude), CCTV cameras, and wearable devices.

[arXiv](https://arxiv.org/abs/2503.08121) | [paper](#) | [dataset](https://drive.google.com/drive/folders/1wtdhKzK9Fbj7xkGAM84KNJ1uYCxSMHdj?usp=sharing)
</div>

## Key Features

- **The largest aerial-ground video dataset** with 6,632 identities, 32,321 tracklets, and 9.6 million frames
- **Multiple platforms** combining aerial drones (at various altitudes: 15m, 30m, 80m, 120m), CCTV cameras, and wearable cameras
- **Rich annotations** including clothing changes and 15 soft-biometric attributes
- **Real-world challenges** including extreme viewpoint variations, scale differences, and occlusions
- **Diverse environments** with outdoor campus scenes captured over 20 days

## AG-VPReID-Net Framework

We propose AG-VPReID-Net, a three-stream architecture specifically designed for aerial-ground person ReID:

1. **Adapted Temporal-Spatial Stream** addressing motion pattern inconsistencies and temporal feature learning
2. **Normalized Appearance Stream** using physics-informed techniques to tackle resolution and appearance changes
3. **Multi-Scale Attention Stream** handling scale variations across drone altitudes

## Performance

### Comparison with State-of-the-Art Methods

| Method | MARS<br>(mAP/R-1) | LS-VID<br>(mAP/R-1) | iLIDS-VID<br>(R-1) | G2A-VReID<br>(mAP/R-1) | AG-VPReID (A2G)<br>(mAP/R-1) | AG-VPReID (G2A)<br>(mAP/R-1) |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| LSTRL | 86.8/91.6 | 82.4/89.8 | 92.2 | - | 61.7/71.3 | 56.7/66.5 |
| CLIP-ReID | 88.1/91.7 | 80.6/88.8 | - | - | 62.3/71.6 | 57.2/66.8 |
| **AG-VPReID-Net** | **91.5/93.2** | **87.3/93.2** | **96.3** | **81.3/73.1** | **64.0/71.9** | **58.0/75.6** |

### Performance Across Drone Altitudes

| Stream | 15m<br>(A2G/G2A) | 30m<br>(A2G/G2A) | 80m<br>(A2G/G2A) | 120m<br>(A2G/G2A) |
|:---:|:---:|:---:|:---:|:---:|
| Stream 1 | 80.28/83.25 | 78.76/83.03 | 67.24/67.07 | 52.47/62.31 |
| Stream 2 | 69.75/72.87 | 68.13/71.41 | 52.62/52.22 | 38.12/45.43 |
| Stream 3 | 74.25/77.18 | 74.01/78.91 | 52.53/56.59 | 35.13/52.56 |
| **Combined** | **80.66/83.92** | **79.00/83.66** | **67.63/67.82** | **53.00/63.32** |

## Dataset Access

The AG-VPReID dataset is available at [Download Link](https://drive.google.com/drive/folders/1wtdhKzK9Fbj7xkGAM84KNJ1uYCxSMHdj?usp=sharing).

## Citation

If you use our dataset or code in your research, please cite our paper:

```bibtex
@inproceedings{nguyen2025agvpreid,
  title={AG-VPReID: A Challenging Large-Scale Benchmark for Aerial-Ground Video-based Person Re-Identification},
  author={Nguyen, Huy and Nguyen, Kien and Pemasiri, Akila and Liu, Feng and Sridharan, Sridha and Fookes, Clinton},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year={2025}
}
```
</div>
