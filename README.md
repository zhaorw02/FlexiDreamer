# FlexiDreamer：Single Image-to-3D Generation with FlexiCubes

<p align="center">
     <span style="font-size: 30px;"><a href="https://arxiv.org">Paper</a></span> | <span style="font-size: 30px;"><a href="https://flexidreamer.github.io/">Project Page</a></span>
</p>

<p align="center">
  <a href="https://zhaorw02.github.io/">Ruowen Zhao</a><sup>1,4</sup>, 
    <a href="https://thuwzy.github.io/">Zhengyi Wang</a><sup>2,4</sup>, 
    <a href="https://yikaiw.github.io/">Yikai Wang</a><sup>2</sup>, 
  	Zihan Zhou<sup>3</sup>, 
    <a href="https://ml.cs.tsinghua.edu.cn/~jun/index.shtml">Jun Zhu</a><sup>2,4</sup>
</p>
<p align="center"><sup>1</sup>University of Chinese Academy of Sciences,&ensp;<sup>2</sup>Tsinghua University,&ensp;<sup>3</sup>Xidian University,&ensp; <sup>4</sup>ShengShu&ensp;


<p align="center"> Our Code will be released soon... 🏗️🚧🔨</p>

## Abstract

3D content generation from text prompts or single images has made remarkable progress in quality and speed recently. One of its dominant paradigms involves generating consistent multi-view images followed by a sparse-view reconstruction. However, due to the challenge of directly deforming the mesh representation to approach the target topology, most methodologies learn an implicit representation (such as NeRF) during the sparse-view reconstruction and acquire the target mesh by a post-processing extraction. Although the implicit representation can effectively model rich 3D information, its training typically entails a long convergence time. In addition, the post-extraction operation from the implicit field also leads to undesirable visual artifacts. In this paper, we propose FlexiDreamer, a novel single image-to-3d generation framework that reconstructs the target mesh in an end-to-end manner. By leveraging a flexible gradient-based extraction known as FlexiCubes, our method circumvents the defects brought by the post-processing and facilitates a direct acquisition of the target mesh. Furthermore, we incorporate a multi-resolution hash grid encoding scheme that progressively activates the encoding levels into the implicit field in FlexiCubes to help capture geometric details for per-step optimization. Notably, FlexiDreamer recovers a dense 3D structure from a single-view image in approximately 1 minute on a single NVIDIA A100 GPU, outperforming previous methodologies by a large margin.

![first.png](./assets/first.png)

## Comparisons

![compare.png](./assets/compare.png)

## BibTex

