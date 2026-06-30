![Kai Liu](https://img.kayphoto.today/photo-main/%E8%AF%81%E4%BB%B6%E7%85%A7_%E7%99%BD_3_4.png)

# Kai Liu

Kai Liu received the B.E. degree in Automation from the School of Automation, Central South University, Changsha, China, in 2025. He is currently pursuing the M.S. degree in Software Engineering at Xi'an Jiaotong University.

His research interests include embodied intelligence, vision-language navigation, vision-language-action models, computer vision, and physically grounded 3D asset generation for robotics.

## Education

- **Xi'an Jiaotong University**, M.S. in Software Engineering, 2025.9-2028.6
- **Central South University**, B.E. in Automation, 2021.9-2025.6

Academic record: weighted GPA 91.64/100, undergraduate rank 4/27, CET-6 578. Core courses include Python Programming, Advanced Mathematics, Linear Algebra, Complex Variables, and Data Structures.

## Selected Research And Projects

### LANDER-Nav: Progressive Landmark-Schema Grounding for Multi-Granularity Open-Vocabulary Navigation

**Status:** AAAI submission, first author  
**Period:** 2026.3-present  
**Project page:** [LANDER-Nav details](projects/lander-nav/)

LANDER-Nav studies multi-granularity open-vocabulary goal navigation, where an embodied agent must follow free-form language to locate category-, region-, or instance-level targets in unseen environments. Instead of compressing the whole instruction into a single query vector, the method parses the instruction into a landmark schema consisting of target, anchor, context, and relation.

My work focuses on the overall method design and evaluation pipeline. I formulate the navigation process as progressive grounding over frontier evidence, object-memory entity binding, and verifiable endpoint selection. The framework introduces role-conditioned spatial voting, landmark-anchored object binding, and Landmark-Ray Endpoint Search to improve instance disambiguation and stopping viewpoint reliability.

Experiments on LangMap and HM3D-OVON show consistent improvements. On LangMap, the Overall SR/SPL improves from 42.0/25.3 to 45.5/28.6 compared with MTU3D, with stronger gains on region- and instance-level targets.

### PhysArtGen: Interactive and Physically Controllable Articulated 3D Assets Generation

**Status:** AAAI submission, second author  
**Period:** 2025.7-2026.2  
**Project page:** [PhysArtGen details](projects/physartgen/)

PhysArtGen is a text-conditioned framework for generating articulated 3D assets that can be compiled into URDF and used for physics-based robotic interaction. The project targets a key bottleneck in embodied intelligence: scalable creation of diverse, physically coherent, and interactive assets for simulation and sim-to-real policy learning.

I participated in the design of the physically grounded generation pipeline, including the Physics Adapter for preserving relative part scale and position, and the Actor-Critic-Verifier multi-agent optimization system for generating and refining URDF links and joints. I also contributed to PhysArtSet construction and experimental evaluation.

The project builds PhysArtSet from PartNet-Mobility, covering 29 object categories, 16 canonical part types, over 1,000 high-quality instances, and 2,800 synthesized parts. The Physics Adapter reduces Part Pose Error from 0.236 to 0.029, and the Actor-Critic-Verifier architecture improves URDF physical consistency and joint modeling.

### A Comprehensive Review and Future Perspectives on Embodied AI Large Models

**Status:** Published in *Radio Engineering*, second author  
**Period:** 2025.6-2025.9

This survey reviews embodied AI large models with a focus on Vision-Language-Action (VLA) systems. It summarizes how VLA models connect visual perception, language understanding, multimodal fusion, and action decoding, and traces the field's evolution from modular pipelines to end-to-end unified architectures.

My contribution centers on literature review and technical organization. I investigated representative visual encoders, language backbones, multimodal fusion strategies, action-token modeling, diffusion- and flow-based continuous action generation, simulators, datasets, benchmarks, and evaluation metrics.

The survey covers resources such as AI2-THOR, Habitat, Isaac Sim/Gym, OXE, BridgeData V2, ALFRED, and LIBERO, and discusses open challenges including generalization, data efficiency, long-horizon reasoning, and real-time response.

## Awards

- Second Prize, the 14th Chinese Mathematics Competitions, 2023.01
- Second Prize, Hunan Provincial College Student Mathematics Competition, 2022.12
- Second Prize, Hunan Rice Cup Smart Car Competition, 2024.02
- Second Prize, Central South University Physics Competition, 2023.04
- National Encouragement Scholarship, 2022.09 and 2023.09
- Outstanding Student, Central South University, 2022.09 and 2023.09

