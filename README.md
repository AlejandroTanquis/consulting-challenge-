# CineMetrics – Análisis de A Minecraft Movie (2025)

## Descripción del proyecto

Proyecto de análisis de datos desarrollado por CineMetrics, con el objetivo de estudiar la recepción de la película *A Minecraft Movie* (2025), comparando las opiniones y calificaciones de críticos especializados y usuarios.

El análisis busca identificar diferencias entre ambos grupos, conocer los principales aspectos mencionados en las reseñas y detectar posibles divergencias en la valoración de la película.

## Objetivo

Comparar la recepción crítica y del público para comprender qué aspectos de la película generan diferentes valoraciones y cuáles presentan coincidencias.

## Fuente de datos

- **Fuente:** Metacritic.
- **Película:** A Minecraft Movie (2025).
- **Total de registros:** 155 reseñas.
- **Críticos:** 40 reseñas.
- **Usuarios:** 115 reseñas.

Las reseñas fueron recopiladas manualmente.

## Metodología

El proyecto se desarrolló en las siguientes etapas:

1. **Obtención de datos:** recopilación de reseñas y calificaciones de críticos y usuarios.
2. **Limpieza:** revisión de valores nulos, duplicados y tipos de datos.
3. **Normalización:** conversión de las puntuaciones de usuarios a una escala de 0 a 100 para permitir su comparación con las de los críticos.
4. **Análisis exploratorio:** estadística descriptiva, distribuciones y comparación de puntuaciones.
5. **Análisis de comentarios:** identificación y agrupación de los principales temas de las reseñas.
6. **Visualización:** elaboración de gráficos para comunicar los resultados.
7. **Hallazgos:** identificación de diferencias y coincidencias entre críticos y usuarios.

## Principales hallazgos

### 1. Comparación general de puntuaciones

- **Promedio de críticos:** 49,75/100.
- **Promedio de usuarios:** 55,30/100.
- **Mediana de críticos:** 50 puntos.
- **Mediana de usuarios:** 60 puntos.
- **Dispersión:** las puntuaciones de los usuarios presentan una desviación estándar de 29,51, frente a 16,43 de los críticos.

Los usuarios presentan una puntuación promedio superior y una mayor dispersión en sus calificaciones, mientras que las puntuaciones de los críticos se encuentran más concentradas.

### 2. Diferencias en la valoración de los temas

- **Humor y entretenimiento:** los usuarios presentan una puntuación promedio de 70,67, frente a 53,25 de los críticos.
- **Guion e historia:** ambos grupos muestran puntuaciones relativamente bajas: 43,79 entre críticos y 38,89 entre usuarios.
- **Adaptación a Minecraft:** los usuarios presentan una puntuación promedio de 61, frente a 49,50 de los críticos.

### 3. Diferencias en los temas destacados

- **Guion e historia:** representa el 35% de las reseñas de críticos y el 15,65% de las reseñas de usuarios.
- **Adaptación y referencias a Minecraft:** representa el 20% de las reseñas de críticos y el 34,78% de las reseñas de usuarios.

Estos resultados muestran que críticos y usuarios no necesariamente destacan los mismos aspectos de la película.

## Conclusiones

Los resultados muestran diferencias en la manera en que críticos y usuarios valoran la película. Mientras los usuarios presentan una recepción más favorable del humor y de los elementos vinculados con Minecraft, los críticos dedican una mayor proporción de sus reseñas al guion y la historia.

## Limitaciones

- La muestra está compuesta por 155 reseñas y no representa necesariamente a todos los críticos y espectadores.
- Los temas principales fueron asignados mediante interpretación cualitativa.

## Estructura del repositorio

```text
CineMetrics/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── images/
│
├── presentation/
│
└── README.md
```

## Reproducción del análisis

Para reproducir el análisis:

1. Clonar el repositorio.
2. Instalar Python y las librerías utilizadas en el notebook.
3. Abrir el notebook de análisis.
4. Ejecutar las celdas en orden, utilizando los archivos de datos incluidos en el repositorio.