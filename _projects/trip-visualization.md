---
title: "Spatiotemporal Trip Visualization (PostGIS + Python)"
excerpt: "A geospatial workflow for transforming trip records into a time-based animated map using PostGIS, SQL, and Python."
header:
  teaser: /assets/images/trip-animation-cover.png
---

[View Project on GitHub](https://github.com/fluidthinker/bike-trip-spatiotemporal-animation){: .btn .btn--primary}

## Overview

## Overview
## Overview

This project demonstrates how bike-share trip data can be transformed into a spatiotemporal visualization that reveals how travel patterns shift throughout the day. The data represents bike rental stations where individual trips begin, with trip starts aggregated to census tracts and grouped into 30-minute time intervals.

Using PostGIS and Python, I built a reproducible workflow that converts these trip start records into a sequence of consistent map frames, showing how activity intensifies and moves across the city over time.
---

## Project Objective

Design and implement a workflow that:

- Aggregates trip activity by census tract and half-hour interval
- Uses spatial SQL and Python-based mapping to generate consistent map frames
- Produces an animated visualization that makes trip patterns easy to explore over time

## Data and tools

- PostgreSQL / PostGIS
- SQL
- Python
- GeoPandas
- Matplotlib
- ImageIO
- Census tract geometry
- Trip origin data

## Workflow

## Workflow

1. Identify the analysis period and define 30-minute time intervals.
2. Join trip origin records to bike station locations.
3. Perform a spatial join to assign each station to a census tract using PostGIS.
4. Aggregate trip starts by census tract and time interval using SQL.
5. Export aggregated results for use in Python-based visualization.
6. Generate one map frame per time interval using GeoPandas and Matplotlib.
7. Apply consistent map extent, legend, and styling across all frames.
8. Compile frames into a final animated GIF using Pillow (PIL).


## Results

<p>Single frame from the final animation:</p>

<img src="/assets/images/trip-animation-cover.png" alt="Single frame from spatiotemporal trip visualization" width="700">

<p><strong>Animated summary:</strong> Trip starts by census tract at 30-minute intervals</p>

<img src="/assets/images/trip_starts_by_tract_halfhour_polished.gif" alt="Animated map of trip starts by census tract over time" width="700">

### Interpreting the Results

#### Context

This visualization shows how trip origins shift across census tracts over time, allowing spatial and temporal patterns to be viewed together rather than in separate charts or maps.

#### Data

Trip origin activity aggregated by census tract and half-hour interval, then rendered as a sequence of choropleth map frames.

---

#### What to look for

- Notice how trip intensity changes across the day rather than remaining evenly distributed
- Compare which census tracts become more active during different time intervals
- Look for periods where activity becomes concentrated in specific parts of the city

---

#### What the map shows

- **Darker / more saturated tracts** → Higher concentration of trip starts during that half-hour interval
- **Lighter tracts** → Lower concentration of trip starts
- **Stable map extent and layout** → Makes it easier to compare changes over time without visual distortion

---

#### Key takeaway

The animation makes it much easier to see when and where trip demand intensifies across the city. By combining spatial aggregation in PostGIS with consistent frame rendering in Python, this project turns raw trip records into a clear visual narrative about urban movement patterns.

## What I learned

This project strengthened my skills in spatial SQL, spatiotemporal aggregation, geospatial visualization, and workflow design. It also reinforced the importance of consistent map framing, legends, and layout when building animations intended for interpretation rather than just display.

## Why it matters

Trip data often contains both spatial and temporal structure that is difficult to understand in static summaries alone. Projects like this show how geospatial pipelines can turn raw event data into interpretable visual outputs that support analysis, communication, and storytelling.
