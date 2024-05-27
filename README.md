# Flood Return Period Analysis: A Case Study of a Polish Region
### **Summary**
><p>Using a dataset of polish address points, flood hazard maps and administrative unit boundaries, the number of locations affected by different flood return periods in various administrative areas (powiats) of Lubuskie voivodeship in Poland were calculated.The analysis considered flood return periods of 10, 20, 50, 100, 200, and 500 years.</p>
><p>To perform the analysis, Python was used along with several packages, including the ElementTree module for extracting data from XML documents containing address points, GeoPandas for creating GeoDataFrames and conducting geospatial operations, and Rasterio for extracting values from raster data.</p>

### **Flood return period**
>A flood return period is a statistical concept to estimate the likelihood of a specific flood event occurring within a given period of time and it is expressed in term of years, for instance:
> - a 100-year return period flood has a 1% chance of occurring in any given year
> - a 50-year return period flood has 2% chance of occurring in any given year
> - a 10-year return period flood has 10% chance of occurring in any given year

### **Results summary**
![results_table_2](https://github.com/mkupisie/Flood_Return_Period_Analysis_A_Case_Study_of_a_Polish_Region/assets/130785524/f4aa6598-b401-4e44-a818-e9232422dbc3)

>The sum of points within powiats across different return periods provides an overall assessment of the cumulative impact on all Lubuskie voivodeship. The highest cumulative impact can be observed for the 500-year return period, reaching 28919 points (14,9% of all points in the dataset). The highest number of affected locations for this return period is noted in **Powiat Nowosolski** (44,6% of all points in the dataset for this powiat). This data implies that in these locations the flood has a 0.2% chance of  occurrence in any given year within a 500-year period. **Powiat Nowosolski**, compared to other powiats, has the highest number of affected locations for each return period. 36,5% of all points in the dataset for Nowosolski powiat has a 10% chance of flood occurrence in any given year within a 10-year period. For the rest of return periods the result is respectively: 39,6% for 20-year return period, 42,3% for 50-year return period and 44,2% for 500-year return period.


>**Such statistics for other powiats are collected in the table below:**
![percentage](https://github.com/mkupisie/Flood_Return_Period_Analysis_A_Case_Study_of_a_Polish_Region/assets/130785524/26684ca8-a42e-4543-b54c-eb8598a35fed)

>0% chance of flood occurrence for each return period can be noticed in **Świebodziński** powiat where none of 11345 locations is affected by any return period. Low impact across all return periods is observed in **Wschowski**, **Zielona Góra**, **Żarski** and **Sulęciński** powiat. For these powiats less than 10% of locations are affected by each return period. More than 10% of locations affected by return period appear **Strzelecko-drezdenecki** and **Krośnieński** powiat and for these powiats above 1000 locations are affected by 100,200 and 500-year return periods and by 50-year return period for **Krośnieński** powiat. The next powiats: **Gorzowski** and **Zielonogórski** are having the percentage of the locations affected by return periods above 10% and this amount is increasing with each return period up to 17,4% (from 1885 locations affected up to 3092 for **Zielonogórski** powiat and from 1922 to 2817 for **Gorzowski** powiat). 
The following powiats: **Międzyrzecki**, **Słubicki**, **Żagański** and **Gorzów Wielkopolski** reach the percentage value of the locations affected above 20% with the following amount of locations affected across all return periods:
>- **Międzyrzecki:** 1287 (10-year return period) to 3047 (500-year return period)
>- **Słubicki:** 1470 (10-year return period) to 2107 (500-year return period)
>- **Żagański:** 2361 (10-year return period) to 3408 (500-year return period)
>- **Gorzów Wielkopolski:** 2074 (10-year return period) to 2684 (500-year return period).


