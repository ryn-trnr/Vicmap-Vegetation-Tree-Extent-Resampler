# Vicmap-Vegetation-Tree-Extent-Resampler
Python script to stitch together the entire Vicmap Vegetation Tree Extent dataset and output one file of full state coverage, and resample from the base resolution of 20cm to whatever resolution is input.

The Vicmap Vegetation Tree Extent dataset is described as: 'A presence/absence of tree cover dataset is derived from statewide dataset aerial photography with a minimum of 20cm pixel resolution. The mapping of tree cover was based a upon a machine learning technique. Tree cover is defined as woody vegetation greater than approximatley two metres in height.' Accessed from here: https://datashare.maps.vic.gov.au/search?q=uuid%3Df6800447-ef34-5f66-acaa-77a5f2936546

## Directions ##

1. Install Python and GDAL. Use of conda is recommended.
   
2. Place all zipped folders into the same destination as the python script.

<img width="764" height="381" alt="image" src="https://github.com/user-attachments/assets/95f80067-0d1a-4f97-8e76-9510db7ac1ce" />

3. On line 10 of `victoria_tree_canopy_cover.py` edit target_resolution as you require. Default is 5 metres.
  
4. In terminal `cd <folder destination>` and then `python victoria_tree_canopy_cover.py`

5. Log print statements in the terminal will update you on progress, and upon completion `victoria_5m.tif` will land in your folder destination.
