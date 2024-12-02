# Awesome-Physics-Inspired-3D-Reconstruction-and-Simulation

A curated list of papers and open-source resources focused on Physics-Inspired 3D Reconstruction and Simulation, intended to keep pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

- [Solution of Inverse Problems](#InverseProblems)
- [Simulation Method Based on 3D Gaussian Splatting](#Sim3DGS)
- [Reconstruction and Simulation Method Incorporating LLM](#SimLLM)
- [Physics-Informed Fluid Reconstruction](#PI-Fluid)

## Solution of Inverse Problems

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

<br>

## Physics-Informed Fluid Reconstruction

### 2024

#### [ACM SIGGRAPH 2024] Physics-Informed Learning of Characteristic Trajectories for Smoke Reconstruction

**Author:** [Y Wang](https://scholar.google.com/citations?user=AVOZmU8AAAAJ&hl=zh-CN&oi=sra), [S Tang](https://scholar.google.com/citations?user=BUDh_4wAAAAJ&hl=zh-CN&oi=sra), [M Chu](https://scholar.google.com/citations?user=G8FHnt8AAAAJ&hl=zh-CN&oi=sra)

<details span><summary><b>Abstract</b></summary>
We delve into the physics-informed neural reconstruction of smoke and obstacles through sparse-view RGB videos, tackling challenges arising from limited observation of complex dynamics. Existing physics-informed neural networks often emphasize short-term physics constraints, leaving the proper preservation of long-term conservation less explored. We introduce Neural Characteristic Trajectory Fields, a novel representation utilizing Eulerian neural fields to implicitly model Lagrangian fluid trajectories. This topology-free, auto-differentiable representation facilitates efficient flow map calculations between arbitrary frames as well as efficient velocity extraction via auto-differentiation. Consequently, it enables end-to-end supervision covering long-term conservation and short-term physics priors. Building on the representation, we propose physics-informed trajectory learning and integration into NeRF-based scene reconstruction. We enable advanced obstacle handling through self-supervised scene decomposition and seamless integrated boundary constraints. Our results showcase the ability to overcome challenges like occlusion uncertainty, density-color ambiguity, and static-dynamic entanglements. Code and sample tests are at https://github.com/19reborn/PICT_smoke.</details>
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

