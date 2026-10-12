# Image Super-Resolution Learning

**Personal study notes on image super-resolution.**

This repository documents my personal study of image super-resolution. I use it to keep reading notes, understand the methods, and plan future reproductions and small experiments. It currently contains 20 paper PDFs: seven classic papers with Chinese reading notes, followed by 13 recent papers and challenge reports from 2023–2026. The collection covers CNNs, residual networks, attention, state-space models, efficient reconstruction, reference-based restoration, and generative super-resolution.

## Reading Guide

| Order | Model and Year | Key Topics | Paper | My Reading Notes |
|---|---|---|---|---|
| 1 | SRCNN (2014) | CNN foundations for super-resolution | [Paper PDF](1_Learning%20a%20Deep%20Convolutional%20Network%20for%20Image%20Super-Resolution/01_SRCNN_ECCV2014.pdf) | [Chinese Notes](1_Learning%20a%20Deep%20Convolutional%20Network%20for%20Image%20Super-Resolution/SRCNN_ECCV2014_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 2 | FSRCNN (2016) | Low-resolution feature processing and learned upsampling | [Paper PDF](2_Accelerating%20the%20Super-Resolution%20Convolutional%20Neural%20Network/02_FSRCNN_ECCV2016.pdf) | [Chinese Notes](2_Accelerating%20the%20Super-Resolution%20Convolutional%20Neural%20Network/FSRCNN_ECCV2016_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 3 | VDSR (2016) | Deep networks, residual learning, and stable training | [Paper PDF](3_Accurate%20Image%20Super-Resolution%20Using%20Very%20Deep%20Convolutional%20Networks/03_VDSR_CVPR2016.pdf) | [Chinese Notes](3_Accurate%20Image%20Super-Resolution%20Using%20Very%20Deep%20Convolutional%20Networks/VDSR_CVPR2016_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 4 | ESPCN (2016) | Sub-pixel convolution and efficient upsampling | [Paper PDF](4_Real-Time%20Single%20Image%20and%20Video%20Super-Resolution%20Using%20an%20Efficient%20Sub-Pixel%20Convolutional%20Neural%20Network/04_ESPCN_CVPR2016.pdf) | [Chinese Notes](4_Real-Time%20Single%20Image%20and%20Video%20Super-Resolution%20Using%20an%20Efficient%20Sub-Pixel%20Convolutional%20Neural%20Network/ESPCN_CVPR2016_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 5 | EDSR (2017) | Enhanced residual networks and multi-scale models | [Paper PDF](5_Enhanced%20Deep%20Residual%20Networks%20for%20Single%20Image%20Super-Resolution/05_EDSR_CVPRW2017.pdf) | [Chinese Notes](5_Enhanced%20Deep%20Residual%20Networks%20for%20Single%20Image%20Super-Resolution/EDSR_CVPRW2017_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 6 | RCAN (2018) | Residual channel attention | [Paper PDF](6_Image%20Super-Resolution%20Using%20Very%20Deep%20Residual%20Channel%20Attention%20Networks/06_RCAN_ECCV2018.pdf) | [Chinese Notes](6_Image%20Super-Resolution%20Using%20Very%20Deep%20Residual%20Channel%20Attention%20Networks/RCAN_ECCV2018_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 7 | TTSR (2020) | Reference-based texture transfer | [Paper PDF](7_Learning%20Texture%20Transformer%20Network%20for%20Image%20Super-Resolution/07_TTSR_CVPR2020.pdf) | [Chinese Notes](7_Learning%20Texture%20Transformer%20Network%20for%20Image%20Super-Resolution/TTSR_CVPR2020_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |

Recommended reading order: **SRCNN → FSRCNN → VDSR → ESPCN → EDSR → RCAN → TTSR**. The first six papers focus on single-image super-resolution; TTSR additionally uses a high-resolution reference image.

## Recent Papers and Reports

These PDFs continue the reading order at 8–20. I will add my reading notes gradually as I study them; notes for these papers have not been uploaded yet. Years below refer to the conference or report year. Where the source is arXiv, the PDF is the author-provided version.

Reading sequence: **HAT → MambaIR → MambaIRv2 → SAFMN → ESPAN → NTIRE Efficient SR Report → iRAG → RefVSR++ → SeeSR → SinSR → TSD-SR → VOSR → NTIRE ×4 SR Report**.

The sequence covers high-fidelity reconstruction (8–10), efficient SR (11–13), reference-based SR (14–15), generative SR (16–19), and evaluation (20). Challenge reports summarize multiple methods and benchmarks.

| Order | Paper / Model | Venue or Report | Key Topics | Paper | Original Source |
|---|---|---|---|---|---|
| 8 | HAT | CVPR 2023 | Hybrid channel/window attention and cross-window interaction | [Paper PDF](8_Activating%20More%20Pixels%20in%20Image%20Super-Resolution%20Transformer/08_HAT_CVPR2023.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2023/papers/Chen_Activating_More_Pixels_in_Image_Super-Resolution_Transformer_CVPR_2023_paper.pdf) |
| 9 | MambaIR | ECCV 2024 | State-space restoration with local enhancement and channel attention | [Paper PDF](9_MambaIR%20-%20A%20Simple%20Baseline%20for%20Image%20Restoration%20with%20State-Space%20Model/09_MambaIR_ECCV2024.pdf) | [ECVA](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/02740.pdf) |
| 10 | MambaIRv2 | CVPR 2025 | Attentive state-space modeling and semantic-guided neighbors | [Paper PDF](10_MambaIRv2%20-%20Attentive%20State%20Space%20Restoration/10_MambaIRv2_CVPR2025.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2025/papers/Guo_MambaIRv2_Attentive_State_Space_Restoration_CVPR_2025_paper.pdf) |
| 11 | SAFMN | ICCV 2023 | Multi-scale spatial feature modulation for efficient SR | [Paper PDF](11_Spatially-Adaptive%20Feature%20Modulation%20for%20Efficient%20Image%20Super-Resolution/11_SAFMN_ICCV2023.pdf) | [CVF](https://openaccess.thecvf.com/content/ICCV2023/papers/Sun_Spatially-Adaptive_Feature_Modulation_for_Efficient_Image_Super-Resolution_ICCV_2023_paper.pdf) |
| 12 | ESPAN | CVPRW / NTIRE 2025 | Efficient attention networks and quality/runtime trade-offs | [Paper PDF](12_Expanded%20SPAN%20for%20Efficient%20Super-Resolution/12_ESPAN_CVPRW2025.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2025W/NTIRE/papers/Wang_Expanded_SPAN_for_Efficient_Super-Resolution_CVPRW_2025_paper.pdf) |
| 13 | NTIRE Efficient SR Report | CVPRW / NTIRE 2026 | Efficient SR methods, runtime, parameters, and FLOPs | [Paper PDF](13_The%20Eleventh%20NTIRE%202026%20Efficient%20Super-Resolution%20Challenge%20Report/13_NTIRE_EfficientSR_CVPRW2026.pdf) | [Author arXiv](https://arxiv.org/pdf/2604.03198) |
| 14 | iRAG / Reference-based SR | ICCV 2025 | Reference retrieval, image-based RAG, and diffusion restoration | [Paper PDF](14_Reference-based%20Super-Resolution%20via%20Image-based%20Retrieval-Augmented%20Generation%20Diffusion/14_RefSR_RAG_ICCV2025.pdf) | [CVF](https://www.openaccess.thecvf.com/content/ICCV2025/papers/Lee_Reference-based_Super-Resolution_via_Image-based_Retrieval-Augmented_Generation_Diffusion_ICCV_2025_paper.pdf) |
| 15 | RefVSR++ | WACV 2025 | Reference-based video SR and temporal aggregation | [Paper PDF](15_RefVSR%2B%2B%20-%20Exploiting%20Reference%20Inputs%20for%20Reference-Based%20Video%20Super-Resolution/15_RefVSRpp_WACV2025.pdf) | [CVF](https://openaccess.thecvf.com/content/WACV2025/papers/Zou_RefVSR_Exploiting_Reference_Inputs_for_Reference-Based_Video_Super-Resolution_WACV_2025_paper.pdf) |
| 16 | SeeSR | CVPR 2024 | Semantic guidance for real-world generative SR | [Paper PDF](16_SeeSR%20-%20Towards%20Semantics-Aware%20Real-World%20Image%20Super-Resolution/16_SeeSR_CVPR2024.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2024/papers/Wu_SeeSR_Towards_Semantics-Aware_Real-World_Image_Super-Resolution_CVPR_2024_paper.pdf) |
| 17 | SinSR | CVPR 2024 | Single-step diffusion through distillation | [Paper PDF](17_SinSR%20-%20Diffusion-Based%20Image%20Super-Resolution%20in%20a%20Single%20Step/17_SinSR_CVPR2024.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2024/papers/Wang_SinSR_Diffusion-Based_Image_Super-Resolution_in_a_Single_Step_CVPR_2024_paper.pdf) |
| 18 | TSD-SR | CVPR 2025 | Target score distillation for one-step real-world SR | [Paper PDF](18_TSD-SR%20-%20One-Step%20Diffusion%20with%20Target%20Score%20Distillation%20for%20Real-World%20Image%20Super-Resolution/18_TSD-SR_CVPR2025.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2025/papers/Dong_TSD-SR_One-Step_Diffusion_with_Target_Score_Distillation_for_Real-World_Image_CVPR_2025_paper.pdf) |
| 19 | VOSR | CVPR 2026 | Vision-only generative SR and one-step distillation | [Paper PDF](19_VOSR%20-%20A%20Vision-Only%20Generative%20Model%20for%20Image%20Super-Resolution/19_VOSR_CVPR2026.pdf) | [CVF](https://openaccess.thecvf.com/content/CVPR2026/papers/Wu_VOSR_A_Vision-Only_Generative_Model_for_Image_Super-Resolution_CVPR_2026_paper.pdf) |
| 20 | NTIRE ×4 SR Report | NTIRE 2026 challenge report | Restoration and perceptual evaluation tracks for ×4 SR | [Paper PDF](20_The%20Fourth%20Challenge%20on%20Image%20Super-Resolution%20%28x4%29%20at%20NTIRE%202026%20-%20Benchmark%20Results%20and%20Method%20Overview/20_NTIRE_SR_x4_CVPRW2026.pdf) | [Author arXiv](https://arxiv.org/pdf/2604.14558) |

The recent folders contain PDFs only. The first seven folders also contain the existing Chinese reading notes.

## My Study Notes

The Chinese reading notes support my own learning. They cover each paper's motivation, methods and mathematical models, experiments, possible research directions, limitations, and a learning plan. Suggested improvements are ideas for future experiments. Technical details and reported results should be checked against the original papers.

## Resource Index

- [Classic Paper Sources and Download Index (1–7)](%E8%AE%BA%E6%96%87%E5%8E%9F%E6%96%87%E4%B8%8B%E8%BD%BD%E6%B8%85%E5%8D%95.md)
- [Classic Paper and Project Summary (Word, 1–7)](%E5%9B%BE%E5%83%8F%E8%B6%85%E5%88%86%E8%BE%A8%E7%8E%87%E7%BB%8F%E5%85%B8%E7%BD%91%E7%BB%9C%E8%AE%BA%E6%96%87%E4%B8%8E%E9%A1%B9%E7%9B%AE%E6%95%B4%E7%90%86.docx)
- [Initial Upload Checksum Snapshot](CHECKSUMS.sha256)

## File Organization

Each paper has its own folder, named with a reading-order number and the English paper title. All 20 folders contain a paper PDF. Folders 1–7 also contain Chinese reading notes in Markdown; I will upload notes for 8–20 later. GitHub can display the tables and LaTeX formulas in the notes; PDFs can be viewed online or downloaded.

Copyright belongs to the original authors and publishers. Source links for recent papers are listed above; sources for the first seven papers are also listed in the classic download index. Please cite the corresponding papers when using their work.
