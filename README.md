# RFMIP2.0

Website for the [Radiative Forcing Model Intercomparison Project](https://rfmip.github.io) (RFMIP), part of CMIP7.

RFMIP2.0 is a coordinated set of fixed sea-surface-temperature experiments designed to diagnose effective radiative forcing (ERF) and separate it from the feedbacks that obscure it, across the CMIP7 model ensemble. The protocol is described in [Kramer et al. (2026), *Geoscientific Model Development*](https://doi.org/10.5194/gmd-19-4447-2026).

**Co-chairs:** Ryan Kramer (GFDL, NOAA) · Chris Smith (VUB & IIASA) · Tim Andrews (Met Office Hadley Centre & University of Leeds)

## Editing content

Adding a news item, a publication, or editing the About page? See [`CONTENT-GUIDE.md`](CONTENT-GUIDE.md) — everything there can be done from github.com, no Jekyll/Ruby/command-line knowledge needed.

## Local development

This is a [Jekyll](https://jekyllrb.com/) site, built on the [al-folio](https://github.com/alshedivat/al-folio) theme. Run it locally with Docker:

```bash
docker compose up
```

Then visit http://localhost:8080 — most content edits hot-reload automatically.

## License

Site code is built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme (MIT-licensed, see [`LICENSE`](LICENSE)).
