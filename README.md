# Kai Liu Personal Homepage

This repository is the local workspace for Kai Liu's GitHub Pages personal homepage. The site is based on a light, concise Jekyll resume theme and has been reorganized around research experience in embodied intelligence, vision-language navigation, VLA models, and physically grounded 3D asset generation.

## Profile Source

The primary content source is [`resume.md`](resume.md). It contains:

- English biography and education background
- Research interests
- Three selected research/project entries
- Awards and academic record

The website should be updated from `resume.md` first, then reflected in the Jekyll homepage configuration and project pages.

## Page Structure

The homepage presents three selected works:

1. **LANDER-Nav: Progressive Landmark-Schema Grounding for Multi-Granularity Open-Vocabulary Navigation**
2. **PhysArtGen: Interactive and Physically Controllable Articulated 3D Assets Generation**
3. **A Comprehensive Review and Future Perspectives on Embodied AI Large Models**

Only two standalone detail links are intentionally created:

- [`projects/lander-nav/`](projects/lander-nav/) for LANDER-Nav
- [`projects/physartgen/`](projects/physartgen/) for PhysArtGen

The embodied AI survey remains a concise homepage entry, without a separate detail page.

## Local Assets

The two standalone project pages use local, fixed assets:

- `assets/projects/lander-nav/framework.png`
- `assets/projects/physartgen/framework.png`
- `assets/projects/physartgen/demo.mp4`

These assets were copied or rendered into the repository so the GitHub Pages site does not depend on the original external corpus folder.

## Deployment

When ready, push this folder to a GitHub repository named:

```text
krona12.github.io
```

Then enable GitHub Pages with **Deploy from a branch** as the source. Use the `master` branch and the repository root.

Expected public URL:

```text
https://krona12.github.io
```

## Template Credit

The original visual base comes from [`sproogen/modern-resume-theme`](https://github.com/sproogen/modern-resume-theme), released under the MIT License.
