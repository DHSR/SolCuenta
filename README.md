# SolCuenta

Herramienta web de acceso abierto, en español, para estimar el ángulo de inclinación óptimo, la producción de energía y la recuperación de la inversión de un sistema fotovoltaico residencial a partir del año meteorológico típico (TMY) de PVGIS del lugar, y no solo de su latitud.

**[Abrir SolCuenta en línea](https://dhsr.github.io/SolCuenta/solcuenta.html)**

## Qué hace

- Calcula, hora por hora durante un año típico, la irradiancia sobre un arreglo orientado al Sur con un modelo isótropo que incluye la radiación directa, la difusa del cielo y la reflejada por el suelo.
- Obtiene la inclinación fija óptima y los ángulos óptimos para cuatro ajustes estacionales a partir del clima del lugar.
- Evalúa cualquier inclinación definida por el usuario, como la pendiente de un techo ya construido, y reporta la energía mensual y anual, la energía por kWp, el periodo de recuperación simple y el CO₂ evitado.
- Incluye los datos de Ciudad Universitaria, Ciudad de México, y acepta el TMY de cualquier otro lugar descargado de PVGIS.

## Cómo usarla

SolCuenta es un solo archivo HTML sin dependencias externas: no requiere instalación ni registro y, una vez descargado, funciona sin conexión.

1. Ábrala con el enlace anterior, o descargue `solcuenta.html` y ábralo con cualquier navegador.
2. Para otro lugar, entre a [PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/es/), elija la ubicación en el mapa, abra la pestaña TMY, descargue el archivo CSV y cárguelo con el botón **Cargar un TMY de PVGIS**.
3. Capture los datos de los módulos, la inclinación, el costo de la instalación y el precio del kWh. El botón **Ayuda** abre el manual de uso, que puede guardarse como PDF.

Los resultados son un predimensionamiento: sirven para saber si vale la pena seguir, no para diseñar la instalación.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `solcuenta.html` | La herramienta completa, con los datos de Ciudad Universitaria incluidos. |
| `pvgis_tmy_cu.csv` | TMY de PVGIS 5.3 de Ciudad Universitaria (19.334° N, 99.198° O) usado en el artículo. |
| `LICENSE` | Licencia MIT. |

## Limitaciones

SolCuenta no considera sombras de obstáculos cercanos, representa las pérdidas por temperatura con un porcentaje fijo, supone módulos orientados al Sur y no incluye la degradación de los módulos, la inflación ni las alzas de tarifa. Los datos describen un año típico, no un año en particular.

## Cómo citar

Si usa SolCuenta en un trabajo académico, cite el artículo:

> Solís Recéndez, D. H., Castillo Valdez, O. F., López Serrano, I. Y., & Solís Recéndez, B. E. (en prensa). SolCuenta: herramienta de acceso abierto para estimar el ángulo óptimo y la recuperación de la inversión fotovoltaica residencial. *InterCiencias y Tecnología*.

El volumen, el número y las páginas se agregarán cuando el artículo se publique.

## Licencia y datos

El código se distribuye bajo la licencia MIT (ver `LICENSE`).

Los datos meteorológicos de `pvgis_tmy_cu.csv`, que también vienen incluidos dentro de `solcuenta.html`, provienen de PVGIS © European Union, 2001-2026. Su reutilización está autorizada siempre que se reconozca la fuente, y no quedan cubiertos por la licencia MIT. El factor de emisión de la red proviene de SEMARNAT (2026).

## Autores

- **Daniel H. Solís Recéndez** ([ORCID](https://orcid.org/0000-0002-2717-2983)), autor de correspondencia: dsolis@ipn.mx. Instituto Politécnico Nacional, Unidad Profesional Interdisciplinaria de Ingeniería Campus Zacatecas.
- **Oscar F. Castillo Valdez** ([ORCID](https://orcid.org/0009-0006-2923-6772)). Instituto Politécnico Nacional, Unidad Profesional Interdisciplinaria de Ingeniería Campus Zacatecas.
- **Irma Y. López Serrano** ([ORCID](https://orcid.org/0009-0004-4129-7645)). Instituto Politécnico Nacional, Unidad Profesional Interdisciplinaria de Ingeniería Campus Zacatecas.
- **Blanca E. Solís Recéndez** ([ORCID](https://orcid.org/0000-0003-3822-3579)). Universidad Autónoma de Zacatecas, Unidad Académica de Ingeniería Eléctrica.
