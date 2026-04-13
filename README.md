<div align="center">

# Durian: Dual Reference Image-Guided Portrait Animation with Attribute Transfer

<a href="https://arxiv.org/abs/2509.04434"><img src='https://img.shields.io/badge/arXiv-2509.04434-b31b1b.svg?style=for-the-badge' alt='arXiv'></a>
<a href="https://arxiv.org/pdf/2509.04434.pdf"><img src='https://img.shields.io/badge/Paper-PDF-green?style=for-the-badge' alt='Paper PDF'></a>
<a href="https://hyunsoocha.github.io/durian/"><img src='https://img.shields.io/badge/Project-Page-blue?style=for-the-badge' alt='Project Page'></a>
<a href="https://openreview.net/forum?id=tz5GRv9Vzu"><img src='https://img.shields.io/badge/OpenReview-Forum-8c1b13?style=for-the-badge' alt='OpenReview'></a>

### ICLR 2026

[Hyunsoo Cha](https://hyunsoocha.github.io/) &nbsp;&nbsp; [Byungjun Kim](https://bjkim95.github.io/) &nbsp;&nbsp; [Hanbyul Joo](https://jhugestar.github.io/)

Seoul National University

<br>

https://github.com/user-attachments/assets/26a8e05b-060c-46d6-a7ca-c7e1287eda55

</div>

---

## News

- **[2026.04]** [arXiv preprint](https://arxiv.org/abs/2509.04434) and [project page](https://hyunsoocha.github.io/durian/) are released.
- **[2026.01]** Paper accepted to **ICLR 2026**!

## TODO

- [x] Release project page
- [x] Release arXiv paper
- [ ] Release inference code & pretrained weights
- [ ] Release training code

## Abstract

We present **Durian**, the first method for generating portrait animation videos with cross-identity attribute transfer from one or more reference images to a target portrait. Training such models typically requires attribute pairs of the same individual, which are rarely available at scale. To address this challenge, we propose a self-reconstruction formulation that leverages ordinary portrait videos to learn attribute transfer without explicit paired data. Two frames from the same video act as a pseudo pair: one serves as an attribute reference and the other as an identity reference. To enable this self-reconstruction training, we introduce a **Dual ReferenceNet** that processes the two references separately and then fuses their features via spatial attention within a diffusion model. To make sure each reference functions as a specialized stream for either identity or attribute information, we apply complementary masking to the reference images. Together, these two components guide the model to reconstruct the original video, naturally learning cross-identity attribute transfer. To bridge the gap between self-reconstruction training and cross-identity inference, we introduce a mask expansion strategy and augmentation schemes, enabling robust transfer of attributes with varying spatial extent and misalignment. Durian achieves state-of-the-art performance on portrait animation with attribute transfer. Moreover, its dual reference design uniquely supports multi-attribute composition and smooth attribute interpolation within a single generation pass, enabling highly flexible and controllable synthesis.

## Citation

If you find our work useful, please consider citing:

```bibtex
@inproceedings{cha2026durian,
  title     = {Durian: Dual Reference Image-Guided Portrait Animation with Attribute Transfer},
  author    = {Cha, Hyunsoo and Kim, Byungjun and Joo, Hanbyul},
  booktitle = {Proceedings of the International Conference on Learning Representations (ICLR)},
  year      = {2026}
}
```

## Acknowledgements

This work was conducted at [SNU VCLab](https://jhugestar.github.io/).

## License

This project is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
