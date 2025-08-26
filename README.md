## Fullstack Python Playground

A collection of small, focused Python scripts and mini-projects for practicing scripting, data processing, basic web scraping, and simple image/PDF manipulation.

### Folder structure

```
fullstack-python/
├─ scraping-data-with-python/
│  └─ hacker-news-project/
│     └─ scrap.py                # Simple Hacker News scraper
└─ scripting-with-python/
   ├─ image processing/
   │  ├─ image.py                # Basic image operations (e.g., grayscale/blur)
   │  ├─ resize.py               # Image resize utility
   │  ├─ images/                 # Sample images
   │  └─ *.png, *.jpg            # Generated/processed outputs and samples
   ├─ JPGtoPNGconverter/
   │  ├─ jpg_to_png_convertor.py # Batch JPG→PNG converter
   │  └─ images/                 # Sample inputs
   └─ PDF processing/
      ├─ pdf.py                  # PDF merge/split utilities
      ├─ pdf_watermark.py        # Apply watermark to PDFs
      └─ *.pdf                   # Sample PDFs and outputs
```

### Prerequisites

- Python 3.9+
- Recommended: create and activate a virtual environment

```
python -m venv .venv
source .venv/bin/activate   # Windows (Git Bash): source .venv/Scripts/activate
pip install -U pip
```

### Suggested dependencies

Install libraries commonly used by the included scripts:

```
pip install pillow requests beautifulsoup4 PyPDF2
```

### How to run

- Image utilities (examples):
  - Grayscale/blur/resize: navigate to `scripting-with-python/image processing/` and run:
    ```
    python image.py
    python resize.py
    ```
  - JPG→PNG converter:
    ```
    cd "scripting-with-python/JPGtoPNGconverter"
    python jpg_to_png_convertor.py
    ```

- PDF tools:
  - Merge/split PDFs:
    ```
    cd "scripting-with-python/PDF processing"
    python pdf.py
    ```
  - Apply watermark:
    ```
    python pdf_watermark.py
    ```

- Web scraping (Hacker News example):
  ```
  cd "scraping-data-with-python/hacker-news-project"
  python scrap.py
  ```

Note: Some scripts expect specific input directories (e.g., `images/`) and will write outputs alongside source files.

### Contributing

Small improvements and additional mini-projects are welcome. Keep scripts self-contained, documented at the top of the file, and place input samples under a subfolder (e.g., `images/` or `samples/`).

### License

This project is licensed under the MIT License. See `LICENSE` for details.


