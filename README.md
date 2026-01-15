
# Clark County Building Age Viewer

A GitHub‑Pages app using Clark County, WA GIS:
- **TaxlotsPublic** (parcels) – contains Year Built fields (`BldgYrBlt`, `BldgEffYrBlt`)  
- **BuildingFootprints** – building outline geometry (no Year Built field)

The app provides:
- ✅ Heatmap of parcel centroids (older = hot)  
- ✅ Parcel click pop‑ups (address, year, sqft, count)  
- ✅ Building footprints *joined* with Year Built (extent‑based client join)  
- ✅ Timeline filter (≤ selected year)

**Live data sources (ArcGIS services):**
- TaxlotsPublic (weekly updates, public item):  
  https://www.arcgis.com/home/item.html?id=d8c5df2e3c4540bea23a9b2f04493a89  
- BuildingFootprints (service metadata):  
  https://gis.clark.wa.gov/arcgisfed/rest/services/ClarkView_Public/BuildingFootprints/MapServer

## Publish
1. Create repo: `clark-county-heatmap`
2. Upload `index.html` and `README.md`
3. Settings → Pages → “Deploy from branch” (main / root)
4. Your URL:

https://clarkco-heatmap.github.io/clark-county-heatmap/
