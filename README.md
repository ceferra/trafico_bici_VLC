# trafico_bici_VLC — Bicycle traffic intensity by measurement point (València)

Historical archive of **bicycle traffic intensity** measured at València's
cycling count points, obtained from the municipal open-government API (now
decommissioned).

## Source

- **Publisher:** València City Council — open-government API
  *apigobiernoabiertortod.valencia.es/apirtod* (resource
  `intensidad_espiras.csv` for the cycling measurement points).
- Decommissioned API; this repository is the backup copy of the history.

## Period

- **409 days** between **2019-04-03** and **2024-10-22**.

## Repository layout

- One ZIP file per day: `DD-MM-YYYY.zip`, holding the CSVs captured that day.
- One commit ("new day") per day, dated with the real date of the data.

## Format and fields

**CSV** files with `;` separator. Columns:

| Column         | Meaning                                                 |
|----------------|---------------------------------------------------------|
| `modified`     | Timestamp of the last update of the datum.              |
| `angulo`       | Measurement-point orientation / angle.                  |
| `intensidad`   | Measured bicycle traffic intensity.                     |
| `punto_medida` | Measurement-point identifier.                           |
| `ycoord`       | Coordinate in **UTM EPSG:25830**.                       |
| `xcoord`       | Coordinate in **UTM EPSG:25830**.                       |
| `uri`          | Resource URI on the data portal.                        |
