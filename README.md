# [FitMe: Deep Photorealistic 3D Morphable Model Avatars](https://alexlattas.com/fitme)
[![Youtube Video](https://img.shields.io/badge/Video-CVPR-lightgrey?logo=youtube)](https://youtu.be/73ZFDkZRRCk)
[![arXiv Preprint](https://img.shields.io/badge/arXiv-Paper-lightgrey?logo=arxiv)](https://arxiv.org/abs/2305.09641)

Published in the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR 2023) (__[CVPR Paper Link](https://openaccess.thecvf.com/content/CVPR2023/papers/Lattas_FitMe_Deep_Photorealistic_3D_Morphable_Model_Avatars_CVPR_2023_paper.pdf)__)

See the __[Project Page](https://alexlattas.com/fitme)__ for more details and HQ videos.

[Alexandros Lattas](https://alexlattas.com),
[Stylianos Moschoglou](https://www.doc.ic.ac.uk/~sm3515/),
[Stylianos Ploumpis](https://www.ploumpis.com/),<br>
[Baris Gecer](https://barisgecer.github.io),
[Jiankang Deng](https://jiankangdeng.github.io/),
[Stefanos Zafeiriou](https://www.imperial.ac.uk/people/s.zafeiriou)
<br/>
Imperial College London
<br/>

## Overview

![teaser](https://github.com/lattas/FitMe/assets/9087275/80a39fdd-3bdd-47ec-ab87-0f8990cd0553)

In this paper, we introduce FitMe, a facial reflectance model and a differentiable rendering optimization pipeline, that can be used to acquire high-fidelity renderable human avatars from single or multiple images.

The model consists of a multi-modal style-based generator, that captures facial appearance in terms of diffuse and specular reflectance, and a PCA-based shape model. We employ a fast differentiable rendering process that can be used in an optimization pipeline, while also achieving photorealistic facial shading. Our optimization process accurately captures both the facial reflectance and shape in high-detail, by exploiting the expressivity of the style-based latent representation and of our shape model.

FitMe achieves state-of-the-art reflectance acquisition and identity preservation on single "in-the-wild" facial images, while it produces impressive scan-like results, when given multiple unconstrained facial images pertaining to the same identity. In contrast with recent implicit avatar reconstructions, FitMe requires only one minute and produces relightable mesh and texture-based avatars, that can be used by end-user applications.

## Method
In two steps, we optimize the latent vector of the generator, the shape and rendering parameters, by combining 3DMM fitting, GAN inversion and GAN tuning. The optimization is guided by accurate diffuse and specular differentiable rendering.

![method](https://github.com/lattas/FitMe/assets/9087275/b62f27fb-8417-4ac4-8ee0-a3b133e2a806)

## Results
FitMe can be optimized for arbitrary facial images, from a single internet sourced picture, to multiple selfie photographs.

![single](https://github.com/lattas/FitMe/assets/9087275/3bae220a-4288-4139-9c96-27b7a3f827f1)

Even with three unconstrained quick selfies of a subject, in an arbitrary environment and illumination, FitMe produces high-fidelity relfectance and shape that can be photorealistically relighted.

https://github.com/lattas/FitMe/assets/9087275/64f04bbe-a7a2-4c86-a90e-5dc28e3e9bb8

## CVPR Video on Youtube
<div align="center">
      <a href="https://youtu.be/73ZFDkZRRCk">
         <img src="https://img.youtube.com/vi/73ZFDkZRRCk/0.jpg" width="480">
      </a>
</div>

## Reference
```
@InProceedings{Lattas_2023_CVPR,
      author    = {Lattas, Alexandros and Moschoglou, Stylianos and Ploumpis, Stylianos and Gecer, Baris and Deng, Jiankang and Zafeiriou, Stefanos},
      title     = {FitMe: Deep Photorealistic 3D Morphable Model Avatars},
      booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
      month     = {June},
      year      = {2023},
      pages     = {8629-8640}
  }
```
