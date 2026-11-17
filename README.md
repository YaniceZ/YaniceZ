## Hi, I'm Yanice

I'm a GIS Developer at Opta Information Intelligence, a Verisk company, based in Vancouver. I write Python that turns municipal open data into standard geospatial datasets, and I spend a lot of my time on the checks that catch bad data before anyone uses it.

**Day to day:** Python (pandas, geopandas, ArcPy), SQL, ArcGIS Pro, ArcGIS REST services, Jupyter, Git, AWS S3

**Background:** Master of Geomatics for Environmental Management, University of British Columbia · B.Sc. Geography, South China Normal University

### Projects

| Project | What it is |
| --- | --- |
| [civic-address-qa](https://github.com/YaniceZ/civic-address-qa) | Downloads civic address points from municipal ArcGIS REST services, maps each source onto one schema, and runs data quality checks. Run on Thunder Bay (45,102 addresses) and West Kelowna (18,255); the address parser matched Thunder Bay's own split fields on 99.95% of rows. |
| [address-pipeline](https://github.com/YaniceZ/address-pipeline) | Loads those address files into a GeoParquet lake and a DuckDB warehouse. A schema contract rejects bad files before they land, SQL models build the tables, and SQL checks gate the run. The contract caught a real bug in civic-address-qa: YAML read `province: ON` as the boolean True. |
| [datacenter-land](https://github.com/YaniceZ/datacenter-land) | What land did the data centre boom take? 2,378 OpenStreetMap campuses in 101 countries, read against annual 10 m land cover, GHSL population and Sentinel-2. Campuses built in 2018–2023 replaced 1,376 ha, 42% of it cropland; 79% of them are on rural land, against about a quarter of older ones. Footprints hold no more cropland than the land around them, so the farmland loss comes from regional siting. Includes a preprint, the campus dataset and bootstrap uncertainty. |
| [canada-fire-severity](https://github.com/YaniceZ/canada-fire-severity) | Asks whether stands killed by mountain pine beetle burned more severely, for the 2024 Jasper and 2023 McDougall Creek wildfires. Burn severity from Sentinel-2, pre-fire decline from Landsat, canopy loss from 1 m LiDAR, and AlphaEarth embeddings, all scored on 3 km blocks a model never saw. Declined stands burned about the same or less in both fires; in the logged Okanagan forest the decline map mostly found clearcuts until harvest areas were taken out. |
| [autoates-bc](https://github.com/YaniceZ/autoates-bc) | AutoATES gives each cell of a mountain one avalanche terrain class and no sense of how far to trust it. A verified, fast rewrite of the chain is rerun hundreds of times with perturbed elevation, forest and threshold inputs, then tested on five lidar-covered BC blocks (leave one out) and two expert benchmark maps. The ensemble flags where 30 m maps are likely wrong (AUC 0.68) but beats a fair baseline by only 11% in Brier score; forest cover is the largest source of uncertainty. Written up as a [manuscript draft](https://github.com/YaniceZ/autoates-bc/blob/main/paper/manuscript.md). Research only, not for route decisions. |
| [trips](https://github.com/YaniceZ/trips) | Installable, offline-capable trip planner: day-by-day itineraries, Leaflet maps, booking countdowns, cost splitting and calendar export. A shared engine checks each trip's content before it loads; optional multi-user sync uses Supabase. |
| [epic-pass-guide](https://github.com/YaniceZ/epic-pass-guide) | Bilingual reference site for Epic Pass holders, with an interactive map and offline support. |

### Contact

[LinkedIn](https://www.linkedin.com/in/yanice-zeng)
