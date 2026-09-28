# Bogota-Water-Quality (2019–2025)

Geospatial assessment of surface water quality in Bogotá, combining in-situ monitoring data (RCHB/OAB network) with Sentinel-2 satellite imagery from Google Earth Engine. The analysis covers TSS, COD, total nitrogen and total phosphorus, and includes trend analysis and hotspot detection linked to land-use pressure.

Authors: Frenklin Vata & Maycol Zaraza Aguilera


The full method, results and discussion are in the notebook.

## Run it in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/FrenklinV/Bogota-Water-Quality/blob/main/Project_Water_Quality_G4_VF.ipynb)

**What you need:** a Google account and a free [Google Earth Engine](https://earthengine.google.com/) account.

1. Click the **Open in Colab** badge above.
2. Run the cells from the top, in order. The notebook downloads this repository and reads the input files from `data/`. You don't need to upload anything.
3. When the Earth Engine cell asks you to log in, click the link, sign in with your Google account, and paste the code back.
4. In that cell, set `EE_PROJECT` to your own Google Cloud / Earth Engine project ID. If you don't have one, create a free one at [code.earthengine.google.com/register](https://code.earthengine.google.com/register).
5. Keep running the cells. Results and figures are saved in the `output/` folder inside the Colab session.

**Notes**
- The Sentinel-2 extraction step takes about 40 minutes.
- The interactive maps only appear while the notebook is running in Colab. On GitHub you see the static figures.

## Repository contents

| Folder / file | Content |
|---|---|
| `Project_Water_Quality_G4_VF.ipynb` | Full analysis notebook |
| `data/` | Input data (water quality xlsx and shapefiles). See `data/README.md` |
| `images/` | Figures used in the notebook |

## Data sources

- In-situ water quality: Observatorio Ambiental de Bogotá (RCHB network)
- Land cover: CORINE Land Cover 2022, IDEAM
- Satellite imagery: Sentinel-2 L2A (`COPERNICUS/S2_SR_HARMONIZED`) via Google Earth Engine

  ## What you can see on GitHub

GitHub previews the notebook without running it, so some outputs don't display:

- Static charts, tables and figures **are shown**.
- The interactive maps (geemap/folium) and Plotly charts **are not shown** on GitHub, and may appear blank. GitHub doesn't run interactive content.
- To see them, open the notebook in Colab, log in to Earth Engine, and run the cells. The four Earth Engine maps only appear when the cells are run.
