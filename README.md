# Implicit Neural Representation in Medical Imaging: A Comparative Survey <br> <span style="float: right"><sub><sup>$\text{(\textcolor{#15babc}{ICCV 2023 CVAMD Workshop})}$</sup></sub></span> 


[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)

:fire::fire: This is a collection of awesome articles about Implicit Neural Representation networks in medical imaging:fire::fire:

:loudspeaker: Our review paper published on arXiv: [Implicit Neural Representation in Medical Imaging: A Comparative Survey](https://arxiv.org/abs/2307.16142) :heart:

#### Citation

```python
@article{molaei2023implicit,
  title={Implicit Neural Representation in Medical Imaging: A Comparative Survey},
  author={Molaei, Amirali and Aminimehr, Amirhossein and Tavakoli, Armin and Kazerouni, Amirhossein and Azad, Bobby and Azad, Reza and Merhof, Dorit},
  journal={arXiv preprint arXiv:2307.16142},
  year={2023}
}
```

# Introduction 

Implicitly representing image signals has gained popularity in recent years for a broad range of medical imaging applications.
The most motivating reasons are the following:
* Memory efficiency: The amount of memory demanded to represent the signal is not restricted by the signal's resolution.
* Unlimited Resolution: They take values in the continuous domain, meaning they can generate values for coordinates in-between the pixel or voxel-wise grid
* Effective data usage: They can learn to handle reconstruction and synthesis tasks without high-cost external annotation.

Which all are significantly important for developing an automatic medical system.<br>
With the aim of providing easier access for researchers, this repo contains a comprehensive paper list of Implicit Neural Representations in Medical Imaging, including papers, codes, and related websites.<br>
We considered a sum of <ins>**76**</ins> research papers spanning from 2021 to 2023.

---
# Introductory Papers
**Implicit Neural Representations with Periodic Activation Functions.** [17th Jun., 2020] [Advances in Neural Information Processing Systems, 2020]<br>
*Vincent Sitzmann, Julien N. P. Martel, Alexander W. Bergman, David B. Lindell, Gordon Wetzstein.*<br>
 [[PDF](https://arxiv.org/abs/2006.09661)]

**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis.** [19th Mar., 2020] [Communications of the ACM, 2021]<br>
*Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, Ren Ng.*<br>
[[PDF](https://dl.acm.org/doi/abs/10.1145/3503250)]

---
# Main papers
<img src="Figures/Taxonomy.png" alt="Taxonomy" width="816">
Here, we taxonomize studies that integrate implicit representations into building medical analysis models.<br>

<details>
<summary>Image Reconstruction</summary>

- [Tomography and CT](#tomography-and-ct)
- [MRI](#mri)
- [Ultrasound](#ultrasound)
- [Dental and Maxillofacial](#dental-and-maxillofacial)
- [General and Miscellaneous](#general-and-miscellaneous)

</details>

<details>
<summary>Image Segmentation</summary>

- [Brain Structures and Lesions](#brain-structures-and-lesions)
- [Cardiac and Heart Structures](#cardiac-and-heart-structures)
- [Retinal Blood Vessels](#retinal-blood-vessels)
- [3D Segmentation](#3d-segmentation)
- [Boundary Refinement](#boundary-refinement)
- [Patch Level Segmentation](#patch-level-segmentation)

</details>

<details>
<summary>Image Registration</summary>

- [Deformable Registration](#deformable-registration)
- [Diffeomorphic Registration](#diffeomorphic-registration)

</details>
- [Neural Rendering](#neural-rendering)
  - [Reconstruction from Limited or Sparse Views](#reconstruction-from-limited-or-sparse-views)
    - [Computed Tomography (CT)](#computed-tomography-ct)
    - [Cone Beam Computed Tomography (CBCT)](#cone-beam-computed-tomography-cbct)
    - [Magnetic Resonance Imaging (MRI)](#magnetic-resonance-imaging-mri)
    - [Digital Subtraction Angiography (DSA)](#digital-subtraction-angiography-dsa)
  - [Surgical Scene Reconstruction](#surgical-scene-reconstruction)
    - [Robotic Surgery](#robotic-surgery)
    - [Endoscopic Surgery](#endoscopic-surgery)
  - [Dental and Oral Imaging](#dental-and-oral-imaging)
  - [Pose Estimation](#pose-estimation)
- [Image Compression](#image-compression)
- [Image Synthesis](#image-synthesis)

(Each section is ordered by the publication dates)
<img src="Figures/Reconstruction.jpg" alt="reconstruction" width="1000" height="5"><br>

## Image Reconstruction

---

### Tomography and CT

1. 📜 **IntraTomo: Self-supervised Learning-based Tomography via Sinogram Synthesis and Prediction**
   - 🗓️ Publication Date: 9th Feb. 2021
   - 📖 Proceedings: IEEE/CVF International Conference on Computer Vision, 2021
   - 🧑‍🔬 Authors: Guangming Zang, Ramzi Idoughi, Rui Li, Peter Wonka, Wolfgang Heidrich
   - 📄 [Download PDF](https://neuralfields.cs.brown.edu/paper_243.html)

2. 📜 **CoIL: Coordinate-based Internal Learning for Imaging Inverse Problems**
   - 🗓️ Publication Date: 9th Feb. 2021
   - 📖 Journal: IEEE Transactions on Computational Imaging, 2021
   - 🧑‍🔬 Authors: Yu Sun, Jiaming Liu, Mingyang Xie, Brendt Wohlberg, Ulugbek S. Kamilov
   - 📄 [Download PDF](https://arxiv.org/abs/2102.05181)
   - 💻 [GitHub](https://github.com/wustl-cig/Cooridnate-based-I)

3. 📜 **Dynamic CT Reconstruction from Limited Views with Implicit Neural Representations and Parametric Motion Fields**
   - 🗓️ Publication Date: 23th Apr. 2021
   - 📖 Proceedings: IEEE/CVF International Conference on Computer Vision, 2021
   - 🧑‍🔬 Authors: Albert W. Reed, Hyojin Kim, Rushil Anirudh, K. Aditya Mohan, Kyle Champley, Jingu Kang, Suren Jayasuriya
   - 📄 [Download PDF](https://arxiv.org/abs/2104.11745)

4. 📜 **Neural Computed Tomography**
   - 🗓️ Publication Date: 17th Jan. 2022
   - 📖 Preprint: arXiv, 2022
   - 🧑‍🔬 Authors: Kunal Gupta, Brendan Colvert, Francisco Contijoch
   - 📄 [Download PDF](https://arxiv.org/abs/2201.06574)
   - 💻 [GitHub](https://github.com/KunalMGupta/DIFIR-CT)

5. 📜 **Streak artifacts reduction algorithm using an implicit neural representation in sparse-view CT**
   - 🗓️ Publication Date: 4th Apr. 2022
   - 📖 Conference: Medical Imaging 2022: Physics of Medical Imaging, 2022
   - 🧑‍🔬 Authors: Byeongjoon Kim, Hyunjung Shim, Jongduk Baek
   - 📄 [Download PDF](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/12031/120312N/Streak-artifacts-reduction-algorithm-using-an-implicit-neural-representation-in/10.1117/12.2610722.short)

6. 📜 **Self-Supervised Coordinate Projection Network for Sparse-View Computed Tomography**
   - 🗓️ Publication Date: 12th Sep. 2022
   - 📖 Journal: IEEE Transactions on Computational Imaging, 2023
   - 🧑‍🔬 Authors: Qing Wu, Ruimin Feng, Hongjiang Wei, Jingyi Yu, Yuyao Zhang
   - 📄 [Download PDF](https://ieeexplore.ieee.org/document/10143286)
   - 💻 [GitHub](https://github.com/iwuqing/SCOPE)

7. 📜 **OReX: Object Reconstruction from Planar Cross-sections Using Neural Fields**
   - 🗓️ Publication Date: 23th Nov. 2022
   - 📖 Conference: CVPR, 2023
   - 🧑‍🔬 Authors: Haim Sawdayee, Amir Vaxman, Amit H. Bermano
   - 📄 [Download PDF](https://arxiv.org/abs/2211.12886)
   - 💻 [GitHub](https://github.com/haimsaw/OReX)

8. 📜 **NeuRec: Incorporating Interpatient prior to Sparse-View Image Reconstruction for Neurorehabilitation**
   - 🗓️ Publication Date: 21th Feb. 2022
   - 📖 Journal: BioMed Research International, 2022
   - 🧑‍🔬 Authors: Cong Liu, Qingbin Wang, Jing Zhang
   - 📄 [Download PDF](https://www.hindawi.com/journals/bmri/2022/5426643/)

9. 📜 **MEPNet: A Model-Driven Equivariant Proximal Network for Joint Sparse-View Reconstruction and Metal Artifact Reduction in CT Images.**
   - 🗓️ Publication Date: 25th Jun. 2023
   - 📖 Preprint: arXiv
   - 🧑‍🔬 Authors: Hong Wang, Minghao Zhou, Dong Wei, Yuexiang Li, Yefeng Zheng
   - 📄 [PDF](https://ui.adsabs.harvard.edu/abs/2023arXiv230614274W/abstract)
   - 🖥️ [GitHub](https://github.com/hongwang01/mepnet)

10. 📜 **UncertaINR: Uncertainty Quantification of End-to-End Implicit Neural Representations for Computed Tomography**
    - 🗓️ Publication Date: 3rd Jun. 2022
    - 📖 Authors: Francisca Vasconcelos, Bobby He, Nalini Singh, Yee Whye Teh
    - 📄 [PDF](https://arxiv.org/abs/2202.10847)
    - 💻 [GitHub](https://github.com/bobby-he/uncertainr)

11. 📜 **Unsupervised Polychromatic Neural Representation for CT Metal Artifact Reduction**
    - 🗓️ Publication Date: 27th Jun. 2023
    - 📖 Preprint: arXiv
    - 🧑‍🔬 Authors: Qing Wu, Lixuan Chen, Ce Wang, Hongjiang Wei, S. Kevin Zhou, Jingyi Yu, Yuyao Zhang
    - 📄 [Download PDF](https://arxiv.org/abs/2306.15203)

12. 📜 **NAISR: A 3D Neural Additive Model for Interpretable Shape Representation**
    - 🗓️ Publication Date: 16th Mar. 2023
    - 📖 Preprint: arXiv
    - 🧑‍🔬 Authors: Yining Jiao, Carlton Zdanski, Julia Kimbell, Andrew Prince, Cameron Worden, Samuel Kirse, Christopher Rutter, Benjamin Shields, William Dunn
    - 📄 [Download PDF](https://arxiv.org/abs/2303.09234)
    - 💻 [GitHub](https://github.com/uncbiag/naisr)
   

<br>

---
### MRI

13. 📜 **An Arbitrary Scale Super-Resolution Approach for 3-Dimensional Magnetic Resonance Image using Implicit Neural Representation**
     - 🗓️ Publication Date: 29th Oct. 2021
     - 🧑‍🔬 Authors: Qing Wu, Yuwei Li, Yawen Sun, Yan Zhou, Hongjiang Wei, Jingyi Yu, Yuyao Zhang
     - 📄 [PDF]([Link to PDF](https://arxiv.org/abs/2110.14476))
     - 💻 [GitHub]([Link to GitHub](https://github.com/iwuqing/arssr))

14. 📜 **IREM: High-Resolution Magnetic Resonance (MR) Image Reconstruction via Implicit Neural Representation**
     - 🗓️ Publication Date: 29th Jun. 2021
     - 🧑‍🔬 Authors: Qing Wu, Yuwei Li, Lan Xu, Ruiming Feng, Hongjiang Wei, Qing Yang, Boliang Yu, Xiaozhao Liu, Jingyi Yu, Yuyao Zhang
     - 📄 [PDF](https://arxiv.org/abs/2106.15097)

15. 📜 **MRI Super-Resolution using Implicit Neural Representation with Frequency Domain Enhancement**
     - 🗓️ Publication Date: Aug. 2022
     - 🧑‍🔬 Authors: Shuangming Mao, Seiichiro Kamata
     - 📄 [PDF](https://dl.acm.org/doi/10.1145/3563737.3563759)

16. 📜 **NeSVoR: Implicit Neural Representation for Slice-to-Volume Reconstruction in MRI**
     - 🗓️ Publication Date: IEEE TRANSACTIONS ON MEDICAL IMAGING, 2022
     - 🧑‍🔬 Authors: Junshen Xu, Daniel Moyer, Borjan Gagoski, Juan Eugenio Iglesias, P. Ellen Grant, Polina Golland, Elfar Adalsteinsson
     - 📄 [PDF](https://www.techrxiv.org/articles/preprint/NeSVoR_Implicit_Neural_Representation_for_Slice-to-Volume_Reconstruction_in_MRI/21398868)
     - 💻 [GitHub](https://github.com/daviddmc/NeSVoR)

17. 📜 **Spatiotemporal implicit neural representation for unsupervised dynamic MRI reconstruction**
     - 🗓️ Publication Date: 31th Dec. 2022
     - 🧑‍🔬 Authors: Jie Feng, Ruimin Feng, Qing Wu, Zhiyong Zhang, Yuyao Zhang, Hongjiang Wei
     - 📄 [PDF](Link to PDF)

18. 📜 **Spatial Attention-based Implicit Neural Representation for Arbitrary Reduction of MRI Slice Spacing**
     - 🗓️ Publication Date: 23th May. 2022
     - 🧑‍🔬 Authors: Xin Wang, Sheng Wang, Honglin Xiong, Kai Xuan, Zixu Zhuang, Mengjun Liu, Zhenrong Shen, Xiangyu Zhao, Lichi Zhang, Qian Wang
     - 📄 [PDF](https://arxiv.org/abs/2301.00127)

19. 📜 **Neural Implicit k-Space for Binning-free Non-Cartesian Cardiac MR Imaging**
      - 🗓️ Publication Date: 16th Dec. 2022
      - 📖 Conference: International Conference on Information Processing in Medical Imaging, 2023
      - 🧑‍🔬 Authors: Wenqi Huang, Hongwei Li, Jiazhen Pan, Gastao Cruz, Daniel Rueckert, Kerstin Hammernik
      - 📄 [PDF](https://arxiv.org/abs/2212.08479)

20. 📜 **Continuous longitudinal fetus brain atlas construction via implicit neural representation**
     - 🗓️ Publication Date: 14th Sep. 2022
     - 🧑‍🔬 Authors: Lixuan Chen, Jiangjie Wu, Qing Wu, Hongjiang Wei, Yuyao Zhang
     - 📄 [PDF](https://arxiv.org/abs/2209.06413)

21. 📜 **Multi-contrast MRI Super-resolution via Implicit Neural Representations**
      - 🗓️ Publication Date: 27th Mar. 2023
      - 🧑‍🔬 Authors: Julian McGinnis, Suprosanna Shit, Hongwei Bran Li, Vasiliki Sideri-Lampretsa, Robert Graf, Maik Dannecker, Jiazhen Pan, Nil Stolt Ansö, Mark Mühlau, Jan S. Kirschke, Daniel Rueckert, Benedikt Wiestler
      - 📄 [PDF](https://arxiv.org/abs/2303.15065)
      - 💻 [GitHub](https://github.com/jqmcginnis/multi_contrast_inr)

22. 📜 **Streak artifacts reduction algorithm using an implicit neural representation in sparse-view CT.**
      - 📅 Publication Date: *4th Apr., 2022*
      - 📖 Journal: *Medical Imaging 2022: Physics of Medical Imaging, 2022*
      - 🧑‍🔬 Authors: *Byeongjoon Kim, Hyunjung Shim, Jongduk Baek.*
      - 📄 [PDF](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/12031/120312N/Streak-artifacts-reduction-algorithm-using-an-implicit-neural-representation-in/10.1117/12.2610722.short)
   
23. 📜 **Spatial Attention-based Implicit Neural Representation for Arbitrary Reduction of MRI Slice Spacing**
     - 🗓️ Publication Date: 23rd May. 2022
     - 🧑‍🔬 Authors: Xin Wang, Sheng Wang, Honglin Xiong, Kai Xuan, Zixu Zhuang, Mengjun Liu, Zhenrong Shen, Xiangyu Zhao, Lichi Zhang, Qian Wang
     - 📄 [PDF](https://arxiv.org/abs/2205.11346)
   
24. 📜 **A scan-specific unsupervised method for parallel MRI reconstruction via implicit neural representation**
     - 🗓️ Publication Date: 19th Oct. 2022
     - 🧑‍🔬 Authors: Ruimin Feng, Qing Wu, Yuyao Zhang, Hongjiang Wei
     - 📄 [PDF](https://arxiv.org/abs/2210.10439)
   
25. 📜 **Dual Arbitrary Scale Super-Resolution for Multi-Contrast MRI**
     - 🗓️ Publication Date: 5th Jul. 2023
     - 🧑‍🔬 Authors: Jiamiao Zhang, Yichen Chi, Jun Lyu, Wenming Yang, Yapeng Tian
     - 📄 [PDF](https://arxiv.org/abs/2307.02334)
     - 💻 [GitHub](https://github.com/jmzhang79/dual-arbnet)
   
26. 📜 **Unsupervised reconstruction of accelerated cardiac cine MRI using Neural Fields**
    - 🗓️ Publication Date: 24th Jul. 2023
    - 📖 Preprint: arxiv
    - 🧑‍🔬 Authors: Tabita Catalán, Matías Courdurier, Axel Osses, René Botnar, Francisco Sahli Costabal, Claudia Prieto
    - 📄 [PDF](https://arxiv.org/abs/2307.14363)
    - 💻 [GitHub](https://github.com/fsahli/NF-cMRI)
    - 📌 Highlight: An unsupervised INR approach that uses the spatio-temporal Fourier Features of the heart's motion.

27. 📜 **Self-supervised arbitrary scale super-resolution framework for anisotropic MRI**
     - 🗓️ Publication Date: 2th May. 2023
     - 🧑‍🔬 Authors: Haonan Zhang, Yuhan Zhang, Qing Wu, Jiangjie Wu, Zhiming Zhen, Feng Shi, Jianmin Yuan, Hongjiang Wei, Chen Liu, Yuyao Zhang
     - 📄 [PDF](https://arxiv.org/abs/2305.01360)
      
28. 📜 **Implicit Neural Networks with Fourier-Feature Inputs for Free-breathing Cardiac MRI Reconstruction**
     - 🗓️ Publication Date: 11th May. 2023
     - 🧑‍🔬 Authors: Johannes F. Kunz, Stefan Ruschke, Reinhard Heckel
     - 📄 [PDF](https://arxiv.org/abs/2305.06822)
     - 💻 [GitHub](https://github.com/mli-lab/cinemri)

29. 📜 **Implicit neural representations for unsupervised super-resolution and denoising of 4D flow MRI**
     - 🗓️ Publication Date: 24th Feb. 2023
     - 🧑‍🔬 Authors: Simone Saitta, Marcello Carioni, Subhadip Mukherjee, Carola-Bibiane Schönlieb, Alberto Redaelli
     - 📄 [PDF](https://arxiv.org/abs/2302.12835)
   
30. 📜 **CoNeS: Conditional neural fields with shift modulation for multi-sequence MRI translation.**
      - 📅 Publication Date: *6th Sep., 2023*
      - 📖 Preprint: *arxiv*
      - 🧑‍🔬 Authors: *Yunjie Chen, Marius Staring, Olaf M. Neve, Stephan R. Romeijn, Erik F. Hensen, Berit M. Verbist, Jelmer M. Wolterink, Qian Tao.*
      - 📄 [PDF](https://arxiv.org/abs/2309.03320)
      - 💻 [GitHub](https://github.com/cyjdswx/cones)


---
### CT and MRI

31. 📜 **NeRP: Implicit Neural Representation Learning with Prior Embedding for Sparsely Sampled Image Reconstruction**
    - 🗓️ Publication Date: *24th Aug. 2021*
    - 📖 Preprint: *IEEE Transactions on Neural Networks and Learning Systems, 2022*
    - 🧑‍🔬 Authors: *Liyue Shen, John Pauly, Lei Xing.*
    - 📄 [PDF](https://arxiv.org/abs/2108.10991)
    - 💻 [Github](https://github.com/liyues/nerp)
   
32. 📜 **CuNeRF: Cube-Based Neural Radiance Field for Zero-Shot Medical Image Arbitrary-Scale Super Resolution**
     - 🗓️ Publication Date: 28th Mar. 2023
     - 🧑‍🔬 Authors: Zixuan Chen, Jianhuang Lai, Lingxiao Yang, Xiaohua Xie
     - 📄 [PDF](https://arxiv.org/abs/2303.16242)

---
### Ultrasound

33. 📜 **ImplicitVol: Sensorless 3D Ultrasound Reconstruction with Deep Implicit Representation**
    - 🗓️ Publication Date: *24th Sep. 2021*
    - 📖 Preprint: arXiv
    - 🧑‍🔬 Authors: *Pak-Hei Yeung, Linde Hesse, Moska Aliasi, Monique Haak, the INTERGROWTH-21st Consortium, Weidi Xie, Ana I.L. Namburete*
    - 📄 [PDF](https://arxiv.org/abs/2109.12108)


34. 📜 **Representing 3D Ultrasound with Neural Fields**
    - 🗓️ Publication Date: *21st Apr. 2022*
    - 📖 Conference: *Medical Imaging with Deep Learning, 2022*
    - 🧑‍🔬 Authors: *Ang Nan Gu, Purang Abolmaesumi, Christina Luong, Kwang Moo Yi*
    - 📄 [PDF](https://openreview.net/forum?id=1EDRk-CyQou)

35. 📜 **Going Off-Grid: Continuous Implicit Neural Representations for 3D Vascular Modeling**
    - 🗓️ Publication Date: *16th Sep. 2022*
    - 📖 Preprint: arXiv
    - 🧑‍🔬 Authors: *Dieuwertje Alblas, Christoph Brune, Kak Khee Yeung, Jelmer M. Wolterink*
    - 📄 [PDF](https://arxiv.org/abs/2207.14663)
      
  ---
### Dental and Maxillofacial

36. 📜 **Topology-Preserving Shape Reconstruction and Registration via Neural Diffeomorphic Flow.** 
     - 📅 Publication Date: *16th Mar., 2022*
     - 📖 Conference: *Proceedings of the IEEE/CVF Conference on CVPR*
     - 🧑‍🔬 Authors: *Shanlin Sun, Kun Han, Deying Kong, Hao Tang, Xiangyi Yan, Xiaohui Xie.*
     - 📄 [PDF](https://arxiv.org/abs/2203.08652)
     - 🖥️ [GitHub](https://github.com/Siwensun/Neural_Diffeomorphic_Flow--NDF)

37. 📜 **Dynamic Cone-beam CT Reconstruction using Spatial and Temporal Implicit Neural Representation Learning (STINR).**
    - 📅 Publication Date: *Sep., 2022*
    - 📖 Journal: *Physics in Medicine and Biology, 2023*
    - 🧑‍🔬 Authors: *You Zhang, Hua-Chieh Shao, Tinsu Pan, Tielige Mengke.*
    - 📄 [PDF](https://pubmed.ncbi.nlm.nih.gov/36638543/)

38. 📜 **Learning Deep Intensity Field for Extremely Sparse-View CBCT Reconstruction.** 
     - 📅 Publication Date: *12th Mar., 2023*
     - 📖 Preprint: *arXiv*
     - 🧑‍🔬 Authors: *Yiqun Lin, Zhongjin Luo, Wei Zhao, Xiaomeng Li.*
     - 📄 [PDF](https://arxiv.org/abs/2303.06681)
     - 🖥️ [GitHub](https://github.com/xmed-lab/dif-net)
    
--- 
### General and Miscellaneous

39. 📜 **Going Off-Grid: Continuous Implicit Neural Representations for 3D Vascular Modeling**
     - 🗓️ Publication Date: 16th Sep. 2022
     - 🧑‍🔬 Authors: Dieuwertje Alblas, Christoph Brune, Kak Khee Yeung, Jelmer M. Wolterink
     - 📄 [PDF](https://arxiv.org/abs/2207.14663)

40. 📜 **Implicitatlas: learning deformable shape templates in medical imaging**
     - 🗓️ Publication Date: CVPR, 2022
     - 🧑‍🔬 Authors: Jiancheng Yang, Udaranga Wickramasinghe, Bingbing Ni, Pascal Fua
     - 📄 [PDF](https://openaccess.thecvf.com/content/CVPR2022/html/Yang_ImplicitAtlas_Learning_Deformable_Shape_Templates_in_Medical_Imaging_CVPR_2022_paper.html)

41. 📜 **MiShape: 3D Shape Modelling of Mitochondria in Microscopy**
     - 🗓️ Publication Date: 2nd Mar. 2023
     - 🧑‍🔬 Authors: Abhinanda R. Punnakkal, Suyog S Jadhav, Alexander Horsch, Krishna Agarwal, Dilip K. Prasad
     - 📄 [PDF](https://arxiv.org/abs/2303.01546)

42. 📜 **A Novel Implicit Neural Representation for Volume Data**
     - 🗓️ Publication Date: 27th Feb. 2023
     - 🧑‍🔬 Authors: Armin Sheibanifard, Hongchuan Yu
     - 📄 [PDF](https://www.mdpi.com/2076-3417/13/5/3242)

43. 📜 **Hybrid Neural Diffeomorphic Flow for Shape Representation and Generation via Triplane**
     - 🗓️ Publication Date: 4th Jul. 2023
     - 🧑‍🔬 Authors: Kun Han, Shanlin Sun, Xiaohui Xie
     - 📄 [PDF](https://arxiv.org/abs/2307.01957)

44. 📜 **Hybrid-CSR: Coupling Explicit and Implicit Shape Representation for Cortical Surface Reconstruction**
     - 🗓️ Publication Date: 23rd Jul. 2023
     - 🧑‍🔬 Authors: Shanlin Sun, Thanh-Tung Le, Chenyu You, Hao Tang, Kun Han, Haoyu Ma, Deying Kong, Xiangyi Yan, Xiaohui Xie
     - 📄 [PDF](https://arxiv.org/abs/2307.12299)

<img src="Figures/Reconstruction.jpg" alt="reconstruction" width="1016" height="5"><br>
<img src="Figures/Segmentation.jpg" alt="Segmentation" width="1016" height="5"><br>
## Image Segmentation

### Brain Structures and Lesions:

45. 📜 **NeRD: Neural Representation of Distribution for Medical Image Segmentation**
    - 📅 Publication Date: *6th Mar., 2021*
    - 📖 Preprint: *arXiv, 2021*
    - 🧑‍🔬 Authors: *Hang Zhang, Rongguang Wang, Jinwei Zhang, Chao Li, Gufeng Yang, Pascal Spincemaille, Thanh Nguyen, Yi Wang*
    - 📄 [PDF](https://arxiv.org/abs/2103.04020)
    - 📌 Highlight: Addresses white matter lesion segmentation and left atrial segmentation.

46. 📜 **Implicit field learning for unsupervised anomaly detection in medical images**
    - 📅 Publication Date: *9th Jun., 2021*
    - 📖 Conference: *MICCAI 2021*
    - 🧑‍🔬 Authors: *Sergio Naval Marimont, Giacomo Tarroni*
    - 📄 [PDF](https://arxiv.org/abs/2106.05214)
    - 📌 Highlight: Aims to localize gliomas on brain MR images using an unsupervised out-of-distribution detection method.

47. 📜 **Direct localization and delineation of human pedunculopontine nucleus based on a self-supervised magnetic resonance image super-resolution method**
    - 📅 Publication Date: *25th Apr., 2023*
    - 📖 Journal: *Human Brain Mapping, 2023*
    - 🧑‍🔬 Authors: *Jun Li, Xiaojun Guan, Qing Wu, Chenyu He, Weimin Zhang, Xiyue Lin, Chunlei Liu, Hongjiang Wei, Xiaojun Xu, Yuyao Zhang*
    - 📄 [PDF](https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.26311)
    - 📌 Highlight: Focuses on delineating the pedunculopontine nucleus (PPN).

---

### Cardiac and Heart Structures
48. 📜 **Binary segmentation of medical images using implicit spline representations and deep learning**
    - 📅 Publication Date: *19th Mar., 2021*
    - 📖 Journal: *Computer Aided Geometric Design, 2021*
    - 🧑‍🔬 Authors: *Oliver J.D. Barrowclough, Georg Muntingh, Varatharajan Nainamalai, Ivar Stangeby*
    - 📄 [PDF](https://arxiv.org/abs/2102.12759)
    - 📌 Highlight: Tackles image segmentation for a congenital heart disease computed tomography medical imaging dataset.

---

### Retinal Blood Vessels:

49. 📜 **Retinal vessel segmentation based on self-distillation and implicit neural representation**
    - 📅 Publication Date: *8th Nov., 2022*
    - 📖 Journal: *Applied Intelligence, 2022*
    - 🧑‍🔬 Authors: *Jia Gu, Fangzheng Tian & Il-Seok Oh*
    - 📄 [PDF](https://link.springer.com/article/10.1007/s10489-022-04252-2)
    - 📌 Highlight: Concentrates on segmenting retinal blood vessels from retinal images.

---

### 3D Segmentation:

50. 📜 **Deep Implicit Statistical Shape Models for 3D Medical Image Delineation**
    - 📅 Publication Date: *28th Jun., 2022*
    - 📖 Conference: *AAAI, 2022*
    - 🧑‍🔬 Authors: *Ashwin Raju, Shun Miao, Dakai Jin, Le Lu, Junzhou Huang, Adam P. Harrison*
    - 📄 [PDF](https://arxiv.org/abs/2104.02847)
    - 🖥️ [GitHub](https://github.com/ashstuff/dissm)
    - 📌 Highlight: Presents a methodology that emphasizes 3D delineation of anatomical structures using deep implicit statistical shape models.

51. 📜 **Implicit Neural Representations for Medical Imaging Segmentation**
    - 📅 Publication Date: *16th Sep., 2022*
    - 📖 Conference: *International Conference on Medical Image Computing and Computer-Assisted Intervention, 2022*
    - 🧑‍🔬 Authors: *Muhammad Osama Khan & Yi Fang*
    - 📄 [PDF](https://link.springer.com/chapter/10.1007/978-3-031-16443-9_42)
    - 📌 Highlight: Specifically mentions 3D signals in medical imaging, hinting at 3D anatomical structures.

---

### Boundary Refinement:

52. 📜 **Implicit Anatomical Rendering for Medical Image Segmentation with Stochastic Experts**
    - 📅 Publication Date: *6th Apr., 2023*
    - 📖 Preprint: *arXiv, 2023*
    - 🧑‍🔬 Authors: *Chenyu You, Weicheng Dai, Yifei Min, Lawrence Staib, James S. Duncan*
    - 📄 [PDF](https://arxiv.org/abs/2304.03209)
    - 🖥️ [GitHub](https://github.com/charlesyou999648/morse)
    - 📌 Highlight: Emphasizes refining the boundary regions of segmented medical images.

---
### Patch Level Segmentation:

53. 📜 **SwIPE: Efficient and Robust Medical Image Segmentation with Implicit Patch Embeddings**
    - 📅 Publication Date: *23rd Jul., 2023*
    - 📖 Conference: *MICCAI 2023*
    - 🧑‍🔬 Authors: *Yejia Zhang, Pengfei Gu, Nishchal Sapkota, Danny Z. Chen*
    - 📄 [PDF](https://arxiv.org/abs/2307.12429)
    - 📌 Highlight: Uses implicit neural representations to predict shapes at the patch level, balancing both local boundary delineation and global shape coherence.


<img src="Figures/Segmentation.jpg" alt="Segmentation" width="1016" height="5"><br>
<img src="Figures/Registration.jpg" alt="Registration" width="1016" height="5"><br>
## Image Registration

### Deformable Registration

54. 📜 **Implicit Neural Representations for Deformable Image Registration**
    - 📅 Publication Date: *22th Jun., 2022*
    - 📖 Conference: *Medical Imaging with Deep Learning, 2022*
    - 🧑‍🔬 Authors: *Jelmer M. Wolterink, Jesse C. Zwienenberg, Christoph Brune*
    - 📄 [PDF](https://openreview.net/forum?id=BP29eKzQBu3)
    - 🖥️ [GitHub](https://github.com/MIAGroupUT/IDIR)
    - 📌 Highlight: Implicit deformable image registration using a neural network to represent continuous transformations

55. 📜 **Learning Homeomorphic Image Registration via Conformal-Invariant Hyperelastic Regularisation**
    - 📅 Publication Date: *30th Jun., 2023*
    - 📖 Preprint: *arXiv, 2023*
    - 🧑‍🔬 Authors: *Jing Zou, Noémie Debroux, Lihao Liu, Jing Qin, Carola-Bibiane Schönlieb, Angelica I Aviles-Rivero*
    - 📄 [PDF](https://arxiv.org/abs/2303.08113)
    - 📌 Highlight: Topology-preserving deformable image registration. It discusses a novel regularizer based on conformal-invariant properties.

56. 📜 **Deformable Image Registration with Geometry-informed Implicit Neural Representations**
    - 📅 Publication Date: *13th Apr., 2023*
    - 📖 Conference: *Medical Imaging with Deep Learning, 2023*
    - 🧑‍🔬 Authors: *Louis van Harten, Rudolf Leonardus Mirjam Van Herten, Jaap Stoker, Ivana Isgum*
    - 📄 [PDF](https://openreview.net/forum?id=Pj9vtDIzSCE)
    - 📌 Highlight: Parameterizes the deformation field by incorporating the geometry encoding of anatomical structures to guide the deformation process.

57. 📜 **Implicit neural representations for joint decomposition and registration of gene expression images in the marmoset brain.**
    - 📅 Publication Date: *8th Aug., 2023*
    - 📖 Preprint: *arXiv*
    - 🧑‍🔬 Authors: *Michal Byra, Charissa Poon, Tomomi Shimogori, Henrik Skibbe*
    - 📄 [PDF](https://arxiv.org/abs/2308.04039)
    - 📌 Highlight: Addresses the registration of brain images with added features or artifacts by emphasizing the decomposition of images into support and residual components.

58. 📜 **INR-LDDMM: Fluid-based Medical Image Registration Integrating Implicit Neural Representation and Large Deformation Diffeomorphic Metric Mapping.**
    - 📅 Publication Date: *18th Aug., 2023*
    - 📖 Preprint: *arXiv*
    - 🧑‍🔬 Authors: *Chulong Zhang, Xiaokun Liang*
    - 📄 [PDF](https://arxiv.org/abs/2308.09473)
    - 📌 Highlight: Combines implicit neural representation with Large Deformable Diffeomorphic Metric Mapping (LDDMM) in a coarse-to-fine approach.

---

### Diffeomorphic Registration

59. 📜 **Medical Image Registration via Neural Fields**
    - 📅 Publication Date: *22th Jun., 2022*
    - 📖 Preprint: *arXiv, 2022*
    - 🧑‍🔬 Authors: *Shanlin Sun, Kun Han, Hao Tang, Deying Kong, Junayed Naushad, Xiangyi Yan, Xiaohui Xie*
    - 📄 [PDF](https://arxiv.org/abs/2206.03111)
    - 📌 Highlight: Introduces a distinction between general deformable registration and diffeomorphic image registration using neural fields.

60. 📜 **Diffeomorphic Image Registration with Neural Velocity Field**
    - 📅 Publication Date: *2023*
    - 📖 Conference: *IEEE/CVF Winter Conference on Applications of Computer Vision, 2023*
    - 🧑‍🔬 Authors: *Kun Han, Shanlin Sun, Xiangyi Yan, Chenyu You, Hao Tang, Junayed Naushad, Haoyu Ma, Deying Kong, Xiaohui Xie*
    - 📄 [PDF](https://arxiv.org/abs/2202.12498)
    - 📌 Highlight: Introduces a cascaded framework for diffeomorphic Image Registration with Neural Velocity Field (DNVF) by modeling the space of transformations.


<img src="Figures/Registration.jpg" alt="Registration" width="1016" height="5"><br>
<img src="Figures/Neural Rendering.jpg" alt="Neural Rendering" width="1016" height="5"><br>
## Neural Rendering

### Reconstruction from Limited or Sparse Views

#### Computed Tomography (CT)

61. 📜 **MedNeRF: Medical Neural Radiance Fields for Reconstructing 3D-aware CT-Projections from a Single X-ray.**
    - 📅 Publication Date: *2nd Feb., 2022*
    - 📖 Conference: *IEEE EMBC, 2022*
    - 🧑‍🔬 Authors: *Abril Corona-Figueroa, Jonathan Frawley, Sam Bond-Taylor, Sarath Bethapudi, Hubert P. H. Shum, Chris G. Willcocks.*
    - 📄 [PDF](https://arxiv.org/abs/2202.01020)
    - 🖥️ [Github](https://github.com/abrilcf/mednerf)
    - 📌 Highlight: Reconstruct CT projections from a few or a single-view X-ray, based on neural radiance fields. The proposed technique minimizes patients' exposure to ionizing radiation.

#### Cone Beam Computed Tomography (CBCT)

62. 📜  **NAF: Neural Attenuation Fields for Sparse-View CBCT Reconstruction.**
    - 📅 Publication Date: *29th Sep., 2022*
    - 📖 Conference: *MICCAI, 2022*
    - 🧑‍🔬 Authors: *Ruyi Zha, Yanhao Zhang, Hongdong Li.*
    - 📄 [PDF](https://arxiv.org/abs/2209.14540)
    - 🖥️ [Github](https://github.com/ruyi-zha/naf_cbct)
    - 📌 Highlight: A self-supervised approach for CBCT reconstruction that requires no external training data, using a deep neural network to represent attenuation coefficients.

63. 📜 **SNAF: Sparse-view CBCT Reconstruction with Neural Attenuation Fields.**
    - 📅 Publication Date: *30th Nov., 2022*
    - 📖 Preprint: *arXiv*
    - 🧑‍🔬 Authors: *Yu Fang, Lanzhuju Mei, Changjian Li, Yuan Liu, Wenping Wang, Zhiming Cui, Dinggang Shen.*
    - 📄 [PDF](https://arxiv.org/abs/2211.17048)
    - 📌 Highlight: Can reconstruct high-quality CBCT images from limited 2D projections, addressing concerns about radiation dose and image quality in dental applications.

#### Magnetic Resonance Imaging (MRI)

64. 📜 **3D reconstructions of brain from MRI scans using neural radiance fields.**
    - 📅 Publication Date: *24th Apr., 2023*
    - 📖 Preprint: *arXiv*
    - 🧑‍🔬 Authors: *Khadija Iddrisu, Sylwia Malec, Alessandro Crimi.*
    - 📄 [PDF](https://www.biorxiv.org/content/10.1101/2023.04.24.538160v1#:~:text=The%20development%20of%20neural%20radiance,2D%20slices%20of%20MRI%20scans.)
    - 📌 Highlight: Uses neural radiance fields to reconstruct 3D MRI images from 2D MRI slices, aiming to reduce scan acquisition times and potential motion artifacts.


#### Digital Subtraction Angiography (DSA)

65. 📜 **TiAVox: Time-aware Attenuation Voxels for Sparse-view 4D DSA Reconstruction.**
    - 📅 Publication Date: *5th Sep., 2023*
    - 📖 Preprint: *arXiv*
    - 🧑‍🔬 Authors: *Zhenghong Zhou, Huangxuan Zhao, Jiemin Fang, Dongqiao Xiang, Lei Chen, Lingxia Wu, Feihong Wu, Wenyu Liu, Chuansheng Zheng, Xinggang Wang.*
    - 📄 [PDF](https://arxiv.org/abs/2309.02318)
    - 📌 Highlight: A method for high-quality sparse-view 4D DSA reconstruction, reducing the required radiation dose and increasing the efficiency of 4D imaging in diagnosing vascular diseases.

### Surgical Scene Reconstruction
#### Robotic Surgery
66. 📜 **Neural Rendering for Stereo 3D Reconstruction of Deformable Tissues in Robotic Surgery.**
    - 📅 Publication Date: *30th Jun., 2022*
    - 📖 Conferenc: *MICCAI, 2022*
    - 🧑‍🔬 Authors: *Yuehao Wang, Yonghao Long, Siu Hin Fan, Qi Dou.*
    - 📄 [PDF](https://arxiv.org/abs/2206.15255)
    - 🖥️ [Github](https://github.com/med-air/endonerf)
    - 📌 Highlight: Uses dynamic neural radiance fields to reconstruct deformable tissues during robotic surgery from stereo video captures 

#### Endoscopic Surgery

67. 📜 **EndoSurf: Neural Surface Reconstruction of Deformable Tissues with Stereo Endoscope Videos.**
    - 📅 Publication Date: *21st Jul., 2023*
    - 📖 Conferenc: *MICCAI 2023*
    - 🧑‍🔬 Authors: *Ruyi Zha, Xuelian Cheng, Hongdong Li, Mehrtash Harandi, Zongyuan Ge.*
    - 📄 [PDF](https://arxiv.org/abs/2307.11307)
    - 🖥️ [Github](https://github.com/ruyi-zha/endosurf)
    - 📌 Highlight: Learns and represents a deforming surface from RGBD sequences captured via endoscope, offering improvements in high-fidelity shape reconstructions.
### Ultrasound Imaging

68. 📜 **Ultra-NeRF: Neural Radiance Fields for Ultrasound Imaging.**
    - 📅 Publication Date: *25th Jan., 2023*
    - 📖 Conferenc: *MIDL, 2023*
    - 🧑‍🔬 Authors: *Magdalena Wysocki, Mohammad Farid Azampour, Christine Eilers, Benjamin Busam, Mehrdad Salehi, Nassir Navab.*
    - 📄 [PDF](https://arxiv.org/abs/2301.10520)
    - 📌 Highlight: Introduces a physics-enhanced implicit neural representation for ultrasound imaging which accounts for view-dependent changes in appearance and geometry, improving the quality of synthesized ultrasound images.

### Dental and Oral Imaging

69. 📜 **Oral-NeXF: 3D Oral Reconstruction with Neural X-ray Field from Panoramic Imaging.**
    - 📅 Publication Date: *21st Mar., 2023*
    - 📖 Preprint: *arxiv*
    - 🧑‍🔬 Authors: *Weinan Song, Haoxin Zheng, Jiawei Yang, Chengwen Liang, Lei He.*
    - 📄 [PDF](https://arxiv.org/abs/2303.12123)
    - 📌 Highlight: Proposes a solution for 3D reconstruction of oral structures using a single panoramic X-ray, with a model that learns to represent the 3D oral structure implicitly

### Pose Estimation

70. 📜 **Robust Single-view Cone-beam X-ray Pose Estimation with Neural Tuned Tomography (NeTT) and Masked Neural Radiance Fields (mNeRF).**
    - 📅 Publication Date: *1st Aug., 2023*
    - 📖 Preprint: *arxiv*
    - 🧑‍🔬 Authors: *Chaochao Zhou, Syed Hasib Akhter Faruqui, Abhinav Patel, Ramez N. Abdalla, Michael C. Hurley, Ali Shaibani, Matthew B. Potts, Babak S. Jahromi, Leon Cho, Sameer A. Ansari, Donald R. Cantrell.*
    - 📄 [PDF](https://arxiv.org/abs/2308.00214)
    - 📌 Highlight: A method for pose estimation of radiolucent objects via X-ray projections. Two high-fidelity view synthesis methods (NeTT and mNeRF) are introduced, with NeTT being highlighted for its computational efficiency and generalization capabilities.


<img src="Figures/Neural Rendering.jpg" alt="Neural Rendering" width="1016" height="5"><br>
<img src="Figures/Compression.jpg" alt="Compression" width="1016" height="5"><br> 
## Image Compression

**SCI: A Spectrum Concentrated Implicit Neural Compression for Biomedical Data.** [23th Nov., 2022] [AAAI, 2023]<br>
*Runzhao Yang, Tingxiong Xiao, Yuxiao Cheng, Qianni Cao, Jinyuan Qu, Jinli Suo, Qionghai Dai.*<br>
 [[PDF](https://arxiv.org/abs/2209.15180)] [[Github](https://github.com/MIAGroupUT/IDIR)]
 
**TINC: Tree-structured Implicit Neural Compression.** [12th Nov., 2022] [arXiv, 2022]<br>
*Runzhao Yang, Tingxiong Xiao, Yuxiao Cheng, Jinli Suo, Qionghai Dai.*<br>
 [[PDF]()] [[Github](https://github.com/MIAGroupUT/IDIR)]

 **COIN++ Neural Compression Across Modalities** [8th Dec ., 2022] [arXiv preprint, 2022]<br>
*Emilien Dupont, Hrushikesh Loya, Milad Alizadeh, Adam Goliński, Yee Whye Teh, Arnaud Doucet*<br>
 [[PDF]( https://arxiv.org/abs/2201.12904)] 

 **SINCO: A Novel structural regularizer for image compression using implicit neural representations** [5th May., 2023] [IEEE International Conference on Acoustics, Speech and Signal Processing, 2023]<br>
*Harry Gao, Weijie Gan, Zhixin Sun, Ulugbek S. Kamilov*<br>
 [[PDF]( https://arxiv.org/abs/2210.14974)]

<img src="Figures/Compression.jpg" alt="Compression" width="1016" height="5"><br> 
<img src="Figures/Synthesis.jpg" alt="Synthesis" width="1016" height="5"><br> 
 ## Image Synthesis

**Implicit Neural Representations for Generative Modeling of Living Cell Shapes.** [6th Oct., 2022] [International Conference on Medical Image Computing and Computer-Assisted Intervention, 2022]<br>
*David Wiesner, Julian Suk, Sven Dummer, David Svoboda, Jelmer M. Wolterink.*<br>
 [[PDF](https://arxiv.org/abs/2207.06283)] 

**Generative modeling of living cells with SO(3)-equivariant implicit neural representations.** [18 th Apr., 2023] [arXiv preprint, 2023]<br>
*David Wiesner, Julian Suk, Sven Dummer, Tereza Nečasová, Vladimír Ulman, David Svoboda, Jelmer M. Wolterink*<br>
 [[PDF]( https://arxiv.org/abs/2304.08960)]


 <img src="Figures/Synthesis.jpg" alt="Synthesis" width="1016" height="5">


