---
layout: project
title: PhysArtGen
subtitle: Interactive and Physically Controllable Articulated 3D Assets Generation
kicker: AAAI submission, second author
---

<figure class="project-figure">
  <img src="{{ '/assets/projects/physartgen/framework.png' | relative_url }}" alt="PhysArtGen framework">
  <figcaption>PhysArtGen goes from semantic understanding, to part-level 3D generation, to Actor-Critic-Verifier URDF optimization.</figcaption>
</figure>

## Overview

PhysArtGen is a text-conditioned framework for generating articulated 3D assets that are not only visually plausible, but also physically controllable and usable in robotic simulation. It addresses a key bottleneck in embodied intelligence: building diverse, interactive digital assets at scale.

Existing 3D generation methods often produce static, monolithic meshes. PhysArtGen instead generates part-level articulated objects, assembles them into URDF, and supports downstream robotic interaction in simulation and real-world transfer.

## Framework

The pipeline contains three stages:

- **Semantic Understanding:** an MLLM decomposes a natural-language prompt into object categories, part categories, spatial relations, and part-relation pairs.
- **Articulated Object Parts Generation:** a conditional latent diffusion model generates part geometry under class, style, and physical constraints. The Physics Adapter preserves relative part size and position.
- **URDF Generation:** an Actor-Critic-Verifier multi-agent system generates and refines link placement, joint attributes, and compilable URDF code.

## Demonstration

<video class="project-video" controls preload="metadata">
  <source src="{{ '/assets/projects/physartgen/demo.mp4' | relative_url }}" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Dataset And Results

The project constructs PhysArtSet from PartNet-Mobility, covering **29 object categories**, **16 canonical part types**, **1,000+ high-quality instances**, and **2,800+ synthesized parts**.

The Physics Adapter reduces Part Pose Error from **0.236** to **0.029**, showing that shared normalization substantially improves relative part placement. In URDF generation, the Actor-Critic-Verifier system improves final physical consistency and joint modeling over actor-only generation.

## My Role

I am the second author of this work. I participated in the design of the Physics Adapter, the Actor-Critic-Verifier URDF optimization workflow, PhysArtSet construction, and experimental evaluation.
