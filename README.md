# Economic Development vs. Sustainability
Author: Katlyn Goeujon-Mackness <br>

This project investigates the relationship between economic growth and environmental impact, focusing on CO₂ emissions, GDP, and population data across countries and years. Using structured, reproducible workflows, we clean, reconcile, and merge publicly available datasets to explore patterns of global development and sustainability.

## Key Metrics Analyzed

- Annual and cumulative CO₂ emissions
- GDP and GDP per capita
- CO₂ per capita and CO₂ intensity
- Population impact and country group classifications
- Emissions and economic bands (e.g., high/low emitters)

## Data Sources

- **CO₂ Emissions**: [Our World in Data](https://github.com/owid/co2-data)
- **GDP & Population**: [World Bank Open Data](https://data.worldbank.org/)
- **Region & Income Groups**: Custom metadata files (based on World Bank classifications)

## Highlights

- Cleaned raw emissions and GDP data with extensive error handling, ISO harmonization, and null filtering
- Constructed log-transformed variables for better outlier handling
- Categorized countries by emissions and economic group
- Merged and validated a unified dataset covering over 180 countries, from 1960 to 2022
- Created a reusable final dataset, suitable for visualization and policy analysis


## Project Structure

### Notebooks
```
notebooks-english/
├── 1a_Discovery_Structuring_GDP.ipynb              # Exploring GDP data structure and sources
├── 1b_Discovery_Structuring_Emissions.ipynb        # Exploring CO₂ emissions data
├── 2a_Data_Cleaning_GDP.ipynb                      # Cleaning and filtering GDP data
├── 2b_Data_Cleaning_Emissions.ipynb                # Cleaning and structuring emissions data
├── 3a_Joining_Datasets.ipynb                       # Merging emissions, GDP, population, and metadata
└── 4a_Presentation_GDP_Emissions.ipynb             # Visualizations and storytelling (to be published)
````

### Data 

````
data/
├── raw/                            # Original, unprocessed data files
│   ├── emissions/                  # Raw emissions datasets
│   │   ├── owid-co2-data_raw.csv
│   │   └── renewable_energy_raw.csv
│   ├── gdp/                        # Raw GDP datasets
│   │   └── gdp_per_capita_constant_USD_raw.csv
│   │   └── GDP-per-capita-percent-growth_raw.csv
│   │   └── Metadata_gdp_per_capita_constant_USD_raw.csv
│   │   └── Metadata_Indicator_gdp_per_capita_constant_USD_raw.csv
│   │   └── Metadata_Indicator_GDP-per-capita-percent-growth_raw.csv
│   │   └── data/raw/gdp/Metadata-GDP-per-capita-percent-growth_raw.csv
│   ├── population/                 # Raw population datasets
│   │   └── population-long-run-with-projections.csv
│   └── metadata/                   # Supporting metadata files
│       ├── country_region_classification.xlsx
│       └── income_groups.csv
├── in_process/                     # Intermediate or partially processed data
│   ├── data/in_process/0_dataset_descriptions.txt
│   ├── ...
├── processed/                      # Final, fully processed datasets
│   └── data_descriptions.txt
│   └── gdp_co2_by_country_final.csv

````

## Next Steps

- Integrate renewable energy metrics
- Explore machine learning-based emission forecasts

## Contributions  
If you'd like to contribute by improving the analysis, adding new visualizations, or correcting potential errors, you're very welcome. You can fork the repository and submit your pull requests. Every contribution will help enrich the project and encourage discussion around sustainable economic growth.

## License  
This project is distributed under the MIT License. For more details, see the LICENSE file.

## Get in Touch  
If you have questions, suggestions, or want to share your ideas about the project, feel free to reach out. I'm open to collaboration and feedback that enhances this analysis.

Email: macknessk@gmail.com  
LinkedIn: Katlyn Goeujon-Mackness
Kaggle: [Global GDP & CO₂ Emissions Dataset (1960–2022)](https://www.kaggle.com/datasets/mackness/global-gdp-and-co-emissions-dataset-19602022/data)


# Español

## Contribuciones
Si deseas contribuir a mejorar el análisis, añadir nuevas visualizaciones o corregir posibles errores, eres bienvenido a hacerlo. Para ello, puedes realizar un fork del repositorio y enviar tus pull requests. Toda contribución ayudará a enriquecer el proyecto y fomentar la discusión sobre el crecimiento económico sostenible.

## Licencia
Este proyecto se distribuye bajo la Licencia MIT. Para más información, consulta el archivo LICENSE.

## Ponte en Contacto
Si tienes preguntas, sugerencias o deseas compartir tus ideas sobre el proyecto, no dudes en ponerte en contacto conmigo. Estoy abierto a colaborar y a recibir comentarios que enriquezcan este análisis.

Correo Electrónico: macknessk@gmail.com
LinkedIn: Katlyn Goeujon-Mackness
