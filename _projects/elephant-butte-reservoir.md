---
title: "Remote Sensing of Surface Water Dynamics — Elephant Butte Reservoir"
excerpt: "A Python-based remote sensing workflow for monitoring surface water dynamics at Elephant Butte Reservoir over time."
header:
  teaser: /assets/images/elephant-butte-cover.png
---

[View Project on GitHub](https://github.com/fluidthinker/openwater-shrinking-lake-monitor){: .btn .btn--primary}

## Overview

This project demonstrates how optical satellite imagery can be used to monitor changing surface water conditions over time. Using Sentinel-2 imagery and Python-based raster workflows, I built a reproducible process to compare reservoir conditions across multiple years and communicate visible shoreline change.

The analysis focuses on Elephant Butte Reservoir in New Mexico, where changing water extent can be clearly observed through time and translated into decision-ready visual outputs.

---

## Project Objective

Design and implement a Python-based remote sensing workflow that:

- Compares reservoir conditions across multiple time periods
- Identifies visible changes in surface water extent and shoreline position
- Produces clear visual outputs for interpretation and communication

## Data and Tools

- Sentinel-2 imagery
- Python
- Jupyter notebooks
- GeoPandas
- Raster processing workflows
- Visualization outputs

## Workflow

1. Define the reservoir area of interest.
2. Gather Sentinel-2 imagery for target dates.
3. Process imagery to derive water-related outputs.
4. Compare reservoir extent across time.
5. Export static and animated visuals to support interpretation.

## Results

<p>Side-by-side comparison of reservoir conditions in September 2019 and September 2025:</p>

<table>
  <tr>
    <th>September 2019</th>
    <th>September 2025</th>
  </tr>
  <tr>
    <td><img src="/assets/images/s2_rgb_2019-09.png" alt="Sentinel-2 RGB September 2019 at Elephant Butte Reservoir" width="420"></td>
    <td><img src="/assets/images/s2_rgb_2025-09.png" alt="Sentinel-2 RGB September 2025 at Elephant Butte Reservoir" width="420"></td>
  </tr>
</table>

<p><strong>Animated summary:</strong> September surface water mask (2019–2025)</p>

![September Surface Water Mask animation](/assets/images/story_sept_2019_2025_2000ms.gif)

### Interpreting the Results

#### Context

This comparison highlights changing surface water conditions at Elephant Butte Reservoir in New Mexico using Sentinel-2 imagery across multiple years.

#### Data

Sentinel-2 optical imagery and derived surface water outputs used to compare shoreline position and reservoir extent through time.

---

#### What to look for

- Compare the visible **shoreline position** between September 2019 and September 2025
- Notice the **reduced water extent** in the later image
- Focus on exposed land areas around the reservoir margins, which indicate reservoir contraction over time

---

#### What the images show

- **Dark blue / dark water areas** → Open water
- **Tan / light brown areas near the shoreline** → Newly exposed land or reduced water coverage
- **Surrounding land surfaces** → Stable upland or non-water areas that help provide visual context for change

---

#### Key takeaway

The side-by-side comparison shows a visible reduction in surface water extent at Elephant Butte Reservoir between September 2019 and September 2025. The animated sequence reinforces this pattern across multiple years, making it easier to see how shoreline position and water coverage changed over time. Together, these outputs demonstrate how remote sensing can be used to communicate reservoir dynamics clearly and effectively.

## What I Learned

This project strengthened my skills in remote sensing workflow design, temporal comparison, reproducibility, and visual communication. It also reinforced the value of pairing static comparison images with animation to help viewers quickly understand environmental change over time.

## Why It Matters

Reservoir dynamics affect water availability, ecosystems, and downstream decision-making. Projects like this show how satellite imagery can translate environmental change into accessible visual evidence that supports understanding, communication, and planning.
