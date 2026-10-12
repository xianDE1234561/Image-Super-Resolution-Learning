# Image Super-Resolution Learning

**Personal study notes on image super-resolution.**

这是我个人学习图像超分辨率的资料与笔记仓库，用于记录论文阅读、梳理算法原理，并规划后续复现与小实验。当前按阅读顺序整理了 7 篇经典论文的原文 PDF 和中文精读，学习内容覆盖早期 CNN、残差网络、通道注意力与参考纹理迁移。

## 阅读导航

| 顺序 | 模型与年份 | 学习重点 | 原论文 | 我的精读笔记 |
|---|---|---|---|---|
| 1 | SRCNN (2014) | CNN 超分辨率基础 | [论文 PDF](1_Learning%20a%20Deep%20Convolutional%20Network%20for%20Image%20Super-Resolution/01_SRCNN_ECCV2014.pdf) | [中文精读](1_Learning%20a%20Deep%20Convolutional%20Network%20for%20Image%20Super-Resolution/SRCNN_ECCV2014_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 2 | FSRCNN (2016) | 低分辨率空间计算与学习上采样 | [论文 PDF](2_Accelerating%20the%20Super-Resolution%20Convolutional%20Neural%20Network/02_FSRCNN_ECCV2016.pdf) | [中文精读](2_Accelerating%20the%20Super-Resolution%20Convolutional%20Neural%20Network/FSRCNN_ECCV2016_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 3 | VDSR (2016) | 深层网络、残差学习与训练稳定性 | [论文 PDF](3_Accurate%20Image%20Super-Resolution%20Using%20Very%20Deep%20Convolutional%20Networks/03_VDSR_CVPR2016.pdf) | [中文精读](3_Accurate%20Image%20Super-Resolution%20Using%20Very%20Deep%20Convolutional%20Networks/VDSR_CVPR2016_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 4 | ESPCN (2016) | 子像素卷积与高效上采样 | [论文 PDF](4_Real-Time%20Single%20Image%20and%20Video%20Super-Resolution%20Using%20an%20Efficient%20Sub-Pixel%20Convolutional%20Neural%20Network/04_ESPCN_CVPR2016.pdf) | [中文精读](4_Real-Time%20Single%20Image%20and%20Video%20Super-Resolution%20Using%20an%20Efficient%20Sub-Pixel%20Convolutional%20Neural%20Network/ESPCN_CVPR2016_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 5 | EDSR (2017) | 增强残差网络与多尺度模型 | [论文 PDF](5_Enhanced%20Deep%20Residual%20Networks%20for%20Single%20Image%20Super-Resolution/05_EDSR_CVPRW2017.pdf) | [中文精读](5_Enhanced%20Deep%20Residual%20Networks%20for%20Single%20Image%20Super-Resolution/EDSR_CVPRW2017_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 6 | RCAN (2018) | 残差通道注意力 | [论文 PDF](6_Image%20Super-Resolution%20Using%20Very%20Deep%20Residual%20Channel%20Attention%20Networks/06_RCAN_ECCV2018.pdf) | [中文精读](6_Image%20Super-Resolution%20Using%20Very%20Deep%20Residual%20Channel%20Attention%20Networks/RCAN_ECCV2018_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |
| 7 | TTSR (2020) | 参考图像引导的纹理迁移 | [论文 PDF](7_Learning%20Texture%20Transformer%20Network%20for%20Image%20Super-Resolution/07_TTSR_CVPR2020.pdf) | [中文精读](7_Learning%20Texture%20Transformer%20Network%20for%20Image%20Super-Resolution/TTSR_CVPR2020_%E6%B7%B1%E5%BA%A6%E7%B2%BE%E8%AF%BB%E4%B8%8E%E7%A7%91%E7%A0%94%E5%88%9B%E6%96%B0%E5%88%86%E6%9E%90.md) |

建议按 **SRCNN → FSRCNN → VDSR → ESPCN → EDSR → RCAN → TTSR** 的顺序学习。前六篇主要研究单幅图像超分辨率；TTSR 额外使用高分辨率参考图像。

## 我的学习笔记

中文精读是供我个人学习使用的辅助笔记，包含整体解读、研究目标、算法与数学模型、实验验证、后续研究方向、批判性评价和本科科研学习路线。笔记中的改进思路作为后续学习与实验的候选方向；实验参数和结果以原论文为准。

## 资料索引

- [论文原文下载清单与来源](%E8%AE%BA%E6%96%87%E5%8E%9F%E6%96%87%E4%B8%8B%E8%BD%BD%E6%B8%85%E5%8D%95.md)
- [论文与项目整理文档（Word）](%E5%9B%BE%E5%83%8F%E8%B6%85%E5%88%86%E8%BE%A8%E7%8E%87%E7%BB%8F%E5%85%B8%E7%BD%91%E7%BB%9C%E8%AE%BA%E6%96%87%E4%B8%8E%E9%A1%B9%E7%9B%AE%E6%95%B4%E7%90%86.docx)
- [文件 SHA-256 校验值](CHECKSUMS.sha256)

## 文件组织

每篇论文保存在独立的“数字 + 英文论文名称”文件夹中，包含原论文 PDF 与中文精读 Markdown。GitHub 可直接预览精读中的表格和 LaTeX 公式；PDF 可在线打开或下载。

论文版权归原作者和出版方所有，原文来源见下载清单。学习和引用时请注明对应论文。
