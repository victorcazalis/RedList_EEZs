Global shapefile of countries EEZs matching Red List (SIS) list of Countries of Occurrence (level 0 and some level 1)


***
NEWS IN V_2023.2
- I split Turkey into Asia and European parts as well as Russia (European part, East Asia, Central Asia) according to their level 1 in SIS. This was needed to enable restricting distributions for European Red List assessments of marine species.

***
NEWS IN V_2023.1

- I added two columns: lookup gives the lookup of the entity (country or subnational entity) according to the lookup list from SIS Connect; lk_SIS0 gives the lookup of the parent country (ie level 0 for SIS) of each entity.

- Columns have been renamed with shorter names: SIS_nm0 for SIS_name0, SIS_nm1 for SIS_name1, lookup and lk_SIS0

***

General methodology: The base map used to create this shapefile is the EEZ map of Flanders Marine Institute (2019). Maritime Boundaries Geodatabase: Maritime Boundaries and Exclusive Economic Zones (200NM), version 11. Available online at https://www.marineregions.org/. https://doi.org/10.14284/386

I used the table in EEZ_crosswalk.csv to transform names of EEZs in names fitting the Red List countries taxonomy. Some countries that are divided into several parts had several associated with EEZ (e.g., Chile has a main part, Easter island, and Desventurados islands). If this matched the Red List subnational entities, I attributed the Red List subnational entity name in column "SIS_name1". Note however that this is not complete (e.g., conversely to the subnational entities in the Red List countries of occurrence, Turkey EEZs are not split between Turkey in Europe and Turkey in Asia, because the EEZs map did not provide such split).
