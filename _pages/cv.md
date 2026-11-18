---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
show_page_title: false
redirect_from:
  - /resume
---

{% include base_path %}

Research Interests
======
Generative modeling for 3D perception and physical scene understanding, with interests in sensor simulation, conditional reconstruction, and world modeling.

Education
======
* **University of Electronic Science and Technology of China (UESTC)**, Chengdu, China
  * *M.Eng. in Computer Science*, 2024 -- 2027 (expected)
  * GPA: 3.98 / 4.00 ｜ **National Scholarship** ｜ Outstanding Graduate
  * Advisors: Prof. [Ping Hu](https://feinanshan.github.io/) and Prof. [Xiaofeng Zhu](https://scholar.google.com/citations?user=-bk1CrcAAAAJ)
* **Guilin University of Electronic Technology (GUET)**, Guilin, China
  * *B.Eng. in Computer Science*, 2020 -- 2024
  * Weighted Average: 89.8 / 100 ｜ **National Scholarship** ｜ Outstanding Graduate (Provincial-level)

English Proficiency
======
* **TOEFL iBT**: **100/120** (Overall 5.0/6.0; Reading 5.0, Listening 5.0, Speaking 4.5, Writing 5.5; CEFR C1; Sept. 30, 2026)

Publications
======
<ul class="cv-list-publications">
{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

Selected Research Experience
======
* **A2CFlow: Range-Aware Rectified Flow for LiDAR Restoration** *(UESTC, Primary Researcher, 2026)*
  * Formulated adverse-weather restoration as conditional rectified flow, jointly suppressing false returns and reconstructing missing range and reflectance from a single LiDAR scan.
  * Developed physically motivated Range-Aware Flow Scheduling (RAFS) using range and return validity, strengthening structural supervision through cleaner training states and refining weakly observed geometry through denser late-stage local-time sampling, without additional network evaluations.
  * Transferred RAFS gains to a two-step model using ReFlow and timestep distillation, improving segmentation mIoU over conditional R2Flow by 6.15 points on Adverse-KITTI and 1.42 points on real SemanticSTF scans without fine-tuning.

* **Structure-to-Intensity Diffusion for Adverse-Weather LiDAR Generation** *(UESTC, Primary Researcher, 2025)*
  * Recognized the asymmetric physical relationship between LiDAR geometry and reflectance; translated it into SiD, a factorized diffusion process that denoises structure first and then generates reflectance conditioned on the recovered structure.
  * Developed Real-Prior Weather Simulation (RPWS) from real sensor statistics, modeling range-dependent attenuation, structured occlusion, and reflectance distortion. SiD reduced Fréchet Point Distance versus WeatherGen by 62.0% in fog, 26.1% in rain, and 45.4% in snow on STF.

* **Taming Stable Diffusion for LiDAR Point-Cloud Generation** *(UESTC, Primary Researcher, 2024)*
  * Identified the mismatch between image-generation priors and rotating-LiDAR sensing; reformulated acquisition as 2.5D equirectangular range imaging to transfer visual priors while preserving the sensor's measurement geometry.
  * Incorporated panoramic-diffusion mechanisms that enforce azimuthal wrap-around continuity, making the generative process compatible with the structure of 360-degree scans.

Selected Honors and Awards
======
* Outstanding Graduate, *University of Electronic Science and Technology of China*, 2027
* **National Scholarship for Graduate Students**, *Ministry of Education of China*, 2026
* Outstanding Graduate (Provincial-level), *Guangxi Zhuang Autonomous Region*, 2024
* **National Scholarship for Undergraduate Students**, *Ministry of Education of China*, 2023
* CASC Scholarship (Third Prize), *China Aerospace Science and Technology Corporation*, 2022
* Guangxi Zhuang Autonomous Region People's Government Scholarship, 2021

Academic Service
======
* **Conference Reviewer**: CVPR, PRCV, VCIP
* **Journal Reviewer**: IEEE Robotics and Automation Letters (RA-L)
