# HiQ-LAI-v1.1

The High-Quality Leaf Area Index (HiQ-LAI) is derived from reprocessed MODIS LAI C6.1 product by SpatioTemporal Information Compositing Algorithm (STICA). This method integrates information from multiple dimensions, including pixel quality information, spatiotemporal correlation, and original observations, to improve the raw MODIS LAI retrievals with poor quality. The HiQ-LAI covers the period from 2000 to 2023 year, with spatial resolutions of 500m/5km for global vegetation area and temporal resolutions of 8 days.

The HiQ-LAI product file name follows certain naming convention, providing useful information about a specific product. More details can found in DataDescriptionForHiQLAI.docx, and data read examples can also be viewed in this file.

The dataset links are as follows:
1) https://doi.org/10.5281/zenodo.12615116 (spatial resolution is 5km and temporal resolution is 8 days, Nearest-neighbour)
2) https://code.earthengine.google.com/?asset=projects/verselab-398313/assets/HiQ_LAI/wgs_500m_8d (spatial resolution is 500m and temporal resolution is 8 days)
3) https://code.earthengine.google.com/?asset=projects/verselab-398313/assets/HiQ_LAI/wgs_5km_8d_Bicubic (spatial resolution is 5km and temporal resolution is 8 days, Bicubic)

Data Citation: Kai Yan, Jingrui Wang, Marie Weiss, & Ranga B. Myneni. (2023). A High-Quality Reprocessed MODIS Leaf Area Index Dataset (HiQ-LAI) (Version 1) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.8296768

### Data update note (25 June 2024):

1) In response to the problem of missing data in the original HiQ-LAI data due to large gaps in the original data (MODIS LAI), we carried out data filling work. Specifically, we found the average value of the pixel values at the same position in the same phase of the image in other years for the missing pixel on the corresponding image as a replacement. The image elements thus obtained were treated as the same as the backup algorithm in the MQA calculations (MQA=4).
2) The data range was extended to 2023.
