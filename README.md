# FLIK Extension Specification

- **Title:** FLIK
- **Identifier:** <https://fiboa.github.io/flik-extension/v0.1.0/schema.yaml>
- **Property Name Prefix:** none
- **Extension Maturity Classification:** Proposal
- **Owner**: @m-mohr

This document explains the FLIK Extension to the
[Field Boundaries for Agriculture (fiboa) Specification](https://github.com/fiboa/specification).

The area identifier (FLIK) is a unique identifier key to clearly identify field blocks and similar entities,
which is mostly used in Germany but can be used internationally.

- Examples:
  - [GeoJSON](examples/geojson/)
  - [GeoParquet](examples/geoparquet/)
- [Schema](schema/schema.yaml)
- [Changelog](./CHANGELOG.md)

## Properties

The properties in the table below can be used in these parts of fiboa documents:

- [ ] Collection
- [x] Feature Properties

| Property Name   | Type   | Description |
| --------------- | ------ | ----------- |
| flik            | string | **REQUIRED**. The area identifier (FLIK code) is a 16-character string. |

The FLIK identifier consists of:
- 2-letter country code (e.g. `DE` for Germany)
- 2-letter state code (e.g. `BB` for Branbenburg)
- 2-letter element type which is assigned on the state level (e.g. `LI`, `LE`, `NF` or `PS`)
- 10 character identifier which is assigned on the state level (e.g. `051B3A5678`)

So an example FLIK code could be: `DEBBLI0260100301`

More information can be found in German language at:
- <https://profilglossar.data-experts.de/mediawiki/index.php/Fl%C3%A4chenidentifikator>
- <https://www.amic.de/hilfe/_flik.htm>
- Search by FLIK in Germany: <https://flik-suche.de/>

## Contributing

See the [contributing guideline](CONTRIBUTING.md) for more details.
