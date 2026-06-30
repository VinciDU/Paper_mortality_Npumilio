Descripción del Proyecto

Este repositorio contiene los datos procesados para el análisis de mortalidad de árboles, clustering y variables ambientales. Los archivos incluyen información de series temporales, datos de árboles muertos y vivos, y resultados de análisis de clusters.
📁 datos/
├── 📄 matriz_final.csv          # Serie temporal con variables climáticas y de mortalidad
├── 📄 cluster_data.csv          # Datos de árboles muertos con variables estructurales y cluster
└── 📄 DB_Vivos.csv        # Datos de árboles vivos con variables estructurales
1. matriz_final.csv
Serie temporal que combina variables climáticas, de crecimiento y mortalidad para el período 1959-2015 (aproximadamente).
Variable	Descripción	Unidades
GS	Año (Growing Season)	Años
Defoliacion	Porcentaje de defoliación	%
ATGS	Anomalía de temperatura en la temporada de crecimiento	°C
ARBDEF	Biomasa aérea defoliada	g/m²
NMuertos	Número de árboles muertos	Individuos
PDSIGS	PDSI en temporada de crecimiento	Adimensional
P_ARBDEF	Proporción de biomasa aérea defoliada	%
ATPRIM	Anomalía de temperatura en primavera	°C
TMAXV	Temperatura máxima en verano	°C
mort_1	Frecuencia de mortalidad (categoría 1)	Conteo
mort_2	Frecuencia de mortalidad (categoría 2)	Conteo
mort_3	Frecuencia de mortalidad (categoría 3)	Conteo

2. cluster_data.csv

Datos de árboles muertos con asignación de clusters basada en variables estructurales.
Variable	Descripción	Unidades
Elevacion	Altitud sitio	metros
DAP	Diámetro a la altura del pecho	cm
Competencia	Índice de competencia con árboles vecinos	Adimensional
Densidad	Densidad de árboles en el área	árboles/ha
Cluster	Asignación de cluster (k-means o similar)	Categórico (1-3)

3. DB_Vivos.csv

Datos de árboles vivos con variables estructurales similares a los datos de muertos.
Variable	Descripción	Unidades
DAP_cm	Diámetro a la altura del pecho	cm
Competencia_Total	Índice de competencia total	Adimensional
Elevation	Altitud del árbol	metros
Densidad	Densidad de árboles en el área	árboles/ha

