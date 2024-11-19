
<div align="center">
  <div>
    <h1 align="center">free-ocr</h1>
  </div>
	<p>A Python library to perform llama-OCR for free with Llama.</p>

<a href="https://pypi.org/project/free-ocr/"><img src="https://img.shields.io/pypi/v/free-ocr" alt="Current version"></a>

</div>

---

## Installation

```bash
pip install free-ocr
```

---

## Usage

```python
from free_ocr import ocr

api_key = "your-together-ai-api-key"  # Together AI API key
file_path = "./trader-joes-receipt.jpg"  # path to your image (soon PDF!)

markdown = ocr(file_path, api_key=api_key)
print(markdown)
```

---

## Hosted Demo

You can use the original Llama OCR demo at [LlamaOCR.com](https://llamaocr.com/) to try out similar functionality online!

---

## How it works

This library is based on the free Llama 3.2 endpoint from [Together AI](https://dub.sh/together-ai), which parses images and returns Markdown content. Paid endpoints for Llama 3.2 11B and Llama 3.2 90B are also available for faster performance and higher rate limits.

You can control this with the `model` parameter, which defaults to `Llama-3.2-90B-Vision`. Alternatively, you can use `free` or `Llama-3.2-11B-Vision`.

---

## Roadmap

- [x] Add support for local image OCR
- [x] Add support for remote image OCR
- [ ] Add support for single-page PDFs
- [ ] Add support for multi-page PDFs OCR (convert PDF pages to images)
- [ ] Add support for JSON output alongside Markdown

---

## Credit

This project is based on the original [llama-ocr](https://github.com/Nutlope/llama-ocr). Special thanks to the contributors of that library for the inspiration and foundational work.
