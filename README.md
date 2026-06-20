# Tianguis CDMX 🛍️

**Nivel socioeconómico y distribución geográfica de los tianguis en la Ciudad de México (2023)**

Análisis de autocorrelación espacial entre el Índice de Rezago Social (CONEVAL) y la densidad de tianguis, a nivel de AGEB urbana, mediante el Índice de Moran (global y bivariado) e indicadores LISA.

Proyecto de Metodología de la Investigación — ESCOM-IPN · Grupo 5AM1.

---

### ▶️ Ver el mapa interactivo

## **https://alangja.github.io/tianguis-cdmx/**

Mapa de elaboración propia (solo Ciudad de México). Muestra los tianguis como puntos coloreados por día de operación, con filtros por día y por alcaldía, conteo en vivo y capas seleccionables por AGEB: Grado de Rezago Social, índice de rezago continuo, densidad de tianguis y LISA bivariado.

---

## Estructura del repositorio

```
tianguis-cdmx/
├── index.html      Mapa interactivo (lo publica GitHub Pages)
├── notebook/       Cuaderno con todo el análisis espacial
└── data/           Datos de entrada y resultados
```

**Archivos de `data/`**

| Archivo | Contenido |
|---|---|
| `tianguis_cdmx.csv` | Padrón de tianguis (SEDECO, 2023) |
| `GRS_AGEB_urbana_2020.xlsx` | Grado de Rezago Social por AGEB (CONEVAL, 2020) |
| `ageb_urbanas_cdmx.json` | Polígonos de AGEB urbanas (INEGI, 2020) |
| `resultados_ageb_tianguis.csv` | Resultados por AGEB (salida del notebook) |
| `resultados_ageb_tianguis.gpkg` | Capa geoespacial de resultados |

## Reproducir el análisis

```bash
pip install geopandas libpysal esda pandas numpy matplotlib openpyxl jupyter
jupyter notebook notebook/tianguis_nse_cdmx.ipynb
```

## Fuentes de datos

| Fuente | Dato | Enlace |
|---|---|---|
| SEDECO | Padrón de tianguis 2023 (Datos Abiertos CDMX / ADIP) | https://datos.cdmx.gob.mx/ |
| INEGI | Marco Geoestadístico 2020 — AGEB urbanas | https://www.inegi.org.mx/temas/mg/ |
| CONEVAL | Grado de Rezago Social por AGEB (2020) | https://www.coneval.org.mx/ |

## Integrantes

Contreras Trejo David Ruben · García Juanillo Alan · Nieves Bartolo Marco Antonio · Reyes Leon Angel Eduardo · Reynoso Ortega Valeria
