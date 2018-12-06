# strava_local_heatmap.py

Python script to reproduce the Strava Global Heatmap (https://www.strava.com/heatmap) with local GPX data

## Usage:

* Download the GPX files from Strava (cf. https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export)
* Copy the GPX files to the `gpx` folder
* [Optional] For best resolution, update `max_nb_tiles` in `strava_local_heatmap.py`
* Run `python3 strava_local_heatmap.py`
* The heatmap PNG and CSV file is saved to the current directory

**heatmap.png result**
![heatmap_zoom.png](heatmap_zoom.png)

**heatmap.csv result imported in** https://umap.openstreetmap.fr (cf. https://github.com/remisalmon/strava-local-heatmap/pull/4)
![heatmap_umap.png](heatmap_umap.png)

[Dynamic Umap map (wait a few seconds)](https://umap.openstreetmap.fr/en/map/demo-heatmap_261644)

## Python dependencies:

* Python >= 3.7.0
* Requests >= 2.20.1
* NumPy >= 1.15.4
* Matplotlib >= 3.0.1
* scikit-image >= 0.14.0 (https://scikit-image.org/)

## Distribution dependencies:

### Archlinux

`sudo pacman -S tk` (cf. https://github.com/remisalmon/strava-local-heatmap/pull/3)