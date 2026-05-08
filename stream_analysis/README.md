# This is the core database for "Stream Analysis for Geoscientists", a project by PyCoGSS and Nick Lewis

## In this directory
| Notebook Name | Description |
|--|--|
|1_DEM_DOWNLOADER.ipynb (jupyter notebook)|Download your DEM based on bounding coordinates and dataset type, stores as 'gtiff_N_E_S_W.tiff' in proj_dir|
|2_WSHED_SPLITTER.ipynb|Uses USGS WDB to parse out individual watersheds of your selected size from your larger DEM. <br><br>Stores in wshed_dems\ as wshedname.tiff<br><br>Reprojects into northing, easting.<br><br>Stores reprojected tiffs in reproj\ as wshedname_reproj.tiff<br><br>Uses XDEM to generate TRI rasters.  Stores in tri_pngs as wshedname.png|
|3_KNICKPOINT_ID.ipynb|Uses lsdtopytools to create CSVs of knickpoints identified and ksn values of all pixels along streams identified.<br><br>Stores knickpoints in kp_csvs/ as wshedname_reproj_knickpoints.csv<br><br>Stores ksn values of all stream pixels in ksn_csvs/ as wshedname_reproj_ksn.csv|
|4_LSHT.ipynb|Identifies LSHT (above 90% elevation, below 90% slope) points.<br><br>Creates chiplots of all streams, stores under chi_plots/ as wshedname_chiplot.png<br><br>Identifies knickpoints within a distance of LSHT and stores in lsht_kps/ as wshedname_lsht_kps.csv<br><br>Maps LSHT points and LSHT knickpoints, stores in kps_mapped/ as wshedname_mapped.png|
|ksn_env.yml|Used to create ksn environment for use with LSDTopyTools in notebook 3.|
|structure.txt|Shows final structure of project directory if all notebooks are run.|
|requirements.txt|Used to create virtual env for notebooks 1, 2, and 4.|
