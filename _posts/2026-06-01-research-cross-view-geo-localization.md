---
layout: post
title: "CIPER: A Unified Framework for Cross-view Image-retrieval and Pose-estimation"
categories: Research
# excerpt_separator:  <!--more-->
---

<div align="center">
    <div style="position: relative; padding-bottom: 56.25%; height: 0;">
        <iframe 
        src="https://www.youtube.com/embed/Z8bKGTeyeSk" 
        frameborder="0" 
        allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen
        style="position: absolute; width: 100%; height: 100%; left: 0; top: 0;"></iframe>
    </div>
</div>

<br>

<div class="icon-container">
    <span class="link-with-icon">
        <i data-feather="paperclip"></i>
        <a href="http://arxiv.org/abs/2606.05011" target="_blank">Paper Link</a>
    </span> 
    <span class="link-with-icon">
        <i data-feather="github"></i>
        <a href="https://github.com/yurimjeon1892/CIPER.git" target="_blank">Code</a>
    </span> 
    <span class="link-with-icon">
        <i data-feather="youtube"></i>
        <a href="https://youtu.be/Z8bKGTeyeSk" target="_blank">Video</a>
    </span>    
</div>

<br>


Cross-view geo-localization aims to estimate the geographic location of a ground image using a reference database of aerial images. Existing approaches typically address this problem through either large-scale image retrieval or precise pose estimation. While retrieval-based methods enable wide-area search, their localization accuracy is limited by database resolution. In contrast, pose estimation methods achieve high accuracy but are constrained to a narrow search space. However, simply cascading these disjoint pipelines often suffers from error propagation and inconsistent feature representations. To overcome these limitations, we formulate cross-view geo-localization as a unified problem that simultaneously requires city-scale retrieval and precise 3-DoF pose estimation. To address this challenge, we propose CIPER (Cross-view Image-retrieval and Pose-estimation transformER), a unified framework that jointly performs both tasks within a single architecture, promoting mutually beneficial feature learning. CIPER employs a shared transformer encoder with task-specific tokens to disentangle global retrieval features and spatial localization cues. To mitigate the significant domain gap between ground and aerial images, we propose a two-way transformer pose decoder that leverages ground features as spatial queries to perform bidirectional cross-attention for robust cross-view alignment. Furthermore, a set prediction strategy is adopted for stable 3-DoF regression under a unified multi-task learning objective. Extensive experiments on large-scale datasets, including VIGOR, KITTI, and Ford Multi-AV, demonstrate that the proposed method achieves reliable and competitive performance, particularly under limited field-of-view and arbitrary orientation conditions. These results validate CIPER as a versatile and robust baseline for practical cross-view localization, providing a reliable foundation for future research in unified architectures. 
