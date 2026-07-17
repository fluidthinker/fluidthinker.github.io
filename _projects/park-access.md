---
excerpt: An end-to-end geospatial data application exploring park
  accessibility across Dane County using PostGIS, GeoParquet, DuckDB,
  and Streamlit.
header:
  teaser: /assets/images/park-access-cover.jpg
title: Dane County Park Access Analysis
---

[View Live Dashboard](https://dane-county-park-access.streamlit.app/){:
.btn .btn--primary}

[View Project on
GitHub](https://github.com/fluidthinker/postgis-park-access){: .btn
.btn--inverse}

## Overview

This project explores how access to parks varies across census tracts in
Dane County, Wisconsin, and whether lower-access neighborhoods also tend
to have lower median household incomes.

I built an end-to-end geospatial data pipeline that combines U.S. Census
American Community Survey data with OpenStreetMap park polygons. Spatial
analysis was performed in PostGIS, the completed tract-level dataset was
exported to GeoParquet, and DuckDB was used to query the analytical
results for an interactive Streamlit dashboard.

The project was designed not only to produce a map, but to demonstrate
how spatial data can move through a reproducible engineering workflow
and become an accessible decision-support application.

------------------------------------------------------------------------

## Project Objective

Design and implement a geospatial data application that:

-   Measures park accessibility across Dane County census tracts
-   Compares park access with median household income
-   Separates computationally intensive spatial processing from
    interactive presentation
-   Communicates spatial patterns through an interactive map and
    supporting charts

## Data and Tools

### Data

-   U.S. Census American Community Survey (ACS)
-   Census tract boundaries
-   OpenStreetMap park polygons

### Technologies

-   Python
-   PostgreSQL / PostGIS
-   GeoPandas
-   OSMnx
-   GeoParquet
-   DuckDB
-   Streamlit
-   Folium
-   Altair

## Park Access Measures

Park accessibility was evaluated using two complementary measures:

-   **Availability** --- the amount of park space available per resident
-   **Proximity** --- the distance from each census tract to the nearest
    park

These measures were combined into four park access tiers:

-   High Access
-   Moderate Access
-   Low Access
-   Very Low Access

## Workflow

1.  Acquire census tract and demographic data.
2.  Download park polygons from OpenStreetMap.
3.  Load datasets into PostGIS.
4.  Calculate park availability and proximity metrics.
5.  Classify census tracts into park access tiers.
6.  Export results to GeoParquet.
7.  Query the analytical dataset with DuckDB.
8.  Build an interactive Streamlit dashboard using Folium.

``` text
ACS Census Data          OpenStreetMap Parks
        │                         │
        └────────────┬────────────┘
                     ▼
              PostGIS Database
                     │
              Spatial Analysis
                     │
                     ▼
              GeoParquet Export
                     │
                     ▼
                DuckDB Queries
                     │
                     ▼
          Streamlit + Folium Dashboard
```

## Interactive Dashboard

The deployed dashboard allows users to:

-   Explore park access by census tract
-   Filter the map by access tier
-   Hover over census tracts to inspect demographic and accessibility
    metrics
-   Compare park access patterns with median household income

[Open the Interactive
Dashboard](https://dane-county-park-access.streamlit.app/){: .btn
.btn--primary}

![Dane County Park Access
Dashboard](/assets/images/park-access-dashboard.png)

## Key Findings

-   Park access varies substantially across Dane County census tracts.
-   Lower-access neighborhoods generally tend to have lower median
    household incomes, although the relationship is not absolute.
-   Income explains only part of the observed spatial pattern.

## Application Architecture

A key design decision was separating computationally intensive spatial
processing from the web application.

PostGIS performs the spatial analysis. The completed results are
exported to GeoParquet. The deployed Streamlit application reads the
analytical dataset with DuckDB, allowing the dashboard to run without
requiring a live PostgreSQL database.

## What I Learned

This project strengthened my understanding of:

-   Designing reproducible geospatial data pipelines
-   Separating analysis from presentation
-   Using portable analytical formats
-   Building interactive geospatial dashboards
-   Deploying Python applications to the cloud

## Why It Matters

Access to parks supports recreation, public health, and quality of life.
This project demonstrates how modern geospatial engineering tools can
transform raw spatial data into an accessible decision-support
application.
