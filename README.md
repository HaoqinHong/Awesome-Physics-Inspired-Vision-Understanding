### Awesome-Physics-Inspired-3D-Reconstruction-and-Simulation

A curated list of papers and open-source resources focused on Physics-Inspired 3D Reconstruction and Simulation, intended to keep pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

- [Solution of Inverse Problems Using NeRF or 3DGS](#solution-of-inverse-problems-using-nerf-or-3dgs)
- [Simulation Method Based on 3D Gaussian Splatting](#simulation-method-based-on-3d-gaussian-splatting)
- [Reconstruction and Simulation Method Incorporating LLM](#reconstruction-and-simulation-method-incorporating-llm)
- [Physically-Based Rendering Using NeRF or 3DGS](#physically-based-rendering-using-nerf-or-3dgs)
- [Physics-Informed Fluid Reconstruction](#physics-informed-fluid-reconstruction)
- [Representive Basic Methods: 3D Reconstruction](#representive-basic-methods-3d-reconstruction)
- [Representive Basic Methods: Dynamic New View Synthesis](#representive-basic-methods-dynamic-new-view-synthesis)

## Related Knowledge Resources

<a href="https://github.com/HaoqinHong/Physics-for-Graphics-Notes">**Physics for Computer Graphics Self-Studying Plan**</a> (By Myself)

<a href="https://github.com/MrNeRF/awesome-3D-gaussian-splatting"> **Awesome 3D Gaussian Splatting**</a>

<a href="https://github.com/Awesome3DGS/3D-Gaussian-Splatting-Papers?tab=readme-ov-file"> **3D Gaussian Splatting Papers**</a>

**🫡 [Keep Updating] Paper Interpretation** (By Myself, only allowed for studying):

<details>
    <summary style="margin-left: 40px;"><b>Foundation Papers</b></summary>
    <ul>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1oM7mbGSl8osIrZPsmdXvczVDCtFTxJ1D/view?usp=drive_link">3D Gaussian Splatting</a></li>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1QFrkBhMLyqLRCn7bujKy98B0hI34PFEH/view?usp=drive_link">2D Gaussian Splatting</a></li>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/12WS_nT51RxmYC8OIg7bw9K-Uwl6fgALD/view?usp=drive_link">Dynamic 3D Gaussians & 4D Gaussian Splatting</a></li>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1rheSh8b9ddjkNqO2vwPT7PSiTZS5BnCD/view?usp=drive_link">Deformable-Gaussians</a></li>
    </ul>
</details>

<details>
    <summary style="margin-left: 40px;"><b>Simulation Method Papers</b></summary>
    <ul>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1gGP4GepEl_6BimyBY2mKY-1maDdQF5Eo/view?usp=drive_link">PhysGaussian</a></li>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1UeIEYOUAYjqssfW6EOnoi57hhoc50uKX/view?usp=drive_link">PhysDreamer & KAN & Other Physics-based Learning Methods</a></li>
    </ul>
</details>

<details>
    <summary style="margin-left: 40px;"><b>Physics-Informed Method Papers</b></summary>
    <ul>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1vperfD5crgXPBXlTtspMpOguhXVQLZmU/view?usp=drive_link">Physics Informed Neural Fields</a></li>
        <li style="margin-left: 50px;"><a href="https://drive.google.com/file/d/1blHG7hLBt8Ndm8s1tV4ZgCA06D1dqpPu/view?usp=drive_link">Physics-Informed Learning of Characteristic Trajectories</a></li>
    </ul>
</details>

## Open-Source Tools

<li><a href="https://playcanvas.com/supersplat/editor/ "> Online Gaussian Editor</a></li>

## Update Log

<details span><summary><b>Details</b></summary>
<li> 2025-2-28 by Haoqin Hong: Update 3D Gaussian Splatting Papers.</li>
<li>2024-12-21 by Haoqin Hong: Update Physically-Based Rendering Using NeRF or 3DGS module and 3 papers.</li>
<li>2024-12-17 by Haoqin Hong: Refine the Projects.</li>
<li>2024-12-10 by Haoqin Hong: Update Representive Basic Methods: 3D Reconstruction or Dynamic New View Synthesis module.</li>
<li>2024-12-4 by Haoqin Hong: Update open-source tools module and merge physical material simulators module.</li>
<li>2024-12-3 by Haoqin Hong: Update physical material simulators module.</li>
<li>2024-12-2 by Haoqin Hong: Update my knowledge notebooks.</li>
<li>2024-12-2 by Haoqin Hong: Update initial version.</li>

</details>

## Solution of Inverse Problems Using NeRF or 3DGS

### 2024

#### [ECCV 2024] Reconstruction and Simulation of Elastic Objects with Spring-Mass 3D Gaussians

**Authors:** [L Zhong](https://scholar.google.com/citations?user=ixobBrEAAAAJ&hl=zh-CN&oi=sra), [HX Yu](https://scholar.google.com/citations?user=kNKncZcAAAAJ&hl=zh-CN&oi=sra), [J Wu](https://scholar.google.com/citations?user=2efgcS0AAAAJ&hl=zh-CN&oi=sra), [Y Li](https://scholar.google.com/citations?user=WlA92lcAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
Reconstructing and simulating elastic objects from visual observations is crucial for applications in computer vision and robotics. Existing methods, such as 3D Gaussians, model 3D appearance and geometry, but lack the ability to estimate physical properties for objects and simulate them. The core challenge lies in integrating an expressive yet efficient physical dynamics model. We propose Spring-Gaus, a 3D physical object representation for reconstructing and simulating elastic objects from videos of the object from multiple viewpoints. In particular, we develop and integrate a 3D Spring-Mass model into 3D Gaussian kernels, enabling the reconstruction of the visual appearance, shape, and physical dynamics of the object. Our approach enables future prediction and simulation under various initial states and environmental properties. We evaluate Spring-Gaus on both synthetic and real-world datasets, demonstrating accurate reconstruction and simulation of elastic objects. Project page: https://zlicheng. com/spring_gaus.
</details>
<a href="https://arxiv.org/abs/2403.09434">📄 Paper</a>  
<a href="https://zlicheng.com/spring_gaus/">🌐 Project Page</a>  
<a href="https://github.com/Colmar-zlicheng/Spring-Gaus">💻 Code</a>

#### [NeurIPS 2024] GIC: Gaussian-Informed Continuum for Physical Property Identification and Simulation

**Authors:** [J Cai](https://scholar.google.com/citations?user=GeSCNR4AAAAJ&hl=zh-CN&oi=sra), Y Yang, [W Yuan](https://scholar.google.com/citations?user=m3tqxRQAAAAJ&hl=zh-CN&oi=sra), [Y He](https://scholar.google.com/citations?user=UM4qFCsAAAAJ&hl=zh-CN&oi=sra), [Z Dong](https://scholar.google.com/citations?user=GHOQKCwAAAAJ&hl=zh-CN&oi=sra), L Bo, H Cheng, [Q Chen](https://scholar.google.com/citations?user=lLMX9hcAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
This paper studies the problem of estimating physical properties (system identification) through visual observations. To facilitate geometry-aware guidance in physical property estimation, we introduce a novel hybrid framework that leverages 3D Gaussian representation to not only capture explicit shapes but also enable the simulated continuum to render object masks as 2D shape surrogates during training. We propose a new dynamic 3D Gaussian framework based on motion factorization to recover the object as 3D Gaussian point sets across different time states. Furthermore, we develop a coarse-to-fine filling strategy to generate the density fields of the object from the Gaussian reconstruction, allowing for the extraction of object continuums along with their surfaces and the integration of Gaussian attributes into these continuum. In addition to the extracted object surfaces, the Gaussian-informed continuum also enables the rendering of object masks during simulations, serving as 2D-shape guidance for physical property estimation. Extensive experimental evaluations demonstrate that our pipeline achieves state-of-the-art performance across multiple benchmarks and metrics. Additionally, we illustrate the effectiveness of the proposed method through real-world demonstrations, showcasing its practical utility. Our project page is at https://jukgei.github.io/project/gic.
</details>
<a href="https://arxiv.org/html/2406.14927">📄 Paper</a>  
<a href="https://jukgei.github.io/project/gic/">🌐 Project Page</a>  
<a href="https://github.com/Jukgei/gic">💻 Code</a>

#### [NeurIPS 2024] NeuMA: Neural Material Adaptor for Visual Grounding of Intrinsic Dynamics

**Authors:** J Cao, S Guan, Y Ge, W Li, X Yang, C Ma

<details span><summary><b>Abstract</b></summary>
While humans effortlessly discern intrinsic dynamics and adapt to new scenarios, modern AI systems often struggle. Current methods for visual grounding of dynamics either use pure neural-network-based simulators (black box), which may violate physical laws, or traditional physical simulators (white box), which rely on expert-defined equations that may not fully capture actual dynamics. We propose the Neural Material Adaptor (NeuMA), which integrates existing physical laws with learned corrections, facilitating accurate learning of actual dynamics while maintaining the generalizability and interpretability of physical priors. Additionally, we propose Particle-GS, a particle-driven 3D Gaussian Splatting variant that bridges simulation and observed images, allowing back-propagate image gradients to optimize the simulator. Comprehensive experiments on various dynamics in terms of grounded particle accuracy, dynamic rendering quality, and generalization ability demonstrate that NeuMA can accurately capture intrinsic dynamics. Project Page: https://xjay18.github.io/projects/neuma.html.
</details>
<a href="https://openreview.net/pdf?id=AvWB40qXZh">📄 Paper</a>  
<a href="https://xjay18.github.io/projects/neuma.html">🌐 Project Page</a>  
<a href="https://github.com/XPandora/PhysGaussian">💻 Code</a>

### 2023

#### [ICLR 2023] PAC-NeRF: Physics Augmented Continuum Neural Radiance Fields for Geometry-Agnostic System Identification

**Authors:** [X Li](https://scholar.google.com/citations?user=xAI6xm4AAAAJ&hl=zh-CN&oi=sra), [YL Qiao](https://scholar.google.com/citations?user=ghpLm2cAAAAJ&hl=zh-CN&oi=sra), [PY Chen](https://scholar.google.com/citations?user=9TX3RmEAAAAJ&hl=zh-CN&oi=sra), [KM Jatavallabhula](https://scholar.google.com/citations?user=kcr8134AAAAJ&hl=zh-CN&oi=sra), [M Lin](https://scholar.google.com/citations?user=ugFNit4AAAAJ&hl=zh-CN&oi=sra), [C Jiang](https://scholar.google.com/citations?user=jTivVMEAAAAJ&hl=zh-CN&oi=sra), [C Gan](https://scholar.google.com/citations?user=PTeSCbIAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
Existing approaches to system identification (estimating the physical parameters of an object) from videos assume known object geometries. This precludes their applicability in a vast majority of scenes where object geometries are complex or unknown. In this work, we aim to identify parameters characterizing a physical system from a set of multi-view videos without any assumption on object geometry or topology. To this end, we propose "Physics Augmented Continuum Neural Radiance Fields" (PAC-NeRF), to estimate both the unknown geometry and physical parameters of highly dynamic objects from multi-view videos. We design PAC-NeRF to only ever produce physically plausible states by enforcing the neural radiance field to follow the conservation laws of continuum mechanics. For this, we design a hybrid Eulerian-Lagrangian representation of the neural radiance field, i.e., we use the Eulerian grid representation for NeRF density and color fields, while advecting the neural radiance fields via Lagrangian particles. This hybrid Eulerian-Lagrangian representation seamlessly blends efficient neural rendering with the material point method (MPM) for robust differentiable physics simulation. We validate the effectiveness of our proposed framework on geometry and physical parameter estimation over a vast range of materials, including elastic bodies, plasticine, sand, Newtonian and non-Newtonian fluids, and demonstrate significant performance gain on most tasks.
</details>
<a href="https://arxiv.org/abs/2303.05512">📄 Paper</a>  
<a href="https://xuan-li.github.io/PAC-NeRF/">🌐 Project Page</a>  
<a href="https://github.com/xuan-li/PAC-NeRF">💻 Code</a>

## Simulation Method Based on 3D Gaussian Splatting

### 2024

#### [AAAI 2025] DreamPhysics: Learning Physical Properties of Dynamic 3D Gaussians with Video Diffusion Priors

[T Huang](https://scholar.google.com/citations?user=vhHmAJYAAAAJ&hl=zh-CN&oi=sra), H Zhang, Y Zeng, [Z Zhang](https://scholar.google.com/citations?user=8pIq2N0AAAAJ&hl=zh-CN&oi=sra), H Li, [W Zuo](https://scholar.google.com/citations?user=rUOpCEYAAAAJ&hl=zh-CN&oi=sra), [RWH Lau](https://scholar.google.com/citations?user=KilQqKYAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
Dynamic 3D interaction has been attracting a lot of attention recently. However, creating such 4D content remains challenging. One solution is to animate 3D scenes with physics-based simulation, which requires manually assigning precise physical properties to the object or the simulated results would become unnatural. Another solution is to learn the deformation of 3D objects with the distillation of video generative models, which, however, tends to produce 3D videos with small and discontinuous motions due to the inappropriate extraction and application of physical prior. In this work, combining the strengths and complementing shortcomings of the above two solutions, we propose to learn the physical properties of a material field with video diffusion priors, and then utilize a physics-based Material-Point-Method (MPM) simulator to generate 4D content with realistic motions. In particular, we propose motion distillation sampling to emphasize video motion information during distillation. Moreover, to facilitate the optimization, we further propose a KAN-based material field with frame boosting. Experimental results demonstrate that our method enjoys more realistic motion than state-of-the-arts. Codes are released at: https://github.com/tyhuang0428/DreamPhysics.
</details>
<a href="https://arxiv.org/abs/2406.01476">📄 Paper</a> 
<a href="https://github.com/tyhuang0428/dreamphysics">💻 Code</a>

#### Gaussian Splashing: Unified Particles for Versatile Motion Synthesis and Rendering

**Authors:** [Yutao Feng](https://arxiv.org/search/cs?searchtype=author&query=Feng,+Y), [Xiang Feng](https://arxiv.org/search/cs?searchtype=author&query=Feng,+X), [Yintong Shang](https://arxiv.org/search/cs?searchtype=author&query=Shang,+Y), [Ying Jiang](https://arxiv.org/search/cs?searchtype=author&query=Jiang,+Y), [Chang Yu](https://arxiv.org/search/cs?searchtype=author&query=Yu,+C), [Zeshun Zong](https://arxiv.org/search/cs?searchtype=author&query=Zong,+Z), [Tianjia Shao](https://arxiv.org/search/cs?searchtype=author&query=Shao,+T), [Hongzhi Wu](https://arxiv.org/search/cs?searchtype=author&query=Wu,+H), [Kun Zhou](https://arxiv.org/search/cs?searchtype=author&query=Zhou,+K), [Chenfanfu Jiang](https://arxiv.org/search/cs?searchtype=author&query=Jiang,+C), [Yin Yang](https://arxiv.org/search/cs?searchtype=author&query=Yang,+Y)

<details span><summary><b>Abstract</b></summary>
We demonstrate the feasibility of integrating physics-based animations of solids and fluids with 3D Gaussian Splatting (3DGS) to create novel effects in virtual scenes reconstructed using 3DGS. Leveraging the coherence of the Gaussian Splatting and Position-Based Dynamics (PBD) in the underlying representation, we manage rendering, view synthesis, and the dynamics of solids and fluids in a cohesive manner. Similar to GaussianShader, we enhance each Gaussian kernel with an added normal, aligning the kernel's orientation with the surface normal to refine the PBD simulation. This approach effectively eliminates spiky noises that arise from rotational deformation in solids. It also allows us to integrate physically based rendering to augment the dynamic surface reflections on fluids. Consequently, our framework is capable of realistically reproducing surface highlights on dynamic fluids and facilitating interactions between scene objects and fluids from new views. For more information, please visit our project page at \url{[this https URL](https://gaussiansplashing.github.io/)}.
</details>
<a href="https://arxiv.org/abs/2401.15318">📄 Paper</a>  
<a href="https://gaussiansplashing.github.io/">🌐 Project Page</a>  <a>💻 Code (Not yet)</a>

#### [ACM MM 2024] LoopGaussian: Creating 3D Cinemagraph with Multi-view Images via Eulerian Motion Field

**Authors:** J Li, [L Cheng](https://scholar.google.com/citations?user=PKFAv-cAAAAJ&hl=zh-CN&oi=sra), Z Wang, [T Mu](https://scholar.google.com/citations?user=dOG10IUAAAAJ&hl=zh-CN&oi=sra), J He

<details span><summary><b>Abstract</b></summary>
Cinemagraph creates captivating video experience by combining elements of still photography and subtle motion. However, most existing cinemagraph video generation lacks depth information, being restricted within 2-dimensional (2D) image space. We advance cinemagraph from 2D image space to 3-dimensional (3D) space with high quality by proposing LoopGaussian. It is based on 3D Gaussian modeling, taking advantage of the 3D Gaussian Splatting (3D-GS) technique that has significantly improved the field of novel view synthesis. Here is a brief overview of our new approach: It employs 3D-GS to reconstruct 3D Gaussian point clouds from multi-view images of static scenes, where shape regularization is used to prevent blurring or artifacts caused by object deformation. To maintain local continuity between scenes, it then clusters the 3D Gaussian points by the proposed SuperGaussian algorithm using features acquired by an autoencoder tailored for 3D Gaussian. Similarities between clusters are used to derive an Eulerian motion field for describing velocities across the entire scene. The estimated Eulerian motion field drives the movement of the 3D Gaussian points, based on which a 3D Cinemagraph is generated through bidirectional animation. The resulting 3D Cinemagraph exhibits natural and seamlessly loopable dynamics. Experiment results validate the effectiveness of the proposed approach, demonstrating high-quality and visually appealing video generation.
</details>
<a href="https://arxiv.org/abs/2404.08966">📄 Paper</a>  
<a href="https://pokerlishao.github.io/LoopGaussian/">🌐 Project Page</a>  
<a href="https://github.com/Pokerlishao/LoopGaussian">💻 Code</a>

#### [ECCV 2024] PhysDreamer: Physics-Based Interaction with 3D Objects via Video Generation

**Authors:** [T Zhang](https://scholar.google.com/citations?user=uJocZjkAAAAJ&hl=zh-CN&oi=sra), [HX Yu](https://scholar.google.com/citations?user=kNKncZcAAAAJ&hl=zh-CN&oi=sra), [R Wu](https://scholar.google.com/citations?user=ulf_Pt0AAAAJ&hl=zh-CN&oi=sra), [BY Feng](https://scholar.google.com/citations?user=VCeYRsYAAAAJ&hl=zh-CN&oi=sra), [C Zheng](https://scholar.google.com/citations?user=-0rEuLgAAAAJ&hl=zh-CN&oi=sra), [N Snavely](https://scholar.google.com/citations?user=Db4BCX8AAAAJ&hl=zh-CN&oi=sra), [J Wu](https://scholar.google.com/citations?user=2efgcS0AAAAJ&hl=zh-CN&oi=sra), [WT Freeman](https://scholar.google.com/citations?user=0zZnyMEAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
Realistic object interactions are crucial for creating immersive virtual experiences, yet synthesizing realistic 3D object dynamics in response to novel interactions remains a significant challenge. Unlike unconditional or text-conditioned dynamics generation, action-conditioned dynamics requires perceiving the physical material properties of objects and grounding the 3D motion prediction on these properties, such as object stiffness. However, estimating physical material properties is an open problem due to the lack of material ground-truth data, as measuring these properties for real objects is highly difficult. We present PhysDreamer, a physics-based approach that endows static 3D objects with interactive dynamics by leveraging the object dynamics priors learned by video generation models. By distilling these priors, PhysDreamer enables the synthesis of realistic object responses to novel interactions, such as external forces or agent manipulations. We demonstrate our approach on diverse examples of elastic objects and evaluate the realism of the synthesized interactions through a user study. PhysDreamer takes a step towards more engaging and realistic virtual experiences by enabling static 3D objects to dynamically respond to interactive stimuli in a physically plausible manner. See our project page at https://physdreamer. github. io/.
</details>
<a href="https://arxiv.org/abs/2404.13026">📄 Paper</a>  
<a href="https://physdreamer.github.io/">🌐 Project Page</a>  
<a href="https://github.com/a1600012888/PhysDreamer">💻 Code</a>

#### [CVPR 2024] PhysGaussian: Physics-Integrated 3D Gaussians for Generative Dynamics

**Authors:** [T Xie](https://scholar.google.com/citations?user=oRt4qcgAAAAJ&hl=zh-CN&oi=sra), [Z Zong](https://scholar.google.com/citations?user=6liRAk4AAAAJ&hl=zh-CN&oi=sra), [Y Qiu](https://scholar.google.com/citations?user=zPZ6ijgAAAAJ&hl=zh-CN&oi=sra), [X Li](https://scholar.google.com/citations?user=xAI6xm4AAAAJ&hl=zh-CN&oi=sra), Y Feng, [Y Yang](https://scholar.google.com/citations?user=-z2_nggAAAAJ&hl=zh-CN&oi=sra), [C Jiang](https://scholar.google.com/citations?user=jTivVMEAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
We introduce PhysGaussian a new method that seamlessly integrates physically grounded Newtonian dynamics within 3D Gaussians to achieve high-quality novel motion synthesis. Employing a customized Material Point Method (MPM) our approach enriches 3D Gaussian kernels with physically meaningful kinematic deformation and mechanical stress attributes all evolved in line with continuum mechanics principles. A defining characteristic of our method is the seamless integration between physical simulation and visual rendering: both components utilize the same 3D Gaussian kernels as their discrete representations. This negates the necessity for triangle/tetrahedron meshing marching cubes cage meshes or any other geometry embedding highlighting the principle of" what you see is what you simulate (WS^ 2)". Our method demonstrates exceptional versatility across a wide variety of materials--including elastic entities plastic metals non-Newtonian fluids and granular materials--showcasing its strong capabilities in creating diverse visual content with novel viewpoints and movements.
</details>
<a href="https://arxiv.org/abs/2311.12198">📄 Paper</a>  
<a href="https://xpandora.github.io/PhysGaussian/">🌐 Project Page</a>  
<a href="https://github.com/XJay18/NeuMA?tab=readme-ov-file#data">💻 Code</a>

## Reconstruction and Simulation Method Incorporating LLM

### 2024

#### Text-to-3D Gaussian Splatting with Physics-Grounded Motion Generation

**Authors:** [Wenqing Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+W), [Yun Fu](https://arxiv.org/search/cs?searchtype=author&query=Fu,+Y)

<details span><summary><b>Abstract</b></summary>
Text-to-3D generation is a valuable technology in virtual reality and digital content creation. While recent works have pushed the boundaries of text-to-3D generation, producing high-fidelity 3D objects with inefficient prompts and simulating their physics-grounded motion accurately still remain unsolved challenges. To address these challenges, we present an innovative framework that utilizes the Large Language Model (LLM)-refined prompts and diffusion priors-guided Gaussian Splatting (GS) for generating 3D models with accurate appearances and geometric structures. We also incorporate a continuum mechanics-based deformation map and color regularization to synthesize vivid physics-grounded motion for the generated 3D Gaussians, adhering to the conservation of mass and momentum. By integrating text-to-3D generation with physics-grounded motion synthesis, our framework renders photo-realistic 3D objects that exhibit physics-aware motion, accurately reflecting the behaviors of the objects under various forces and constraints across different materials. Extensive experiments demonstrate that our approach achieves high-quality 3D generations with realistic physics-grounded motion.
</details>
<a href="https://arxiv.org/abs/2412.05560">📄 Paper</a>  
<a>💻 Code (Not yet)</a>

#### Sim Anything: Automated 3D Physical Simulation of Open-world Scene with Gaussian Splatting

**Authors:** [Haoyu Zhao](https://arxiv.org/search/cs?searchtype=author&query=Zhao,+H), [Hao Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+H), [Xingyue Zhao](https://arxiv.org/search/cs?searchtype=author&query=Zhao,+X), [Hongqiu Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+H), [Zhiyu Wu](https://arxiv.org/search/cs?searchtype=author&query=Wu,+Z), [Chengjiang Long](https://arxiv.org/search/cs?searchtype=author&query=Long,+C), [Hua Zou](https://arxiv.org/search/cs?searchtype=author&query=Zou,+H)

<details span><summary><b>Abstract</b></summary>
Recent advancements in 3D generation models have opened new possibilities for simulating dynamic 3D object movements and customizing behaviors, yet creating this content remains challenging. Current methods often require manual assignment of precise physical properties for simulations or rely on video generation models to predict them, which is computationally intensive. In this paper, we rethink the usage of multi-modal large language model (MLLM) in physics-based simulation, and present Sim Anything, a physics-based approach that endows static 3D objects with interactive dynamics. We begin with detailed scene reconstruction and object-level 3D open-vocabulary segmentation, progressing to multi-view image in-painting. Inspired by human visual reasoning, we propose MLLM-based Physical Property Perception (MLLM-P3) to predict mean physical properties of objects in a zero-shot manner. Based on the mean values and the object's geometry, the Material Property Distribution Prediction model (MPDP) model then estimates the full distribution, reformulating the problem as probability distribution estimation to reduce computational costs. Finally, we simulate objects in an open-world scene with particles sampled via the Physical-Geometric Adaptive Sampling (PGAS) strategy, efficiently capturing complex deformations and significantly reducing computational costs. Extensive experiments and user studies demonstrate our Sim Anything achieves more realistic motion than state-of-the-art methods within 2 minutes on a single GPU.
</details>
<a href="https://arxiv.org/abs/2411.12789">📄 Paper</a>  
<a href="https://sim-gs.github.io/">🌐 Project Page</a>  
<a>💻 Code (Not yet)</a>

#### Unleashing the Potential of Multi-modal Foundation Models and Video Diffusion for 4D Dynamic Physical Scene Simulation

**Authors:** [Zhuoman Liu](https://arxiv.org/search/cs?searchtype=author&query=Liu,+Z), [Weicai Ye](https://arxiv.org/search/cs?searchtype=author&query=Ye,+W), [Yan Luximon](https://arxiv.org/search/cs?searchtype=author&query=Luximon,+Y), [Pengfei Wan](https://arxiv.org/search/cs?searchtype=author&query=Wan,+P), [Di Zhang](https://arxiv.org/search/cs?searchtype=author&query=Zhang,+D)

<details span><summary><b>Abstract</b></summary>
Realistic simulation of dynamic scenes requires accurately capturing diverse material properties and modeling complex object interactions grounded in physical principles. However, existing methods are constrained to basic material types with limited predictable parameters, making them insufficient to represent the complexity of real-world materials. We introduce a novel approach that leverages multi-modal foundation models and video diffusion to achieve enhanced 4D dynamic scene simulation. Our method utilizes multi-modal models to identify material types and initialize material parameters through image queries, while simultaneously inferring 3D Gaussian splats for detailed scene representation. We further refine these material parameters using video diffusion with a differentiable Material Point Method (MPM) and optical flow guidance rather than render loss or Score Distillation Sampling (SDS) loss. This integrated framework enables accurate prediction and realistic simulation of dynamic interactions in real-world scenarios, advancing both accuracy and flexibility in physics-based simulations.
</details>
<a href="https://arxiv.org/abs/2411.14423">📄 Paper</a>  
<a href="https://zhuomanliu.github.io/PhysFlow/">🌐 Project Page</a>  
<a>💻 Code (Not yet)</a>

## Physically-Based Rendering Using NeRF or 3DGS

### 2024

#### PBR-NeRF: Inverse Rendering with Physics-Based Neural Fields

**Authors:** [Sean Wu](https://export.arxiv.org/find/cs/1/au:+Wu_S/0/1/0/all/0/1), [Shamik Basu](https://export.arxiv.org/find/cs/1/au:+Basu_S/0/1/0/all/0/1), [Tim Broedermann](https://export.arxiv.org/find/cs/1/au:+Broedermann_T/0/1/0/all/0/1), [Luc Van Gool](https://export.arxiv.org/find/cs/1/au:+Gool_L/0/1/0/all/0/1), [Christos Sakaridis](https://export.arxiv.org/find/cs/1/au:+Sakaridis_C/0/1/0/all/0/1)

<details span><summary><b>Abstract</b></summary>
We tackle the ill-posed inverse rendering problem in 3D reconstruction with a Neural Radiance Field (NeRF) approach informed by Physics-Based Rendering (PBR) theory, named PBR-NeRF. Our method addresses a key limitation in most NeRF and 3D Gaussian Splatting approaches: they estimate view-dependent appearance without modeling scene materials and illumination. To address this limitation, we present an inverse rendering (IR) model capable of jointly estimating scene geometry, materials, and illumination. Our model builds upon recent NeRF-based IR approaches, but crucially introduces two novel physics-based priors that better constrain the IR estimation. Our priors are rigorously formulated as intuitive loss terms and achieve state-of-the-art material estimation without compromising novel view synthesis quality. Our method is easily adaptable to other inverse rendering and 3D reconstruction frameworks that require material estimation. We demonstrate the importance of extending current neural rendering approaches to fully model scene properties beyond geometry and view-dependent appearance. Code is publicly available at [this https URL](https://github.com/s3anwu/pbrnerf)
</details>
<a href="https://arxiv.org/html/2412.09680">📄 Paper</a>  
<a href="https://github.com/s3anwu/pbrnerf">💻 Code</a>

#### [CVPR 2024] GaussianShader: 3D Gaussian Splatting with Shading Functions for Reflective Surfaces

**Authors:** [Yingwenqi Jiang](https://arxiv.org/search/cs?searchtype=author&query=Jiang,+Y), [Jiadong Tu](https://arxiv.org/search/cs?searchtype=author&query=Tu,+J), [Yuan Liu](https://arxiv.org/search/cs?searchtype=author&query=Liu,+Y), [Xifeng Gao](https://arxiv.org/search/cs?searchtype=author&query=Gao,+X), [Xiaoxiao Long](https://arxiv.org/search/cs?searchtype=author&query=Long,+X), [Wenping Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+W), [Yuexin Ma](https://arxiv.org/search/cs?searchtype=author&query=Ma,+Y)

<details span><summary><b>Abstract</b></summary>
The advent of neural 3D Gaussians has recently brought about a revolution in the field of neural rendering, facilitating the generation of high-quality renderings at real-time speeds. However, the explicit and discrete representation encounters challenges when applied to scenes featuring reflective surfaces. In this paper, we present GaussianShader, a novel method that applies a simplified shading function on 3D Gaussians to enhance the neural rendering in scenes with reflective surfaces while preserving the training and rendering efficiency. The main challenge in applying the shading function lies in the accurate normal estimation on discrete 3D Gaussians. Specifically, we proposed a novel normal estimation framework based on the shortest axis directions of 3D Gaussians with a delicately designed loss to make the consistency between the normals and the geometries of Gaussian spheres. Experiments show that GaussianShader strikes a commendable balance between efficiency and visual quality. Our method surpasses Gaussian Splatting in PSNR on specular object datasets, exhibiting an improvement of 1.57dB. When compared to prior works handling reflective surfaces, such as Ref-NeRF, our optimization time is significantly accelerated (23h vs. 0.58h). Please click on our project website to see more results.
</details>
<a href="https://arxiv.org/abs/2311.17977">📄 Paper</a>  
<a href="https://asparagus15.github.io/GaussianShader.github.io/">🌐 Project Page</a>  
<a href="https://github.com/Asparagus15/GaussianShader">💻 Code</a>

## Physics-Informed Fluid Reconstruction

### 2024

#### [ACM SIGGRAPH 2024] Physics-Informed Learning of Characteristic Trajectories for Smoke Reconstruction

**Authors:** [Y Wang](https://scholar.google.com/citations?user=AVOZmU8AAAAJ&hl=zh-CN&oi=sra), [S Tang](https://scholar.google.com/citations?user=BUDh_4wAAAAJ&hl=zh-CN&oi=sra), [M Chu](https://scholar.google.com/citations?user=G8FHnt8AAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
We delve into the physics-informed neural reconstruction of smoke and obstacles through sparse-view RGB videos, tackling challenges arising from limited observation of complex dynamics. Existing physics-informed neural networks often emphasize short-term physics constraints, leaving the proper preservation of long-term conservation less explored. We introduce Neural Characteristic Trajectory Fields, a novel representation utilizing Eulerian neural fields to implicitly model Lagrangian fluid trajectories. This topology-free, auto-differentiable representation facilitates efficient flow map calculations between arbitrary frames as well as efficient velocity extraction via auto-differentiation. Consequently, it enables end-to-end supervision covering long-term conservation and short-term physics priors. Building on the representation, we propose physics-informed trajectory learning and integration into NeRF-based scene reconstruction. We enable advanced obstacle handling through self-supervised scene decomposition and seamless integrated boundary constraints. Our results showcase the ability to overcome challenges like occlusion uncertainty, density-color ambiguity, and static-dynamic entanglements. Code and sample tests are at https://github.com/19reborn/PICT_smoke.
</details>
<a href="https://arxiv.org/abs/2407.09679">📄 Paper</a>  
<a href="https://19reborn.github.io/PICT_Smoke.github.io/">🌐 Project Page</a>  
<a href="https://github.com/19reborn/PICT_smoke">💻 Code</a>

#### [NeurIPS 2024] Inferring Hybrid Neural Fluid Fields from Videos

**Authors:** [HX Yu](https://scholar.google.com/citations?user=kNKncZcAAAAJ&hl=zh-CN&oi=sra), [Y Zheng](https://scholar.google.com/citations?user=Q7Ouk0QAAAAJ&hl=zh-CN&oi=sra), [Y Gao](https://scholar.google.com/citations?user=z0BX_4wAAAAJ&hl=zh-CN&oi=sra), [Y Deng](https://scholar.google.com/citations?user=oNqBXkgAAAAJ&hl=zh-CN&oi=sra), [B Zhu](https://scholar.google.com/citations?user=atNjbs0AAAAJ&hl=zh-CN&oi=sra), [J Wu](https://scholar.google.com/citations?user=2efgcS0AAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
We study recovering fluid density and velocity from sparse multiview videos. Existing neural dynamic reconstruction methods predominantly rely on optical flows; therefore, they cannot accurately estimate the density and uncover the underlying velocity due to the inherent visual ambiguities of fluid velocity, as fluids are often shapeless and lack stable visual features. The challenge is further pronounced by the turbulent nature of fluid flows, which calls for properly designed fluid velocity representations. To address these challenges, we propose hybrid neural fluid fields (HyFluid), a neural approach to jointly infer fluid density and velocity fields. Specifically, to deal with visual ambiguities of fluid velocity, we introduce a set of physics-based losses that enforce inferring a physically plausible velocity field, which is divergence-free and drives the transport of density. To deal with the turbulent nature of fluid velocity, we design a hybrid neural velocity representation that includes a base neural velocity field that captures most irrotational energy and a vortex particle-based velocity that models residual turbulent velocity. We show that our method enables recovering vortical flow details. Our approach opens up possibilities for various learning and reconstruction applications centered around 3D incompressible flow, including fluid re-simulation and editing, future prediction, and neural dynamic scene composition. Project website: https://kovenyu. com/HyFluid/.</details>

</details>
<a href="https://arxiv.org/abs/2312.06561">📄 Paper</a>  
<a href="https://github.com/y-zheng18/HyFluid">💻 Code</a>

### 2022

#### [ACM ToG] Physics Informed Neural Fields for Smoke Reconstruction with Sparse Data

**Authors:** [M Chu](https://scholar.google.com/citations?user=G8FHnt8AAAAJ&hl=zh-CN&oi=sra), [L Liu](https://scholar.google.com/citations?user=HZPnJ9gAAAAJ&hl=zh-CN&oi=sra), [Q Zheng](https://scholar.google.com/citations?user=yOnb0EcAAAAJ&hl=zh-CN&oi=sra), E Franz, [HP Seidel](https://scholar.google.com/citations?user=s2Ibok8AAAAJ&hl=zh-CN&oi=sra), [C Theobalt](https://scholar.google.com/citations?user=eIWg8NMAAAAJ&hl=zh-CN&oi=sra), [R Zayer](https://scholar.google.com/citations?user=txnPmm8AAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
High-fidelity reconstruction of dynamic fluids from sparse multiview RGB videos remains a formidable challenge, due to the complexity of the underlying physics as well as the severe occlusion and complex lighting in the captured data. Existing solutions either assume knowledge of obstacles and lighting, or only focus on simple fluid scenes without obstacles or complex lighting, and thus are unsuitable for real-world scenes with unknown lighting conditions or arbitrary obstacles. We present the first method to reconstruct dynamic fluid phenomena by leveraging the governing physics (ie, Navier -Stokes equations) in an end-to-end optimization from a mere set of sparse video frames without taking lighting conditions, geometry information, or boundary conditions as input. Our method provides a continuous spatio-temporal scene representation using neural networks as the ansatz of density and velocity solution functions for fluids as well as the radiance field for static objects. With a hybrid architecture that separates static and dynamic contents apart, fluid interactions with static obstacles are reconstructed for the first time without additional geometry input or human labeling. By augmenting time-varying neural radiance fields with physics-informed deep learning, our method benefits from the supervision of images and physical priors. Our progressively growing model with regularization further disentangles the density-color ambiguity in the radiance field, which allows for a more robust optimization from the given input of sparse views. A pretrained density-to-velocity fluid model is leveraged in addition as the data prior to avoid suboptimal velocity solutions which underestimate vorticity but trivially fulfill physical equations. Our method exhibits high-quality results with relaxed constraints and strong flexibility on a representative set of synthetic and real flow captures. Code and sample tests are at https://people.mpi-inf.mpg.de/~mchu/projects/PI-NeRF/.
</details>
<a href="https://dl.acm.org/doi/pdf/10.1145/3528223.3530169">📄 Paper</a>  
<a href="https://rachelcmy.github.io/pinf_smoke/">🌐 Project Page</a>  
<a href="https://github.com/RachelCmy/pinf_smoke">💻 Code</a>

## Representive Basic Methods: 3D Reconstruction

### 2024

#### [SOTA🔥] PGSR: Planar-based Gaussian Splatting for Efficient and High-Fidelity Surface Reconstruction

**Authors:** [Danpeng Chen](https://arxiv.org/search/cs?searchtype=author&query=Chen,+D), [Hai Li](https://arxiv.org/search/cs?searchtype=author&query=Li,+H), [Weicai Ye](https://arxiv.org/search/cs?searchtype=author&query=Ye,+W), [Yifan Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+Y), [Weijian Xie](https://arxiv.org/search/cs?searchtype=author&query=Xie,+W), [Shangjin Zhai](https://arxiv.org/search/cs?searchtype=author&query=Zhai,+S), [Nan Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+N), [Haomin Liu](https://arxiv.org/search/cs?searchtype=author&query=Liu,+H), [Hujun Bao](https://arxiv.org/search/cs?searchtype=author&query=Bao,+H), [Guofeng Zhang](https://arxiv.org/search/cs?searchtype=author&query=Zhang,+G)

<details span><summary><b>Abstract</b></summary>
Recently, 3D Gaussian Splatting (3DGS) has attracted widespread attention due to its high-quality rendering, and ultra-fast training and rendering speed. However, due to the unstructured and irregular nature of Gaussian point clouds, it is difficult to guarantee geometric reconstruction accuracy and multi-view consistency simply by relying on image reconstruction loss. Although many studies on surface reconstruction based on 3DGS have emerged recently, the quality of their meshes is generally unsatisfactory. To address this problem, we propose a fast planar-based Gaussian splatting reconstruction representation (PGSR) to achieve high-fidelity surface reconstruction while ensuring high-quality rendering. Specifically, we first introduce an unbiased depth rendering method, which directly renders the distance from the camera origin to the Gaussian plane and the corresponding normal map based on the Gaussian distribution of the point cloud, and divides the two to obtain the unbiased depth. We then introduce single-view geometric, multi-view photometric, and geometric regularization to preserve global geometric accuracy. We also propose a camera exposure compensation model to cope with scenes with large illumination variations. Experiments on indoor and outdoor scenes show that our method achieves fast training and rendering while maintaining high-fidelity rendering and geometric reconstruction, outperforming 3DGS-based and NeRF-based methods.
</details>
<a href="https://arxiv.org/abs/2406.06521">📄 Paper</a>  
<a href="https://zju3dv.github.io/pgsr/">🌐 Project Page</a>  
<a href="https://github.com/zju3dv/PGSR">💻 Code</a>

#### [ACM SIGGRAPH Asia 2024 & ACM ToG] Gaussian Opacity Fields: Efficient Adaptive Surface Reconstruction in Unbounded Scenes

**Authors:** [Zehao Yu](https://arxiv.org/search/cs?searchtype=author&query=Yu,+Z), [Torsten Sattler](https://arxiv.org/search/cs?searchtype=author&query=Sattler,+T), [Andreas Geiger](https://arxiv.org/search/cs?searchtype=author&query=Geiger,+A)

<details span><summary><b>Abstract</b></summary>
Recently, 3D Gaussian Splatting (3DGS) has demonstrated impressive novel view synthesis results, while allowing the rendering of high-resolution images in real-time. However, leveraging 3D Gaussians for surface reconstruction poses significant challenges due to the explicit and disconnected nature of 3D Gaussians. In this work, we present Gaussian Opacity Fields (GOF), a novel approach for efficient, high-quality, and adaptive surface reconstruction in unbounded scenes. Our GOF is derived from ray-tracing-based volume rendering of 3D Gaussians, enabling direct geometry extraction from 3D Gaussians by identifying its levelset, without resorting to Poisson reconstruction or TSDF fusion as in previous work. We approximate the surface normal of Gaussians as the normal of the ray-Gaussian intersection plane, enabling the application of regularization that significantly enhances geometry. Furthermore, we develop an efficient geometry extraction method utilizing Marching Tetrahedra, where the tetrahedral grids are induced from 3D Gaussians and thus adapt to the scene's complexity. Our evaluations reveal that GOF surpasses existing 3DGS-based methods in surface reconstruction and novel view synthesis. Further, it compares favorably to or even outperforms, neural implicit methods in both quality and speed.
</details>
<a href="https://drive.google.com/file/d/1_IEpaSqDP4DzQ3TbhKyjhXo6SKscpaeq/view">📄 Paper</a>  
<a href="https://niujinshuchong.github.io/gaussian-opacity-fields/">🌐 Project Page</a>  
<a href="https://github.com/autonomousvision/gaussian-opacity-fields">💻 Code</a>

#### [ACM SIGGRAPH 2024 & ACM ToG] 2D Gaussian Splatting for Geometrically Accurate Radiance Fields

**Authors:** [B Huang](https://scholar.google.com/citations?user=5da8iKwAAAAJ&hl=zh-CN&oi=sra), [Z Yu](https://scholar.google.com/citations?user=Z8MwnzsAAAAJ&hl=zh-CN&oi=sra), [A Chen](https://scholar.google.com/citations?user=fuR1FBwAAAAJ&hl=zh-CN&oi=sra), [A Geiger](https://scholar.google.com/citations?user=SrVnrPcAAAAJ&hl=zh-CN&oi=sra), [S Gao](https://scholar.google.com/citations?user=fe-1v0MAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
3D Gaussian Splatting (3DGS) has recently revolutionized radiance field reconstruction, achieving high quality novel view synthesis and fast rendering speed without baking. However, 3DGS fails to accurately represent surfaces due to the multi-view inconsistent nature of 3D Gaussians. We present 2D Gaussian Splatting (2DGS), a novel approach to model and reconstruct geometrically accurate radiance fields from multi-view images. Our key idea is to collapse the 3D volume into a set of 2D oriented planar Gaussian disks. Unlike 3D Gaussians, 2D Gaussians provide view-consistent geometry while modeling surfaces intrinsically. To accurately recover thin surfaces and achieve stable optimization, we introduce a perspective-correct 2D splatting process utilizing ray-splat intersection and rasterization. Additionally, we incorporate depth distortion and normal consistency terms to further enhance the quality of the reconstructions. We demonstrate that our differentiable renderer allows for noise-free and detailed geometry reconstruction while maintaining competitive appearance quality, fast training speed, and real-time rendering.
</details>
<a href="https://arxiv.org/abs/2403.17888">📄 Paper</a>  
<a href="https://surfsplatting.github.io/">🌐 Project Page</a>  
<a href="https://github.com/hbb1/2d-gaussian-splatting">💻 Code</a>

### 2023

#### [ACM SIGGRAPH 2023 & ACM ToG] 3D Gaussian Splatting for Real-Time Radiance Field Rendering

**Authors:** [Bernhard Kerbl](https://arxiv.org/search/cs?searchtype=author&query=Kerbl,+B), [Georgios Kopanas](https://arxiv.org/search/cs?searchtype=author&query=Kopanas,+G), [Thomas Leimkühler](https://arxiv.org/search/cs?searchtype=author&query=Leimk%C3%BChler,+T), [George Drettakis](https://arxiv.org/search/cs?searchtype=author&query=Drettakis,+G)

<details span><summary><b>Abstract</b></summary>
Radiance Field methods have recently revolutionized novel-view synthesis of scenes captured with multiple photos or videos. However, achieving high visual quality still requires neural networks that are costly to train and render, while recent faster methods inevitably trade off speed for quality. For unbounded and complete scenes (rather than isolated objects) and 1080p resolution rendering, no current method can achieve real-time display rates. We introduce three key elements that allow us to achieve state-of-the-art visual quality while maintaining competitive training times and importantly allow high-quality real-time (>= 30 fps) novel-view synthesis at 1080p resolution. First, starting from sparse points produced during camera calibration, we represent the scene with 3D Gaussians that preserve desirable properties of continuous volumetric radiance fields for scene optimization while avoiding unnecessary computation in empty space; Second, we perform interleaved optimization/density control of the 3D Gaussians, notably optimizing anisotropic covariance to achieve an accurate representation of the scene; Third, we develop a fast visibility-aware rendering algorithm that supports anisotropic splatting and both accelerates training and allows realtime rendering. We demonstrate state-of-the-art visual quality and real-time rendering on several established datasets.
</details>
<a href="https://arxiv.org/abs/2308.04079">📄 Paper</a>  
<a href="https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/">🌐 Project Page</a>  
<a href="https://github.com/graphdeco-inria/gaussian-splatting">💻 Code</a>

## Representive Basic Methods: Dynamic New View Synthesis

### 2024

#### [ACM SIGGRAPH Asia & ACM ToG] Dynamic Gaussian Marbles for Novel View Synthesis of Casual Monocular Videos

**Authors:** [Colton Stearns](https://arxiv.org/search/cs?searchtype=author&query=Stearns,+C), [Adam Harley](https://arxiv.org/search/cs?searchtype=author&query=Harley,+A), [Mikaela Uy](https://arxiv.org/search/cs?searchtype=author&query=Uy,+M), [Florian Dubost](https://arxiv.org/search/cs?searchtype=author&query=Dubost,+F), [Federico Tombari](https://arxiv.org/search/cs?searchtype=author&query=Tombari,+F), [Gordon Wetzstein](https://arxiv.org/search/cs?searchtype=author&query=Wetzstein,+G), [Leonidas Guibas](https://arxiv.org/search/cs?searchtype=author&query=Guibas,+L)

<details span><summary><b>Abstract</b></summary>
Gaussian splatting has become a popular representation for novel-view synthesis, exhibiting clear strengths in efficiency, photometric quality, and compositional edibility. Following its success, many works have extended Gaussians to 4D, showing that dynamic Gaussians maintain these benefits while also tracking scene geometry far better than alternative representations. Yet, these methods assume dense multi-view videos as supervision. In this work, we are interested in extending the capability of Gaussian scene representations to casually captured monocular videos. We show that existing 4D Gaussian methods dramatically fail in this setup because the monocular setting is underconstrained. Building off this finding, we propose a method we call Dynamic Gaussian Marbles, which consist of three core modifications that target the difficulties of the monocular setting. First, we use isotropic Gaussian "marbles'', reducing the degrees of freedom of each Gaussian. Second, we employ a hierarchical divide and-conquer learning strategy to efficiently guide the optimization towards solutions with globally coherent motion. Finally, we add image-level and geometry-level priors into the optimization, including a tracking loss that takes advantage of recent progress in point tracking. By constraining the optimization, Dynamic Gaussian Marbles learns Gaussian trajectories that enable novel-view rendering and accurately capture the 3D motion of the scene elements. We evaluate on the Nvidia Dynamic Scenes dataset and the DyCheck iPhone dataset, and show that Gaussian Marbles significantly outperforms other Gaussian baselines in quality, and is on-par with non-Gaussian representations, all while maintaining the efficiency, compositionality, editability, and tracking benefits of Gaussians. Our project page can be found here [this https URL](https://geometry.stanford.edu/projects/dynamic-gaussian-marbles.github.io/).
</details>
<a href="https://arxiv.org/abs/2406.18717">📄 Paper</a>  
<a href="https://geometry.stanford.edu/projects/dynamic-gaussian-marbles.github.io/">🌐 Project Page</a>  
<a href="https://github.com/coltonstearns/dynamic-gaussian-marbles">💻 Code</a>

#### [CVPR 2024] SC-GS: Sparse-Controlled Gaussian Splatting for Editable Dynamic Scenes

**Authors:** [Yi-Hua Huang](https://arxiv.org/search/cs?searchtype=author&query=Huang,+Y), [Yang-Tian Sun](https://arxiv.org/search/cs?searchtype=author&query=Sun,+Y), [Ziyi Yang](https://arxiv.org/search/cs?searchtype=author&query=Yang,+Z), [Xiaoyang Lyu](https://arxiv.org/search/cs?searchtype=author&query=Lyu,+X), [Yan-Pei Cao](https://arxiv.org/search/cs?searchtype=author&query=Cao,+Y), [Xiaojuan Qi](https://arxiv.org/search/cs?searchtype=author&query=Qi,+X)

<details span><summary><b>Abstract</b></summary>
Novel view synthesis for dynamic scenes is still a challenging problem in computer vision and graphics. Recently, Gaussian splatting has emerged as a robust technique to represent static scenes and enable high-quality and real-time novel view synthesis. Building upon this technique, we propose a new representation that explicitly decomposes the motion and appearance of dynamic scenes into sparse control points and dense Gaussians, respectively. Our key idea is to use sparse control points, significantly fewer in number than the Gaussians, to learn compact 6 DoF transformation bases, which can be locally interpolated through learned interpolation weights to yield the motion field of 3D Gaussians. We employ a deformation MLP to predict time-varying 6 DoF transformations for each control point, which reduces learning complexities, enhances learning abilities, and facilitates obtaining temporal and spatial coherent motion patterns. Then, we jointly learn the 3D Gaussians, the canonical space locations of control points, and the deformation MLP to reconstruct the appearance, geometry, and dynamics of 3D scenes. During learning, the location and number of control points are adaptively adjusted to accommodate varying motion complexities in different regions, and an ARAP loss following the principle of as rigid as possible is developed to enforce spatial continuity and local rigidity of learned motions. Finally, thanks to the explicit sparse motion representation and its decomposition from appearance, our method can enable user-controlled motion editing while retaining high-fidelity appearances. Extensive experiments demonstrate that our approach outperforms existing approaches on novel view synthesis with a high rendering speed and enables novel appearance-preserved motion editing applications. Project page: [this https URL](https://yihua7.github.io/SC-GS-web/)
</details>
<a href="https://arxiv.org/abs/2312.14937">📄 Paper</a>  
<a href="https://github.com/yihua7/SC-GS">💻 Code</a>

#### [CVPR 2024] Deformable 3D Gaussians for High-Fidelity Monocular Dynamic Scene Reconstruction

**Authors:** [Ziyi Yang](https://arxiv.org/search/cs?searchtype=author&query=Yang,+Z), [Xinyu Gao](https://arxiv.org/search/cs?searchtype=author&query=Gao,+X), [Wen Zhou](https://arxiv.org/search/cs?searchtype=author&query=Zhou,+W), [Shaohui Jiao](https://arxiv.org/search/cs?searchtype=author&query=Jiao,+S), [Yuqing Zhang](https://arxiv.org/search/cs?searchtype=author&query=Zhang,+Y), [Xiaogang Jin](https://arxiv.org/search/cs?searchtype=author&query=Jin,+X)

<details span><summary><b>Abstract</b></summary>
Implicit neural representation has paved the way for new approaches to dynamic scene reconstruction and rendering. Nonetheless, cutting-edge dynamic neural rendering methods rely heavily on these implicit representations, which frequently struggle to capture the intricate details of objects in the scene. Furthermore, implicit methods have difficulty achieving real-time rendering in general dynamic scenes, limiting their use in a variety of tasks. To address the issues, we propose a deformable 3D Gaussians Splatting method that reconstructs scenes using 3D Gaussians and learns them in canonical space with a deformation field to model monocular dynamic scenes. We also introduce an annealing smoothing training mechanism with no extra overhead, which can mitigate the impact of inaccurate poses on the smoothness of time interpolation tasks in real-world datasets. Through a differential Gaussian rasterizer, the deformable 3D Gaussians not only achieve higher rendering quality but also real-time rendering speed. Experiments show that our method outperforms existing methods significantly in terms of both rendering quality and speed, making it well-suited for tasks such as novel-view synthesis, time interpolation, and real-time rendering.
</details>
<a href="https://arxiv.org/abs/2309.13101">📄 Paper</a>  
<a href="https://guanjunwu.github.io/4dgs/index.html">🌐 Project Page</a>  
<a href="https://github.com/ingra14m/Deformable-3D-Gaussians">💻 Code</a>

#### [CVPR 2024] 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering

**Authors:** [Guanjun Wu](https://arxiv.org/search/cs?searchtype=author&query=Wu,+G), [Taoran Yi](https://arxiv.org/search/cs?searchtype=author&query=Yi,+T), [Jiemin Fang](https://arxiv.org/search/cs?searchtype=author&query=Fang,+J), [Lingxi Xie](https://arxiv.org/search/cs?searchtype=author&query=Xie,+L), [Xiaopeng Zhang](https://arxiv.org/search/cs?searchtype=author&query=Zhang,+X), [Wei Wei](https://arxiv.org/search/cs?searchtype=author&query=Wei,+W), [Wenyu Liu](https://arxiv.org/search/cs?searchtype=author&query=Liu,+W), [Qi Tian](https://arxiv.org/search/cs?searchtype=author&query=Tian,+Q), [Xinggang Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+X)

<details span><summary><b>Abstract</b></summary>
Representing and rendering dynamic scenes has been an important but challenging task. Especially, to accurately model complex motions, high efficiency is usually hard to guarantee. To achieve real-time dynamic scene rendering while also enjoying high training and storage efficiency, we propose 4D Gaussian Splatting (4D-GS) as a holistic representation for dynamic scenes rather than applying 3D-GS for each individual frame. In 4D-GS, a novel explicit representation containing both 3D Gaussians and 4D neural voxels is proposed. A decomposed neural voxel encoding algorithm inspired by HexPlane is proposed to efficiently build Gaussian features from 4D neural voxels and then a lightweight MLP is applied to predict Gaussian deformations at novel timestamps. Our 4D-GS method achieves real-time rendering under high resolutions, 82 FPS at an 800**×**800 resolution on an RTX 3090 GPU while maintaining comparable or better quality than previous state-of-the-art methods. More demos and code are available at [this https URL](https://guanjunwu.github.io/4dgs/).
</details>
<a href="https://arxiv.org/abs/2310.08528">📄 Paper</a>  
<a href="https://guanjunwu.github.io/4dgs/index.html">🌐 Project Page</a>  
<a href="https://github.com/hustvl/4DGaussians">💻 Code</a>

### 2023

#### [3DV] Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis

**Authors:** [Jonathon Luiten](https://arxiv.org/search/cs?searchtype=author&query=Luiten,+J), [Georgios Kopanas](https://arxiv.org/search/cs?searchtype=author&query=Kopanas,+G), [Bastian Leibe](https://arxiv.org/search/cs?searchtype=author&query=Leibe,+B), [Deva Ramanan](https://arxiv.org/search/cs?searchtype=author&query=Ramanan,+D)

<details span><summary><b>Abstract</b></summary>
We present a method that simultaneously addresses the tasks of dynamic scene novel-view synthesis and six degree-of-freedom (6-DOF) tracking of all dense scene elements. We follow an analysis-by-synthesis framework, inspired by recent work that models scenes as a collection of 3D Gaussians which are optimized to reconstruct input images via differentiable rendering. To model dynamic scenes, we allow Gaussians to move and rotate over time while enforcing that they have persistent color, opacity, and size. By regularizing Gaussians' motion and rotation with local-rigidity constraints, we show that our Dynamic 3D Gaussians correctly model the same area of physical space over time, including the rotation of that space. Dense 6-DOF tracking and dynamic reconstruction emerges naturally from persistent dynamic view synthesis, without requiring any correspondence or flow as input. We demonstrate a large number of downstream applications enabled by our representation, including first-person view synthesis, dynamic compositional scene synthesis, and 4D video editing.
</details>
<a href="https://arxiv.org/pdf/2308.09713">📄 Paper</a>  
<a href="https://dynamic3dgaussians.github.io/">🌐 Project Page</a>  
<a href="https://github.com/JonathonLuiten/Dynamic3DGaussians">💻 Code</a>

