# trafico_bici_VLC — Intensidad de tráfico ciclista por puntos de medida (València)

Archivo histórico de la **intensidad de tráfico de bicicletas** medida en los
puntos de aforo ciclista de València, obtenida de la API de gobierno abierto
municipal (hoy descatalogada).

## Origen

- **Fuente:** Ayuntamiento de València — API de gobierno abierto
  *apigobiernoabiertortod.valencia.es/apirtod* (recurso
  `intensidad_espiras.csv` correspondiente a puntos de medida ciclista).
- API descatalogada; este repositorio es la copia de respaldo del histórico.

## Periodo

- **409 días** entre **03-04-2019** y **22-10-2024**.

## Estructura del repositorio

- Un fichero ZIP por día: `DD-MM-YYYY.zip`, con los CSV capturados ese día.
- Un commit ("new day") por día, fechado con la fecha real del dato.

## Formato y campos

Ficheros **CSV** con separador `;`. Columnas:

| Columna        | Significado                                              |
|----------------|---------------------------------------------------------|
| `modified`     | Marca de tiempo de la última actualización del dato.    |
| `angulo`       | Orientación / ángulo del punto de medida.               |
| `intensidad`   | Intensidad de tráfico ciclista medida.                  |
| `punto_medida` | Identificador del punto de medida.                      |
| `ycoord`       | Coordenada en **UTM EPSG:25830**.                       |
| `xcoord`       | Coordenada en **UTM EPSG:25830**.                       |
| `uri`          | URI del recurso en el portal de datos.                  |
