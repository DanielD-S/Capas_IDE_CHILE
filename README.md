# Catastro Minero Chile — Datos Abiertos

Base de datos de propiedad minera vigente de Chile con geometría poligonal completa.

**Fuente:** SERNAGEOMIN — Servicio Nacional de Geología y Minería  
**Vigencia:** Abril 2026 (actualización mensual vía Boletín Oficial de Minería)  
**Registros:** 195.072 propiedades mineras  
**Sistema de referencia:** WGS84 — EPSG:4326

## Descarga

👉 [Descargar datos — Release v1.0-abril2026](https://github.com/DanielD-S/catastro_minero/releases/tag/v1.0-abril2026)

## Contenido

| Archivo | Tipo | Registros | Cobertura temporal |
|---|---|---|---|
| `concesion.geojson` / `.csv` | Concesiones de exploración | 40.158 | 2022–2026 |
| `manifestacion.geojson` / `.csv` | Manifestaciones mineras | 64.131 | 1903–2026 |
| `mensura.geojson` / `.csv` | Mensuras | 85.977 | 1900–2026 |
| `pedimento.geojson` / `.csv` | Pedimentos | 4.806 | 2024–2026 |

## Atributos

Cada registro incluye:

| Campo | Descripción |
|---|---|
| `id` | Identificador único |
| `nombre` | Nombre de la propiedad minera |
| `titular` | Titular actual |
| `rol` | Rol minero |
| `hectareas` | Superficie en hectáreas |
| `juzgado` | Juzgado de letras de minas |
| `f_sentenci` | Fecha de sentencia |
| `bol_senten` | Número de boletín de sentencia |
| `solicitud` | Fecha de solicitud |
| `_lat` / `_lon` | Coordenadas del centroide |

## Formatos

- **GeoJSON** — carga directa en QGIS, ArcGIS, Leaflet, Mapbox
- **CSV** — compatible con Excel, Python, R

## Cómo usar en QGIS

```
Capa → Agregar capa → Agregar capa vectorial → seleccionar .geojson
```

El sistema de referencia se detecta automáticamente (EPSG:4326).

## Cobertura temporal

Los datos corresponden al **catastro vigente** publicado por SERNAGEOMIN:

- **Manifestaciones y mensuras:** historia completa desde ~1980
- **Concesiones de exploración:** estado vigente (desde 2022)
- **Pedimentos:** estado vigente (desde 2024)

## Nota

Esta información es de carácter público conforme a la **Ley 20.285 sobre Acceso a la Información Pública**.

Los servicios web de SERNAGEOMIN se encuentran fuera de línea desde diciembre de 2025 tras un ataque de ransomware, sin fecha confirmada de restitución. Estos datos fueron procesados y se comparten para facilitar el acceso a información pública mientras se restablecen los servicios oficiales.

---

**Autor:** Daniel Díaz Santander  
**Última actualización:** Junio 2026
