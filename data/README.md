# Data

Input datasets used by `Project_Water_Quality_G4_VF.ipynb`.

## Files

| File | Description | Source |
|---|---|---|
| `RCHB-Tradicional_Consolidado3.xlsx` | In-situ water quality measurements from Bogotá's Water Quality Network (RCHB). Sheets: `CONSOLIDADO` (5,395 measurements, 72 columns, 2006–2025, 34 stations), `ESTACIONID` (30 monitoring stations with coordinates), `PARAMETROS` (36 parameters). The notebook uses 2019–2025 only. | Observatorio Ambiental de Bogotá (OAB) |
| `CLC_2022_AOI.*` | CORINE Land Cover 2022, clipped to the study area. Used to compute land-use pressure. CRS: MAGNA-SIRGAS (geographic). | IDEAM Geoportal |
| `AOI_DS.*` | Study area boundary for Bogotá. CRS: WGS 84. | Local administrative data |
| `BodyWater_BTA.*` | Water body polygons of Bogotá with a 200 m buffer. CRS: MAGNA-SIRGAS (geographic). | Local administrative data |

Each shapefile is made of several files (`.shp`, `.shx`, `.dbf`, `.prj`, `.cpg`). All of them are needed for the notebook to read it.

## Not stored here

- **Sentinel-2 imagery** is read online from Google Earth Engine (`COPERNICUS/S2_SR_HARMONIZED`). It needs a free Earth Engine account.

## Generated files

Files created by the notebook are written to `output/` (created automatically when the notebook runs).

## Licenses and citation

Check the license of each source before reuse. Data belongs to the organisations above.
