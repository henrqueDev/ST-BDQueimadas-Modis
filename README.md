# 🌍🔥 Clusterização Espaço-Temporal de Focos de Calor na Caatinga (PB)
- Projeto simples que aplica técnica de Machine Learning Não Supervisionado para agrupar focos de calor na Caatinga capturados pelo sensor MODIS do Satélite Aqua, no estado da PB.

## 📌 Visão Geral do Projeto
- A clusterização de focos de calor permite entender como os focos de calor capturados pelo sensor MODIS do satélite Aqua (Tarde) 
estão distribuídos geograficamente pelo tempo.
- Para a clusterização, o algoritmo utilizado foi o ST-DBSCAN (dados já processados em ./clustered_heat_points_1.parquet)
- O sensor MODIS tem resolução de 1km X 1km, sendo 1km o raio a ser definido para agrupar os focos de calor.
- O Satélite Aqua demora em torno de 1 hora e 39 minutos para completar uma volta no planeta Terra, sendo esse o tempo em segundos (5940s) para ser o epsilon temporal.
- Os outros 2 arquivos com epsilons distintos em 1.2km e 2km são apenas para exploração, sem rigor cientifico.

## 🛠️ Tecnologias e Algoritmos
As seguintes ferramentas e bibliotecas foram utilizadas no desenvolvimento:

- Python 3.12
- VS Code
- Jupyter Notebook
- Pandas & NumPy: Manipulação e tratamento dos dados geográficos.
- Scikit-Learn: Implementação de algoritmos de clusterização.
- Geopandas: Processamento de dados espaciais e criação dos buffers de raio.
- Folium: Visualização interativa dos clusters em mapas.

## 🚀 Rodar o projeto
``sh
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
pip install -r requirements.txt
``
