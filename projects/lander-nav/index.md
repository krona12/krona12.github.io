---
layout: project
title: LANDER-Nav
subtitle: Progressive Landmark-Schema Grounding for Multi-Granularity Open-Vocabulary Navigation
kicker: AAAI submission, first author
---

<figure class="project-figure">
  <img src="{{ '/assets/projects/lander-nav/framework.png' | relative_url }}" alt="LANDER-Nav framework">
  <figcaption>LANDER-Nav grounds open-vocabulary navigation instructions through frontier evidence, object binding, and verifiable endpoint search.</figcaption>
</figure>

## Overview

LANDER-Nav studies multi-granularity open-vocabulary goal navigation, where an embodied agent must follow free-form language to locate category-, region-, or instance-level targets in unseen environments. A core difficulty is that natural-language goals often contain target objects, reference landmarks, spatial relations, and contextual constraints at the same time.

Instead of compressing the full instruction into a single query vector, LANDER-Nav parses it into a **landmark schema** with four roles: target, anchor, context, and relation. The same schema is then used across exploration, entity grounding, and stopping viewpoint selection.

## Method

The framework maintains online scene memory, including object memory, explored occupancy maps, and frontier candidates. It performs three progressive grounding steps:

- **Evidence Grounding:** selects frontiers that are most likely to complete missing semantic evidence.
- **Entity Grounding:** binds targets in object memory through landmark-anchored object binding and role-conditioned spatial voting.
- **Endpoint Grounding:** searches for reachable, visible, and relation-verifiable stopping viewpoints through Landmark-Ray Endpoint Search.

This design keeps landmark support active throughout navigation, improving instance-level disambiguation and making the final stop more verifiable.

## Results

Experiments are conducted on LangMap and HM3D-OVON. On LangMap, LANDER-Nav improves Overall SR/SPL from **42.0/25.3** to **45.5/28.6** compared with MTU3D. The gains are especially clear on region- and instance-level goals, where anchor and relation cues are critical.

## My Role

I am the first author of this work. I designed the landmark-schema grounding formulation, organized the navigation decision process into evidence, entity, and endpoint grounding, and contributed to the method implementation, experiments, ablations, and paper writing.

