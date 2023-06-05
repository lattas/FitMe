# [FitMe: Deep Photorealistic 3D Morphable Model Avatars](https://alexlattas.com/fitme)
[![Youtube Video](https://img.shields.io/badge/Video-CVPR-lightgrey?logo=youtube)](https://youtu.be/73ZFDkZRRCk)
[![arXiv Preprint](https://img.shields.io/badge/arXiv-Paper-lightgrey?logo=arxiv)](https://arxiv.org/abs/2305.09641)

Published in the IEEE/CVF Conference on Computer Vision and Pattern Recognition (__[CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Lattas_FitMe_Deep_Photorealistic_3D_Morphable_Model_Avatars_CVPR_2023_paper.pdf)__)

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

In this paper, we introduce FitMe, a facial reflectance model and a differentiable rendering optimization pipeline, that can be used to acquire high-fidelity renderable human avatars from single or multiple images.

The model consists of a multi-modal style-based generator, that captures facial appearance in terms of diffuse and specular reflectance, and a PCA-based shape model. We employ a fast differentiable rendering process that can be used in an optimization pipeline, while also achieving photorealistic facial shading. Our optimization process accurately captures both the facial reflectance and shape in high-detail, by exploiting the expressivity of the style-based latent representation and of our shape model.

FitMe achieves state-of-the-art reflectance acquisition and identity preservation on single ``in-the-wild'' facial images, while it produces impressive scan-like results, when given multiple unconstrained facial images pertaining to the same identity. In contrast with recent implicit avatar reconstructions, FitMe requires only one minute and produces relightable mesh and texture-based avatars, that can be used by end-user applications.

## CVPR Video on Youtube
<div align="center">
      <a href="hhttps://youtu.be/73ZFDkZRRCk">
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