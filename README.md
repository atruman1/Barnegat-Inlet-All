Barnegat Inlet Sediment Change Analysis  
Author: Andrew Truman  
Contact: TRUMANAJ@GMAIL.COM 
Date: August 2025  
Last Updated: 08/28/2025

Overview:  
This repository contains the primary datasets and supporting tables used in the analysis for the Master’s thesis titled *Transformative Shifts: Sediment Loss and Flood Tidal Delta Decline in Barnegat Inlet, New Jersey*. Data includes historical shoreline area, dredging records, bathymetry estimates, and climate factors (e.g., rainfall, sea level rise) compiled from government sources and academic literature from the years 1930-2024.

---

Structure & Data Manifest:

1. Land Area Change  
   - Description: Landmass area (acres) for each island cluster, the dike, and the shoal for each study year (1930-2024).  
   - Source: Digitized from georeferenced aerial imagery (NJDEP, USGS, NOAA).  
   - Use: Supports Figures 4 & 5.  
   - Units: Acres.

2. Powell Comparison 
   - Description: Flood tidal delta volume vs. tidal prism comparison using Powell et al. (2006) framework. Includes Barnegat data points for 1940, 1975, and 1994.  
   - Source: This study’s bathymetric estimates & tidal prism from Powell regression line.  
   - Use: Figure 9.  
   - Units: Volume (m³), Prism (m³).

3. Dredging Volumes  
   - Description: Dredging volumes compiled from USACE Chief of Engineers Annual Reports.  
   - Source: USACE reports, 1940–2012.  
   - Use: Figure 9.  
   - *Units*: Cubic yards (CY).

4. Land Area vs. Rainfall  
   - Description: Yearly land area values vs. annual rainfall to explore potential climate correlation.  
   - Source: NJ Climatology Office, NOAA, and geospatial imagery analysis.  
   - Use: Figure 11.  
   - Units: Acres, Inches/year.

5. Data  
   - Description: Intermediate calculations and values from land area and volume analyses.  
   - Source: Derived.  
   - Use: Internal reference; not cited directly in figures.  
   - Units: Mixed.

6.Percent Change  
   - Description: Percentage change in landmass area per cluster per time period.  
   - Source: Derived from “Land Area Change.”  
   - Use: Text discussion.  
   - Units: Percent (%).

7. Precip  
   - Description: Monthly/seasonal rainfall data used to calculate annual precipitation.  
   - Source: NJ Climatology Office.  
   - Use: Supporting data for climate analysis.  
   - Units: Inches.

8. Precip Annual  
   - Description: Annualized rainfall values with rolling means.  
   - Source: Derived from “Precip.”  
   - Use: Figure 11.  
   - Units: Inches/year.

9. Bathymetry XSection - Figure not used in Thesis report  
   - Description: Cross-section profiles extracted from NOAA nautical charts showing bathymetric evolution from 1957 to 2017.  
   - Source: NOAA Historical Chart Archive.  
   - Use: Text discussion.  
   - Units: Depth (feet), distance (feet).

---
 
|   Figure   |   Input Excel File(s)     |   Sheet / Layer   |     Input ArcGIS Files    |        Projection       |         Source        |      Units      |           Used For            |
|------------|---------------------------|-------------------|---------------------------|-------------------------|-----------------------|-----------------|-------------------------------|
| Figure  1  |          NA               |        NA         |      Bing Tile Service    | NAD 1983 NJ State Plane |       www.bing.com    |       NA        |       Aerial Overview         |
| Figure  2  |          NA               |        NA         | BI / Soils / soilmu_a_aoi |        WGS 1984         |  USDA Web Soil Survey |       NA        | Regional Soil Identification  |
| Figure  3  |          NA               |        NA         |            NA             |           NA            |  NOAA Station 8534720 |      M/yr       |    Demonstrate Sea Level Rise |
| Figure  4  | Thesis Table Upload.xlsx  |       Data        |     BI / Land Area        | NAD 1983 NJ State Plane | NOAA Nautical Charts  |      acres      |  Land Area Change Comparison  |
| Figure  5  | Thesis Table Upload.xlsx  |       Data        |     BI / Land Area        | NAD 1983 NJ State Plane | NOAA Nautical Charts  |      acres      |  Land Area Change Comparison  |
| Figure  6  | Thesis Table Upload.xlsx  |       Data        |     BI / Land Area        | NAD 1983 NJ State Plane | NOAA Nautical Charts  |      acres      |  Land Area Change Comparison  |
| Figure  7  |          NA               |        NA         |   BI / Bathymetry Data    | NAD 1983 NJ State Plane | NOAA Nautical Charts  |      feet       |  Bathymetry Raster Comparison |
| Figure  8  |          NA               |        NA         |           NA              |           NA            |  Seabergh et al, 2003 |   percent/year  |           Text Support        |
| Figure  9  | Thesis Table Upload.xlsx  | Powell Comparison |           NA              |           NA            | Powell et al, 2006    |   cubic meters  |       Powell comparison       |
| Figure 10  | Thesis Table Upload.xlsx  |  Dredging Volumes |     BI / Land Area        | NAD 1983 NJ State Plane |         USACE         |cubic yards/acres| Land Area/Dredging Comparison |
| Figure 11  | Thesis Table Upload.xlsx  |   Precip Annual   |     BI / Land Area        | NAD 1983 NJ State Plane | NJ Climatology Office |   inches/acres  | Land Area/Rainfall Comparison |  
  
---

Processing & Analysis Notes:
- Landmass areas were digitized in ArcGIS Pro from historic aerial imagery using shoreline delineation at MHW (mean high water).
- Bathymetric rasters were interpolated from digitized depth soundings taken from NOAA nautical charts.
- Volume estimates for delta comparison were calculated using planform area × assumed depth, validated by elevation contours.
- Dredging data were transcribed from USACE Annual Reports and grouped by decade.
- Climate data (rainfall and sea level) were reviewed visually against landmass trends but not statistically correlated.

---

Reproduction Notes:
- Analysis was conducted using Microsoft Excel and ArcGIS Pro (v3.4.2).  
- No scripts or code-based automation was used.  
- All source references are included in the main thesis bibliography.  
- For reuse or citation, please contact the author or cite this dataset as:  
  “Truman, A. (2025). Supplemental Data for Barnegat Inlet Sediment Study. Montclair State University Thesis Repository.”
