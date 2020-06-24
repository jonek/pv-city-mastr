# Analyse Photovoltaic Systems in MaStR

The tools and data in this repository provide insight into photovoltaic systems deployed in Germany.

## Data Source

The analysed data is provided by the German [Markstammdatenregister](https://www.bundesnetzagentur.de/DE/Sachgebiete/ElektrizitaetundGas/Unternehmen_Institutionen/DatenaustauschundMonitoring/Marktstammdatenregister/MaStR_node.html#doc514816bodyText4) (MaStR).

## Data Processing

You can reproduce the following data processing steps on your computer:

1. Download data (from MaStR): [data/README.md](data/README.md)
2. Convert data from Excel to CSV
   - Migration parts 1 and 2 (data before Jan 2019): [notebooks/convert-MaStR-Migration-to-CSV.ipynb](notebooks/convert-MaStR-Migration-to-CSV.ipynb)
   - data since Jan 2019: [notebooks/convert-MaStR-since20190131-to-CSV.ipynb](notebooks/convert-MaStR-since20190131-to-CSV.ipynb)
3. Extract data for a given city
   - Migration parts 1 and 2: [notebooks/extract-city-from-MaStR-before20190201.ipynb](notebooks/extract-city-from-MaStR-before20190201.ipynb)
   - data since Jan 2019: [notebooks/extract-city-from-MaStR-since20190131.ipynb](notebooks/extract-city-from-MaStR-since20190131.ipynb)
4. Combine data partitions
   - Migration part 1
   - Migration part 2
   - data since 2019

Each step is implemented in a shell script or a Jupyter notebook.

## Data Visualisation

Either in a Jupyter notebook or in an Observable. (TODO)

## Data Partitioning

To enable further analysis of the data, the combined partitions (see "Data Processing" step 4 above) are split up again.
This results in handable chunks of data, one partition per federal state (German: *Bundesland*).

You can find these partitions in `states/<state name>.csv`. (TODO)