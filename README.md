# Smart Farming Interface Prototype

A personal **Streamlit interface prototype** by Gcina Mdizwa, exploring how satellite, UAV and agricultural analysis themes could be presented through a web application.

## Current implementation

The application renders a styled landing page with a navigation-style header, a hero section, four feature cards and a footer. It demonstrates Python-driven interface composition and custom HTML/CSS inside Streamlit.

**Current scope:** presentation and interface design. The navigation labels and `Read More` button do not implement page routing or a downstream analysis workflow.

The cards describe potential application areas. Satellite processing, UAV processing, irrigation recommendations and yield prediction are **not implemented** in the current `app.py`.

## Run locally

```bash
git clone https://github.com/Gcina22/Gcinapy2.git
cd Gcinapy2
python -m venv .venv
```

Activate the environment (`.venv\Scripts\activate` on Windows or `source .venv/bin/activate` on macOS/Linux), then run:

```bash
python -m pip install streamlit
python -m streamlit run app.py
```

The current entry point imports only Streamlit. `requirements.txt` also lists libraries that could support future mapping and raster work; those are not currently used by `app.py`. Package versions have not yet been pinned or validated across platforms.

## Included datasets

The repository contains `Summer_2025_Hyacinth_Map.tif`, `Winter_2025_Hyacinth_Map.tif` and `water_hyacinth_2025.csv`. The current application does not read these files. Their collection methods, location, class definitions, accuracy and reuse terms are not documented here; they should not be treated as validated evidence solely from their filenames.

## Design notes and limitations

- The background photograph is loaded from an external Unsplash URL and requires internet access.
- This prototype does not connect to satellite services, field sensors or live farm data.
- No crop-health, irrigation or yield model is currently provided.
- Desktop and mobile accessibility/usability have not yet been formally evaluated.

## Next improvements

Choose one working use case, such as a clearly labelled seasonal water-hyacinth map comparison. Document the data, implement the workflow, validate its outputs and add a screenshot and reproducible example before describing the app as an analytical dashboard.

## Author

[Gcina Mdizwa](https://www.linkedin.com/in/gcina-mdizwa-501025249/) — GIS, remote sensing and Python geospatial development.

No code or data reuse licence is currently specified in this repository.
