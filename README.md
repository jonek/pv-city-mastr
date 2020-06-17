# Analyse Photovoltaic Systems in MaStR

The tools and data in this repository provide insight into photovoltaic systems deployed in Germany.

## Data Source

The analysed data is provided by the German [Markstammdatenregister](https://www.bundesnetzagentur.de/DE/Sachgebiete/ElektrizitaetundGas/Unternehmen_Institutionen/DatenaustauschundMonitoring/Marktstammdatenregister/MaStR_node.html#doc514816bodyText4) (MaStR).

## Data Processing

You can reproduce the following data processing steps on your computer:

1. Download data (from MaStR)
2. Convert data from Excel to CSV
3. Extract data for a given city
4. Combine data partitions
   - Migration part 1
   - Migration part 2
   - data since 2019

Each step is implemented in a shell script or a Jupyter notebook.

## Data Visualisation

Either in a Jupyter notebook or in an Observable. (TODO)
