---
title: "Home"
layout: splash
permalink: /
header:
  overlay_color: "#1f2937"
  overlay_filter: 0.35
  caption: "Geospatial systems, remote sensing, and decision-support tools"
intro:
  - excerpt: "I build geospatial data workflows and environmental analysis tools using Python, GIS, remote sensing, and spatial databases."
feature_row:
  - image_path: /assets/images/elephant-butte-cover.png
    alt: "Remote Sensing of Surface Water Dynamics"
    title: "Remote Sensing of Surface Water Dynamics — Elephant Butte Reservoir"
    excerpt: "A remote sensing workflow for tracking surface water dynamics at Elephant Butte Reservoir."
    url: /projects/elephant-butte-reservoir/
    btn_label: "View Project"
    btn_class: "btn--primary"
  - image_path: /assets/images/trip-animation-cover.png
    alt: "Spatiotemporal trip visualization project"
    title: "Spatiotemporal Trip Visualization (PostGIS + Python)"
    excerpt: "A geospatial workflow that transforms trip records into a time-based animated map using PostGIS, SQL, and Python."
    url: /projects/trip-visualization/
    btn_label: "View Project"
    btn_class: "btn--primary"
  - image_path: /assets/images/sars-cover.jpg
    alt: "SAR Change Detection project"
    title: "SAR Change Detection (Sentinel-1)"
    excerpt: "Radar-based change detection using Sentinel-1 to compare pre- and post-event conditions."
    url: /projects/sar-project/
    btn_label: "View Project"
    btn_class: "btn--primary"


---

## About this portfolio

This site highlights selected work across remote sensing, spatial analytics, data engineering, and visualization. My focus is on building clear, reproducible workflows that help people understand environmental patterns and make better decisions.

## Featured projects

{% include feature_row %}

{% include feature_row id="feature_row2" %}
