# Satisfacción y Clasificación de Clientes de una Aerolínea

Proyecto académico grupal del Grado en Ciencia de Datos — UPV (2024-2025).

## Descripción
Estudio estadístico de los perfiles y nivel de satisfacción de 1.917 pasajeros de
una aerolínea, con 21 variables. El objetivo es identificar segmentos de clientes
y predecir su satisfacción mediante métodos no supervisados y supervisados.

## Tecnologías
- **Lenguaje:** R / RStudio
- **Librerías:** FactoMineR, cluster, caret, ropls, mice
- **Técnicas:** PCA (T²-Hotelling, SCR), K-Means, Clustering Jerárquico,
  K-Medoides, PLS-DA, LDA, QDA, Regresión Logística, Curvas ROC,
  ANOVA, Test de Tukey, Chi-cuadrado

## Dataset
Dataset de clientes de una aerolínea con 1.917 pasajeros y 21 variables:
datos demográficos (edad, género, tipo de cliente) y valoraciones de 14
aspectos del servicio en escala 0-5 (Wifi, confort, comida, entretenimiento,
limpieza, etc.).

## Resultados clave
- PCA con 5 componentes que explican el 72% de la varianza, agrupando
  variables en: confort físico, calidad del servicio de tripulación,
  experiencia previa al embarque y organización de la aerolínea
- K-Means (k=4) obtuvo el mejor resultado de clustering (silhouette = 0.16),
  identificando segmentos desde clientes insatisfechos digitalmente hasta
  altamente satisfechos
- La edad mostró relación significativa con los clusters (ANOVA p < 0.05);
  los retrasos y la distancia no
- LDA seleccionado como modelo final (AUC = 0.858, accuracy = 89.1%,
  sensibilidad = 96.8%) tras comparar LDA, QDA y regresión logística
- Variables más determinantes: fidelidad del cliente y calidad del Wifi;
  el confort del asiento y la comida aportaron poca discriminación

## Autores
- Carla Jimenez Argudo
- Michele Romero Calero
- Marta Martínez Martínez
- Fernanda De Paula Gonçalves
- Isaac Gimeno
