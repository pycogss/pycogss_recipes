# ⚙️ PyCoGSS recipes! ⚙️

This is a collection of scripts and Jupyter notebooks that helps facilitate scalable and reproducible analysis of landscape data. 

`aoi-2-dataset.ipynb` demonstrates how to search within an area of interest (AOI) in Google Earth Engine for topographic and multispectral data in the Arctic, download that data, and convert it to a format that can be used to create labels and training data for image segmentation via [Doodleverse](https://github.com/Doodleverse) tools. For now this includes functions but in the future this tool may take the form of a package or functions/methods within a package. But for now you can run this notebook to collect your own data. Stay tuned!

`imagery-dem-profiler` uses `geemap` to load up a visual of a landscape and then you can draw multiple topographic profiles on that imagery. Great for exploring water tracks!

`spectral-change-detector` creates annual composite images to look at pixelwise changes in spectral indices over time. Great for exploring greening and browning of water tracks!

# Other resources

- [NASA EarthData recipes](https://www.earthdata.nasa.gov/learn/gis/data-recipes) and [NASA Earthdata Cloud Cookbook](https://nasa-openscapes.github.io/earthdata-cloud-cookbook/)