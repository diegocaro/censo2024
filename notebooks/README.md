# Pre-procesamiento de datos
 - [`1.0-dc-loading-maps.ipynb`](notebooks/1.0-dc-loading-maps.ipynb): Carga y procesa los datos geográficos del Censo 2024, generando archivos GeoJSON para comunas y áreas metropolitanas.
    - Archivos: [`chile_comunas.geojson`](data/processed/chile_comunas.geojson)
 - [`1.1-dc-preprocess-data.ipynb`](notebooks/1.1-dc-preprocess-data.ipynb): Limpia y convierte los microdatos de hogares, personas y viviendas a formato Parquet comprimido.
    - [`hogares_clean.parquet`](data/processed/hogares_clean.parquet)
    - [`personas_clean.parquet`](data/processed/personas_clean.parquet)
    - [`viviendas_clean.parquet`](data/processed/viviendas_clean.parquet)
 - [`1.2-dc-preprocess-tables.ipynb`](notebooks/1.2-dc-preprocess-tables.ipynb): Procesa los diccionarios de variables y genera archivos de mapeo JSON para hogares, personas y viviendas.
    - [`hogares_mapping.json`](data/processed/hogares_mapping.json)
    - [`personas_mapping.json`](data/processed/personas_mapping.json)
    - [`viviendas_mapping.json`](data/processed/viviendas_mapping.json)





Los archivos de datos raw fueron descargados desde:
- https://censo2024.ine.gob.cl/resultados/ 
- https://www.siet-chile.cl/descargables/

Y en particular, necesitas descargar los siguientes:
- https://censo2024.ine.gob.cl/wp-content/uploads/2025/12/diccionario_variables_censo2024.xlsx
- https://storage.googleapis.com/bktdescargascenso2024/viv_hog_per_censo2024.zip
- https://www.siet-chile.cl/wp-content/uploads/2025/12/GDB_SIET-Chile_04Dic2025.zip
