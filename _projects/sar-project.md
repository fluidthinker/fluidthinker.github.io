---
title: "Open-Source SAR Pre/Post Comparison — Sentinel-1"
excerpt: "A radar-based workflow for detecting environmental change using Sentinel-1 SAR imagery."
header:
  teaser: /assets/images/sar-cover.jpg
---

[View Project on GitHub](https://github.com/fluidthinker/opensar-conservation-monitor){: .btn .btn--primary}

## Why I built this

Optical satellite imagery is often limited by cloud cover, especially in regions where environmental monitoring is most critical. I wanted to explore how Synthetic Aperture Radar (SAR) data could be used as a reliable alternative for detecting change over time.

This project focuses on using Sentinel-1 SAR imagery to compare conditions before and after an event or time period, with an emphasis on building a clear and reproducible workflow.

## Project goal

The goal was to design an open-source workflow that enables pre/post comparison using SAR data, allowing users to identify changes in surface conditions regardless of weather or lighting constraints.

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
      <img src="/assets/images/pre_rg_shared.png" alt="Pre-event SAR composite" width="420">
    </td>
    <td>
      <img src="/assets/images/sars-cover.jpg" alt="Post-event SAR composite" width="420">
    </td>
  </tr>
</table>

## What I learned

This project strengthened my understanding of radar-based remote sensing and how SAR data differs from optical imagery. It also reinforced the importance of building workflows that remain reliable under real-world constraints like cloud cover.

## Why it matters

SAR-based approaches enable consistent environmental monitoring in regions where optical imagery is unreliable. This has important implications for conservation, disaster response, and long-term environmental analysis.
