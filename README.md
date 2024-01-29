# Google_Data_Analytics_case_study
Capstone project for Google Data Analytics certificate

In this project I will use process for data analytics: Ask, Prepre, Process, Analyze, Share, and Act to come with conclusion to better understand how annual members and casul riders differ in using bycicles

After adding calcualating data in Excel I've combined add data in SQL, here is script:

DROP TABLE IF EXISTS `Cyclistic.combined_data_2023`

CREATE TABLE IF NOT EXISTS `Cyclistic.combined_data_2023`
AS (
  SELECT * FROM `Cyclistic.2023_01`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_02`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_03`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_04`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_05`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_06`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_07`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_08`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_09`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_10`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_11`
  UNION ALL
  SELECT * FROM `Cyclistic.2023_12`
);
