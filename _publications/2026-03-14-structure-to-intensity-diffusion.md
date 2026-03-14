---
title: "Structure-to-Intensity Diffusion for Adverse-Weather LiDAR Generation"
collection: publications
category: conferences
permalink: /publication/structure-to-intensity-diffusion-cvpr-2026
excerpt: "Adverse-weather LiDAR point cloud generation is challenged by complex weather-induced degradations. These degradations affect geometry and reflectance in fundamentally different ways, making joint modeling difficult and ambiguous, especially when diverse real-world training data is limited. To address this, we propose Structure-to-Intensity Diffusion (SiD), a diffusion-based framework that explicitly factorizes the denoising process at each time step: it first reconstructs the geometric structure, then conditions reflectance intensity denoising on the estimated structure. This structure-conditioned design decomposes the joint distribution, reduces modeling ambiguity, and leads to point clouds that are both geometrically coherent and radiometrically realistic. To mitigate data scarcity, we introduce Real-Prior Weather Simulation (RPWS), a degradation module that leverages real-world sensor statistics to synthesize physically plausible adverse-weather point clouds from clear scans. Extensive experiments demonstrate that, with similar model complexity, our approach outperforms the previous state-of-the-art in generating adverse-weather LiDAR scans with both structural and radiometric properties more closely aligned with real-world data."
date: 2026-03-14
venue: "Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)"
citation: "Peiyang Ni, et al. (2026). \"Structure-to-Intensity Diffusion for Adverse-Weather LiDAR Generation.\" In <i>Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)</i>."
---

## Abstract

Adverse-weather LiDAR point cloud generation is challenged by complex weather-induced degradations. These degradations affect geometry and reflectance in fundamentally different ways, making joint modeling difficult and ambiguous, especially when diverse real-world training data is limited. To address this, we propose Structure-to-Intensity Diffusion (SiD), a diffusion-based framework that explicitly factorizes the denoising process at each time step: it first reconstructs the geometric structure, then conditions reflectance intensity denoising on the estimated structure. This structure-conditioned design decomposes the joint distribution, reduces modeling ambiguity, and leads to point clouds that are both geometrically coherent and radiometrically realistic. To mitigate data scarcity, we introduce Real-Prior Weather Simulation (RPWS), a degradation module that leverages real-world sensor statistics to synthesize physically plausible adverse-weather point clouds from clear scans. Extensive experiments demonstrate that, with similar model complexity, our approach outperforms the previous state-of-the-art in generating adverse-weather LiDAR scans with both structural and radiometric properties more closely aligned with real-world data.

## BibTeX

```bibtex
@inproceedings{ni2026structure,
  title     = {Structure-to-Intensity Diffusion for Adverse-Weather LiDAR Generation},
  author    = {Ni, Peiyang and others},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2026}
}
```
