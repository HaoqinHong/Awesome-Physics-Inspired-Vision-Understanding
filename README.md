# Awesome-Physics-Inspired-3D-Reconstruction-and-Simulation
A curated list of papers and open-source resources focused on Physics-Inspired 3D Reconstruction and Simulation, intended to keep pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

- [Physics-Informed Fluid Reconstruction](#PI-Fluid)
- [Solution of Inverse Problems](#InverseProblems)
- [Simulation Method Based on 3D Gaussian Splatting](#Sim3DGS)
- [Reconstruction and Simulation Method Incorporating LLM](#SimLLM)

## Physics-Informed Fluid Reconstruction

## 2022
### 1.Physics Informed Neural Fields for Smoke Reconstruction with Sparse Data
**Authors:** M Chu, L Liu, Q Zheng, E Franz, HP Seidel, C Theobalt, R Zayer<details span>
<summary><b>Abstract</b></summary>
High-fidelity reconstruction of dynamic fluids from sparse multiview RGB videos remains a formidable challenge, due to the complexity of the underlying physics as well as the severe occlusion and complex lighting in the captured data. Existing solutions either assume knowledge of obstacles and lighting, or only focus on simple fluid scenes without obstacles or complex lighting, and thus are unsuitable for real-world scenes with unknown lighting conditions or arbitrary obstacles. We present the first method to reconstruct dynamic fluid phenomena by leveraging the governing physics (ie, Navier -Stokes equations) in an end-to-end optimization from a mere set of sparse video frames without taking lighting conditions, geometry information, or boundary conditions as input. Our method provides a continuous spatio-temporal scene representation using neural networks as the ansatz of density and velocity solution functions for fluids as well as the radiance field for static objects. With a hybrid architecture that separates static and dynamic contents apart, fluid interactions with static obstacles are reconstructed for the first time without additional geometry input or human labeling. By augmenting time-varying neural radiance fields with physics-informed deep learning, our method benefits from the supervision of images and physical priors. Our progressively growing model with regularization further disentangles the density-color ambiguity in the radiance field, which allows for a more robust optimization from the given input of sparse views. A pretrained density-to-velocity fluid model is leveraged in addition as the data prior to avoid suboptimal velocity solutions which underestimate vorticity but trivially fulfill physical equations. Our method exhibits high-quality results with relaxed constraints and strong flexibility on a representative set of synthetic and real flow captures. Code and sample tests are at https://people.mpi-inf.mpg.de/~mchu/projects/PI-NeRF/.
</details>
  [📄 Paper](https://dl.acm.org/doi/pdf/10.1145/3528223.3530169) | [🌐 Project Page](https://rachelcmy.github.io/pinf_smoke/) | [💻 Code](https://github.com/RachelCmy/pinf_smoke) 
