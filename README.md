# data-pipeline-diagrams

Architecture diagrams, written as code for [Eraser](https://www.eraser.io), for a three-part data pipeline: scraping, processing and validation, then storage and search.

## Status

Documentation only. There is no runnable code. The files have no extension and contain Eraser diagram-as-code text.

## Contents

| File | Part | What it shows |
|------|------|---------------|
| `Web Scraping Architecture` | 1 | Python, BeautifulSoup4 and Requests scraping, a proxy list and retry path (Smartproxy), a ThredUp source, output to a local CSV file |
| `Data Processing and Validation Workflow` | 2 | Read JSON, clean (Pandas, NumPy, regular expressions), filter valid data, quality check, store as CSV |
| `ETL Pipeline` | 3 | Transform the CSV, then index with Algolia, store in Google Cloud Firestore, deploy on Cloud Run and Kubernetes, integrate with a Flutter app |

## Structure

```
Web Scraping Architecture
Data Processing and Validation Workflow
ETL Pipeline
```

## How to view

1. Open Eraser and create a new diagram-as-code file.
2. Paste the contents of one of the files.
3. The diagram renders on the canvas and can be exported as an image.

## License

MIT
