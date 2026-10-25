# AppotecariaDB

Medicines database used by the [Appotecaria](https://github.com/ermengol/Appotecaria)
study app: Spanish medicines and active ingredients with study sections from
their technical datasheets. The app downloads it from the releases of this
repository.

**Educational use only.** This is not a medical device and it gives no dosing
advice for any patient. Highlights and tags in the data are generated
automatically and do not replace the official technical datasheet (ficha
técnica) or package leaflet (prospecto). Always check the source.

## Contents

Each release will publish:

- `medicines.sqlite.gz`: the SQLite database read by the app.
- `manifest.json`: version, schema version, minimum app version, SHA-256,
  size and the date of each source, signed so the app only accepts
  databases published here.

## Sources

The data comes from public sector information of the Spanish administration,
reused under Ley 37/2007 on the reuse of public sector information. The
meaning of the source data has not been altered; each release states the date
of each source.

| Source | Publisher | Data |
| --- | --- | --- |
| [CIMA REST API](https://cima.aemps.es/cima/rest/) | Agencia Española de Medicamentos y Productos Sanitarios (AEMPS) | Technical datasheet sections, change log |
| [Nomenclátor de prescripción](https://listadomedicamentos.aemps.gob.es/prescripcion.zip) | AEMPS | Medicines, active ingredients, ATC, dosage forms, routes |
| [Nomenclátor de facturación](https://www.sanidad.gob.es/profesionales/nomenclator.do) | Ministerio de Sanidad | Reimbursement, prices, patient contribution |

Source: AEMPS and Ministerio de Sanidad. The source data remains under the
reuse conditions of its publishers.

## License

The structure of the database, the tags and the other additions made by this
project are licensed under
[Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0). The
source data listed above is not relicensed: it stays under the reuse
conditions of the AEMPS and the Ministerio de Sanidad, which also require
citing the source and its update date.
