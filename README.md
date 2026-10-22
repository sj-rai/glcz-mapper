### Global Local Climate Zone Mapper

#### 1. Project Summary
Rapid urbanization and climate change have intensified the Urban Heat Island (UHI) effect
- where built-up areas experience significantly higher temperatures than rural surroundings.
Standard satellite maps simply label areas as ”urban” or ”natural,” ignoring critical differences
in building height, density, and greenery.
This project delivers a Deep Learning Analytics Pipeline using TorchGeo that converts raw
European Space Agency (ESA) satellite imagery into detailed Local Climate Zone (LCZ) maps.
These maps classify landscapes into 17 standardized microclimate categories (e.g., Compact
High-Rise, Open Low-Rise, Dense Forest), helping city planners to identify extreme heat risks
and target green infrastructure where it is needed most.
#### 2. The Challenge: Why Simple Satellites Are Not Enough
Mapping microclimates requires understanding both surface materials (concrete vs. grass)
and 3D urban geometry (building heights and shadows):
• Optical Satellites (Color / Infra-red): Excellent at spotting vegetation and water,
but struggle to differentiate a 20-story glass skyscraper from a 2-story glass office building.
• Radar Satellites: Can penetrate cloud cover and bounce off vertical walls to measure
3D structural roughness and building height, but lack surface color detail.
Achieving accurate, automated climate mapping requires fusing these two distinct satellite
viewpoints into a single intelligent vision model.
#### 3. Solution & Technical Strategy
The pipeline uses a multi-modal artificial intelligence approach that combines radar and optical
satellite feeds:
• Dual-Branch Data Fusion: A two-stream neural network processes Sentinel-1 (Radar)
and Sentinel-2 (Optical) imagery simultaneously, blending physical structural signa-
tures with surface material profiles.
• Global Multi-City Intelligence: The network will be trained across 52 diverse global
cities (such as Berlin, Tokyo, and S˜ao Paulo) to ensure it performs accurately across
varying global architectural styles.
• Actionable Map Exports: The model processes raw satellite grids and outputs color-
coded thematic maps that integrate directly into Geographic Information Systems (GIS)
used by urban planning departments.
#### 4. Key Real-World Applications
• Urban Heat Island Mitigation: Identifies specific neighborhoods vulnerable to heat
stress to prioritize tree-planting initiatives and cool-roof installations.
• Energy Grid Forecasting: Predicts localized surge demands for summer air condition-
ing across high-density residential zones.
• Climate Policy & City Planning: Provides an automated, repeatable tool for city
councils to measure urban density changes over time without manual field surveys.