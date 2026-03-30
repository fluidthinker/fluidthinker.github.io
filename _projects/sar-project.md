---
title: "Open-Source SAR Pre/Post Comparison — Sentinel-1"
excerpt: "A radar-based workflow for detecting environmental change using Sentinel-1 SAR imagery."
header:
  teaser: /assets/images/sar-cover.jpg
---

[View Project on GitHub](https://github.com/fluidthinker/opensar-conservation-monitor){: .btn .btn--primary}

## Overview

This project demonstrates how Synthetic Aperture Radar (SAR) imagery can be used to detect environmental change in conditions where optical imagery is unreliable. Using Sentinel-1 data, I built a reproducible workflow to compare pre- and post-event conditions and identify surface changes associated with flooding.

The analysis focuses on Hurricane Harvey (2017) near Freeport, Texas, where persistent cloud cover limited the effectiveness of traditional optical satellite imagery.

---

## Project Objective

Design and implement a Python-based workflow for SAR change detection that:

- Compares pre- and post-event Sentinel-1 imagery  
- Highlights differences in radar backscatter associated with surface water and land change  
- Produces clear, interpretable visual outputs for analysis and communication  

## Data and tools

- Sentinel-1 SAR imagery
- Python
- Jupyter notebooks
- Raster processing workflows
- Visualization techniques for change detection

## Workflow

1. Define an area of interest and time window.
2. Retrieve Sentinel-1 SAR imagery for pre- and post-event dates.
3. Process and normalize radar backscatter values.
4. Compare pre/post conditions to identify change.
5. Generate visual outputs to highlight areas of difference.

## Results


<p>Pre- and post-event SAR imagery comparison:</p>

<table>
  <tr>
    <th>Pre-Event</th>
    <th>Post-Event</th>
  </tr>
  <tr>
    <td>
      <img src="/assets/images/pre_rgb_shared.png" alt="Pre-event SAR composite" width="420">
    </td>
    <td>
      <img src="/assets/images/sars-cover.jpg" alt="Post-event SAR composite" width="420">
    </td>
  </tr>
</table>

### Interpreting the Results

#### Context

This comparison highlights flooding impacts from Hurricane Harvey (2017) near Freeport, Texas using Sentinel-1 SAR imagery.

#### Data

Sentinel-1 SAR (VV/VH composite, shared stretch applied to both images)

---

#### What the colors represent

- **Green tones** → Vegetation and stable land surfaces  
- **Dark areas (black/blue)** → Water or low radar return  
- **Purple / magenta tones** → Changes in radar backscatter (indicative of flooding, increased soil moisture, or surface disturbance)

---

#### What to look for

- Focus on **coastal and low-lying areas** between the two images  
- In the post-event image, notice the **increase in purple-toned regions**  
- These areas reflect changes in surface conditions, consistent with flooding after Hurricane Harvey  

---

#### Key takeaway

The post-event image shows expanded areas of radar backscatter variation along the coastline near Freeport, Texas, indicating flooding and surface water change following Hurricane Harvey. This demonstrates how SAR imagery enables reliable change detection even when optical imagery is limited by cloud cover.


---

#### Key takeaway

The post-event image shows expanded areas of radar backscatter variation along the coastline near Freeport, Texas, indicating flooding and surface water change following Hurricane Harvey. This demonstrates how **SAR imagery enables reliable change detection even when optical imagery is limited by cloud cover**.
**Key takeaway:**
The post-event image shows a clear increase in radar backscatter variation in coastal zones, suggesting environmental change that would not be easily observable using optical imagery alone.



## What I learned

This project strengthened my understanding of radar-based remote sensing and how SAR data differs from optical imagery. It also reinforced the importance of building workflows that remain reliable under real-world constraints like cloud cover.

## Why it matters

SAR-based approaches enable consistent environmental monitoring in regions where optical imagery is unreliable. This has important implications for conservation, disaster response, and long-term environmental analysis.
