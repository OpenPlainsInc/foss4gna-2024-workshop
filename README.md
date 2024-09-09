# foss4gna-2024-workshop

Materials for FOSS4GNA workshop - Developing Web Applications with GRASS GIS

## 1. Install Docker

## 2. Run Docker Compose

```bash 
docker compose up
```

## 3. Actinia

The actinia service will run by default at ``http://localhost:8088/``

```bash
curl -X GET "http://localhost:8088/api/v3/version" -H  "accept: application/json"
```

## Install sample data

```bash
curl -SL https://grass.osgeo.org/sampledata/north_carolina/nc_spm_08_grass7.zip > nc_spm_08_grass7.zip
unzip -qq nc_spm_08_grass7.zip
mv nc_spm_08_grass7 actinia-core-data/grassdb
rm nc_spm_08_grass7.zip
```
