#Land Use and Land Cover (LULC) Classification with Machine Learning
# Classifica_de_Uso_e_Cobertura_do_Solo_Sentinel-2_GEE_ML

Project Overview

This project demonstrates a complete end-to-end workflow for Land Use and Land Cover (LULC) classification using remote sensing data, Google Earth Engine (GEE), Python, and Machine Learning in Google Colab.

The main objective is to build a reproducible, automated, and professional pipeline suitable for a geospatial portfolio, targeting positions such as Geoprocessing Analyst / GIS Analyst / Remote Sensing Analyst.

The workflow integrates cloud-based data acquisition (GEE) with local machine learning processing (Colab), following best practices in geospatial data science.


Data Source

Satellite: Sentinel-2 MSI

Spatial Resolution: 10 m

Platform: Google Earth Engine

Bands used:

B2 (Blue)

B3 (Green)

B4 (Red)

B8 (Near Infrared)


Methodology

1 - Image Acquisition (Google Earth Engine)

Selection of AOI

Cloud masking

Image compositing

Export of spectral bands and labeled samples

2 - Data Preparation (Google Colab)

Import of raster data

Feature matrix construction

Label encoding

Train-test split (train_test_split(X, y, test_size=0.3, random_state=42))

3 - Machine Learning Model

Algorithm: Random Forest Classifier

Justification:

Robust to noise

Handles nonlinear relationships

Widely used in remote sensing applications

4 - Model Evaluation

Confusion Matrix

Overall Accuracy

Class-wise performance

5 - Image Classification

Pixel-wise prediction

Generation of classified raster

GeoTIFF export


Repository Structures

lulc-ml-remote-sensing/

├── gee/

└── gee_export.js # Google Earth Engine script

├── notebooks/

 └── lulc_classification.ipynb

├── data/

├── raw/ # Exported spectral bands

└── samples/ # Training samples

├── results/

├── maps/ # Classified GeoTIFFs

 └── metrics/ # Accuracy reports

├── figures/

└── lulc_map_cartographic.png

├── requirements.txt
└── README.md


Technologies Used

Google Earth Engine (JavaScript API)

Python

Google Colab

Scikit-learn

Rasterio

NumPy

Matplotlib


Why This Project Matters

This project demonstrates:

Integration between cloud and local processing

Applied machine learning for geospatial analysis

Cartographic quality output

Reproducibility and clean repository structure


🇧🇷 Resumo em Português

Este projeto apresenta um fluxo completo de classificação de Uso e Cobertura do Solo (LULC) utilizando dados de sensoriamento remoto, Google Earth Engine, Python e Machine Learning em ambiente Google Colab.

O objetivo principal é demonstrar a integração entre aquisição de dados em nuvem (GEE), processamento local, treinamento de modelos de aprendizado de máquina e geração de produtos cartográficos com qualidade profissional.

O projeto foi desenvolvido com foco em portfólio técnico, seguindo boas práticas de organização de repositório, reprodutibilidade e comunicação de resultados, sendo especialmente voltado para vagas de Analista de Geoprocessamento, Analista SIG e Analista de Sensoriamento Remoto.

São abordadas etapas como:

Seleção e exportação de imagens no Google Earth Engine

Preparação dos dados espectrais

Treinamento de classificador Random Forest

Avaliação do modelo

Geração de mapa LULC com legenda, escala, seta de norte e coordenadas

Este repositório serve como projeto base, com grande potencial de expansão para análises multi-temporais, inclusão de índices espectrais e testes com outros algoritmos de classificação.

Etapa 1 – Configurar o Google Colab

Etapa 2 – Buscar imagem no Google Earth Engine

Etapa 3 – Seleção de bandas e índices espectrais

Etapa 4 – Exportar imagem para o Colab

Etapa 5 – Amostras de treinamento (Criar amostras manualmente no GEE)

Etapa 6 – Treinamento do modelo (Random Forest)

Etapa 7 – Classificação da imagem inteira

Etapa 8 – Visualização do resultado


