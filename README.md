# 📊 Consulting Challenge — Data Analytics Lab: *A Minecraft Movie* (2025)

## 1. Descripción del Proyecto
Consultoría de datos orientada a evaluar el desempeño financiero y la distribución geográfica internacional de *A Minecraft Movie* (2025), comparándola frente a otras adaptaciones de videojuegos y producciones familiares del mismo año.

## 2. Objetivo de la Consultoría (CineMetrics)
Determinar qué factores comerciales explican el rendimiento en taquilla de *A Minecraft Movie* y traducir esos hallazgos en criterios concretos de inversión, presupuesto y estrategia de lanzamiento internacional para futuros proyectos cinematográficos basados en propiedades intelectuales (IPs).

## 3. Fuentes de Datos
Se consolidaron registros provenientes de fuentes públicas auditadas:
* **Box Office Mojo:** Ranking de taquilla global 2025 y desglose por territorios internacionales (`A_minecraft_movie_taquillas.csv`).
* **The Numbers:** Presupuestos de producción y recaudación mundial para el cálculo de retorno de inversión (`Comparacion_peliculas_2025.csv`).

## 4. Metodología Utilizada
1. **Extracción y Carga:** Estructuración de datasets abiertos en formatos CSV en `data/raw/`.
2. **Limpieza y Validación:** Normalización de variables monetarias a formato numérico (`float`), eliminación de filas vacías y corrección de traducciones erróneas en nombres de países (`Porcelana` → China, `Pavo` → Turquía) para el almacenamiento limpio en `data/processed/`.
3. **Análisis Exploratorio (EDA) Comercial:** Cálculo de multiplicadores de ROI ($\text{Recaudación Mundial} / \text{Presupuesto}$), análisis de participación por mercado geográfico y detección de valores atípicos (*outliers* como *Ne Zha 2*).
4. **Visualización:** Generación de gráficos ejecutivos en Python (`matplotlib` / `seaborn`) guardados en `images/`.

## 5. Principales Hallazgos Comerciales
* **Eficiencia de Capital (ROI de 6,41x):** *A Minecraft Movie* recaudó **$961,2M** sobre un presupuesto de producción de **$150M**. *Explicación alternativa descartada:* El éxito financiero no se explica por un presupuesto desmedido ni por estacionalidad de temporada alta; producciones familiares con idéntico costo ($150M) como *Elio* apenas alcanzaron un multiplicador de **1,03x**.
* **Comportamiento en Mercados Internacionales:** El **55,9%** de la taquilla total ($537,1M) provino de mercados fuera de EE. UU., liderados por el Reino Unido ($76,2M), Australia ($39,8M) y Alemania ($39,2M). Asimismo, se identificaron distintas velocidades de retención: mientras mercados como China concentraron un porcentaje elevado de su recaudación inicial en el fin de semana de estreno, territorios como el Reino Unido y Japón mostraron un mantenimiento de cartelera mucho más sostenido en el tiempo.
