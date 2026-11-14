## Hi, I'm Yanice

I'm a GIS Developer at Opta Information Intelligence, a Verisk company, based in Vancouver. I write Python that turns municipal open data into standard geospatial datasets, and I spend a lot of my time on the checks that catch bad data before anyone uses it.

**Day to day:** Python (pandas, geopandas, ArcPy), SQL, ArcGIS Pro, ArcGIS REST services, Jupyter, Git, AWS S3

**Background:** Master of Geomatics for Environmental Management, University of British Columbia · B.Sc. Geography, South China Normal University

### Projects

| Project | What it is |
| --- | --- |
| [civic-address-qa](https://github.com/YaniceZ/civic-address-qa) | Downloads civic address points from municipal ArcGIS REST services, maps each source onto one schema, and runs data quality checks. Run on Thunder Bay (45,102 addresses) and West Kelowna (18,255); the address parser matched Thunder Bay's own split fields on 99.95% of rows. |
| [address-pipeline](https://github.com/YaniceZ/address-pipeline) | Loads those address files into a GeoParquet lake and a DuckDB warehouse. A schema contract rejects bad files before they land, SQL models build the tables, and SQL checks gate the run. The contract caught a real bug in civic-address-qa: YAML read `province: ON` as the boolean True. |
| [autoates-bc](https://github.com/YaniceZ/autoates-bc) | AutoATES gives each cell of a mountain one avalanche terrain class and no sense of how far to trust it. This reruns the whole chain with perturbed elevation, forest and threshold inputs to get a probability per class, for a block of the BC Coast Mountains, then checks those probabilities against a lidar-based run and against two expert benchmark maps. Research only, not for route decisions. |
| [trips](https://github.com/YaniceZ/trips) | Installable, offline-capable trip planner: day-by-day itineraries, Leaflet maps, booking countdowns, cost splitting and calendar export. A shared engine checks each trip's content before it loads; optional multi-user sync uses Supabase. |
| [epic-pass-guide](https://github.com/YaniceZ/epic-pass-guide) | Bilingual reference site for Epic Pass holders, with an interactive map and offline support. |

### Contact

[LinkedIn](https://www.linkedin.com/in/yanice-zeng)
