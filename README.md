# Awesome-Physics-Inspired-3D-Reconstruction-and-Simulation

A curated list of papers and open-source resources focused on Physics-Inspired 3D Reconstruction and Simulation, intended to keep pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

- [Solution of Inverse Problems Using NeRF or 3DGS](#solution-of-inverse-problems-using-nerf-or-3dgs)
- [Simulation Method Based on 3D Gaussian Splatting](#simulation-method-based-on-3d-gaussian-splatting)
- [Reconstruction and Simulation Method Incorporating LLM](#reconstruction-and-simulation-method-incorporating-llm)
- [Physics-Informed Fluid Reconstruction](#physics-informed-fluid-reconstruction)

## Related Knowledge Resources 
- [Physics for Computer Graphics Self-Studying Plan](https://github.com/HaoqinHong/Physics-for-Graphics-Notes)
- **[Keep Updating] Paper Interpretation** (Only allowed for studying 🫡)
    - **Foundation Papers**
      - [3D Gaussian Splatting](https://drive.google.com/file/d/1oM7mbGSl8osIrZPsmdXvczVDCtFTxJ1D/view?usp=drive_link)
      - [2D Gaussian Splatting](https://drive.google.com/file/d/1QFrkBhMLyqLRCn7bujKy98B0hI34PFEH/view?usp=drive_link)
      - [Deformable-Gaussians](https://drive.google.com/file/d/1rheSh8b9ddjkNqO2vwPT7PSiTZS5BnCD/view?usp=drive_link)

    - **Simulation Method**
      - [PhysGaussian](https://drive.google.com/file/d/1gGP4GepEl_6BimyBY2mKY-1maDdQF5Eo/view?usp=drive_link)
      - [PhysDreamer and KAN](https://drive.google.com/file/d/1UeIEYOUAYjqssfW6EOnoi57hhoc50uKX/view?usp=drive_link)

    - **Physics-Informed Method**
      - [Physics Informed Neural Fields](https://drive.google.com/file/d/1vperfD5crgXPBXlTtspMpOguhXVQLZmU/view?usp=drive_link)

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

#### DreamPhysics: Learning Physical Properties of Dynamic 3D Gaussians with Video Diffusion Priors

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

**Author:** [T Xie](https://scholar.google.com/citations?user=oRt4qcgAAAAJ&hl=zh-CN&oi=sra), [Z Zong](https://scholar.google.com/citations?user=6liRAk4AAAAJ&hl=zh-CN&oi=sra), [Y Qiu](https://scholar.google.com/citations?user=zPZ6ijgAAAAJ&hl=zh-CN&oi=sra), [X Li](https://scholar.google.com/citations?user=xAI6xm4AAAAJ&hl=zh-CN&oi=sra), Y Feng, [Y Yang](https://scholar.google.com/citations?user=-z2_nggAAAAJ&hl=zh-CN&oi=sra), [C Jiang](https://scholar.google.com/citations?user=jTivVMEAAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
We introduce PhysGaussian a new method that seamlessly integrates physically grounded Newtonian dynamics within 3D Gaussians to achieve high-quality novel motion synthesis. Employing a customized Material Point Method (MPM) our approach enriches 3D Gaussian kernels with physically meaningful kinematic deformation and mechanical stress attributes all evolved in line with continuum mechanics principles. A defining characteristic of our method is the seamless integration between physical simulation and visual rendering: both components utilize the same 3D Gaussian kernels as their discrete representations. This negates the necessity for triangle/tetrahedron meshing marching cubes cage meshes or any other geometry embedding highlighting the principle of" what you see is what you simulate (WS^ 2)". Our method demonstrates exceptional versatility across a wide variety of materials--including elastic entities plastic metals non-Newtonian fluids and granular materials--showcasing its strong capabilities in creating diverse visual content with novel viewpoints and movements.
</details>
<a href="https://arxiv.org/abs/2311.12198">📄 Paper</a>  
<a href="https://xpandora.github.io/PhysGaussian/">🌐 Project Page</a>  
<a href="https://github.com/XPandora/PhysGaussian">💻 Code</a>

## Reconstruction and Simulation Method Incorporating LLM

### 2024

#### Sim Anything: Automated 3D Physical Simulation of Open-world Scene with Gaussian Splatting

[Haoyu Zhao](https://arxiv.org/search/cs?searchtype=author&query=Zhao,+H), [Hao Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+H), [Xingyue Zhao](https://arxiv.org/search/cs?searchtype=author&query=Zhao,+X), [Hongqiu Wang](https://arxiv.org/search/cs?searchtype=author&query=Wang,+H), [Zhiyu Wu](https://arxiv.org/search/cs?searchtype=author&query=Wu,+Z), [Chengjiang Long](https://arxiv.org/search/cs?searchtype=author&query=Long,+C), [Hua Zou](https://arxiv.org/search/cs?searchtype=author&query=Zou,+H)

<details span><summary><b>Abstract</b></summary>
Recent advancements in 3D generation models have opened new possibilities for simulating dynamic 3D object movements and customizing behaviors, yet creating this content remains challenging. Current methods often require manual assignment of precise physical properties for simulations or rely on video generation models to predict them, which is computationally intensive. In this paper, we rethink the usage of multi-modal large language model (MLLM) in physics-based simulation, and present Sim Anything, a physics-based approach that endows static 3D objects with interactive dynamics. We begin with detailed scene reconstruction and object-level 3D open-vocabulary segmentation, progressing to multi-view image in-painting. Inspired by human visual reasoning, we propose MLLM-based Physical Property Perception (MLLM-P3) to predict mean physical properties of objects in a zero-shot manner. Based on the mean values and the object's geometry, the Material Property Distribution Prediction model (MPDP) model then estimates the full distribution, reformulating the problem as probability distribution estimation to reduce computational costs. Finally, we simulate objects in an open-world scene with particles sampled via the Physical-Geometric Adaptive Sampling (PGAS) strategy, efficiently capturing complex deformations and significantly reducing computational costs. Extensive experiments and user studies demonstrate our Sim Anything achieves more realistic motion than state-of-the-art methods within 2 minutes on a single GPU.
</details>
<a href="https://arxiv.org/abs/2411.12789">📄 Paper</a>  
<a href="https://sim-gs.github.io/">🌐 Project Page</a>  
<a>💻 Code (Not yet)</a>



#### Unleashing the Potential of Multi-modal Foundation Models and Video Diffusion for 4D Dynamic Physical Scene Simulation

[Zhuoman Liu](https://arxiv.org/search/cs?searchtype=author&query=Liu,+Z), [Weicai Ye](https://arxiv.org/search/cs?searchtype=author&query=Ye,+W), [Yan Luximon](https://arxiv.org/search/cs?searchtype=author&query=Luximon,+Y), [Pengfei Wan](https://arxiv.org/search/cs?searchtype=author&query=Wan,+P), [Di Zhang](https://arxiv.org/search/cs?searchtype=author&query=Zhang,+D)

<details span><summary><b>Abstract</b></summary>
Realistic simulation of dynamic scenes requires accurately capturing diverse material properties and modeling complex object interactions grounded in physical principles. However, existing methods are constrained to basic material types with limited predictable parameters, making them insufficient to represent the complexity of real-world materials. We introduce a novel approach that leverages multi-modal foundation models and video diffusion to achieve enhanced 4D dynamic scene simulation. Our method utilizes multi-modal models to identify material types and initialize material parameters through image queries, while simultaneously inferring 3D Gaussian splats for detailed scene representation. We further refine these material parameters using video diffusion with a differentiable Material Point Method (MPM) and optical flow guidance rather than render loss or Score Distillation Sampling (SDS) loss. This integrated framework enables accurate prediction and realistic simulation of dynamic interactions in real-world scenarios, advancing both accuracy and flexibility in physics-based simulations.
</details>
<a href="https://arxiv.org/abs/2411.14423">📄 Paper</a>  
<a href="https://zhuomanliu.github.io/PhysFlow/">🌐 Project Page</a>  
<a>💻 Code (Not yet)</a>



## Physics-Informed Fluid Reconstruction

### 2024

#### [ACM SIGGRAPH 2024] Physics-Informed Learning of Characteristic Trajectories for Smoke Reconstruction

**Author:** [Y Wang](https://scholar.google.com/citations?user=AVOZmU8AAAAJ&hl=zh-CN&oi=sra), [S Tang](https://scholar.google.com/citations?user=BUDh_4wAAAAJ&hl=zh-CN&oi=sra), [M Chu](https://scholar.google.com/citations?user=G8FHnt8AAAAJ&hl=zh-CN&oi=sra)

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

