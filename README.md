# Image Super-Resolution Learning

**Personal study notes on image super-resolution.**

This repository documents my personal study of image super-resolution. I use it to keep reading notes, understand the methods, and plan future reproductions and small experiments. It currently contains seven classic papers and Chinese reading notes, covering early CNNs, residual networks, channel attention, and reference-based texture transfer.

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

## My Study Notes

The Chinese reading notes support my own learning. They cover each paper's motivation, methods and mathematical models, experiments, possible research directions, limitations, and a learning plan. Suggested improvements are ideas for future experiments. Technical details and reported results should be checked against the original papers.

## Resource Index

- [Paper Sources and Download Index](%E8%AE%BA%E6%96%87%E5%8E%9F%E6%96%87%E4%B8%8B%E8%BD%BD%E6%B8%85%E5%8D%95.md)
- [Paper and Project Summary (Word)](%E5%9B%BE%E5%83%8F%E8%B6%85%E5%88%86%E8%BE%A8%E7%8E%87%E7%BB%8F%E5%85%B8%E7%BD%91%E7%BB%9C%E8%AE%BA%E6%96%87%E4%B8%8E%E9%A1%B9%E7%9B%AE%E6%95%B4%E7%90%86.docx)
- [File SHA-256 Checksums](CHECKSUMS.sha256)

## File Organization

Each paper has its own folder, named with a reading-order number and the English paper title. The folder contains the paper PDF and Chinese reading notes in Markdown. GitHub can display the tables and LaTeX formulas in the notes; PDFs can be viewed online or downloaded.

Copyright belongs to the original authors and publishers. Source links are listed in the download index. Please cite the corresponding papers when using their work.
