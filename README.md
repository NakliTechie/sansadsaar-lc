# sansadsaar-lc

Archive of PDF reports from the **Law Commission of India** (<https://lawcommissionofindia.nic.in/>), the companion to the metadata + extracted text held in [parliamentwatch-data](https://github.com/NakliTechie/parliamentwatch-data) under `docs/lc/`.

Auto-populated by parliamentwatch-data's scrape and OCR workflows whenever a new Law Commission report PDF is fetched.

## Why

A durability hedge. The upstream site runs on WordPress / S3WaaS with a track record of URL rotations and occasional content loss across the Government of India CMS estate. If the source ever goes offline, every PDF we've fetched is still here.

## Layout

```
pdfs/<report_number>.pdf       — the PDFs
index.json                     — manifest (sha256, size, archived_at, source_url per report)
```

## Family

- [SansadSaar](https://github.com/NakliTechie/SansadSaar) — the app
- [parliamentwatch-data](https://github.com/NakliTechie/parliamentwatch-data) — LC metadata + extracted text
- [sansadsaar-proceedings-data](https://github.com/NakliTechie/sansadsaar-proceedings-data) — Debates, Questions
- [sansadsaar-gazettes](https://github.com/NakliTechie/sansadsaar-gazettes) — Central Gazette
