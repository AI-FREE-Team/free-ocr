
<div align="center">
  <div>
    <h1 align="center">FREE OCR</h1>
  </div>
	<p>A Python package to perform OCR for free.</p>

<a href="https://pypi.org/project/free-ocr/"><img src="https://img.shields.io/pypi/v/free-ocr" alt="Current version"></a> <a href="https://pypi.org/project/free-ocr/" target="_blank">![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)</a>

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
file_path = "./trader-joes-receipt.jpg"  # path to your image

markdown = ocr(file_path, api_key=api_key)
print(markdown)
```

---

## Original Resources

This package is based on the free Llama 3.2 endpoint from [Together AI](https://dub.sh/together-ai), which parses images and returns Markdown content.

 - Web Llama OCR demo: [LlamaOCR.com](https://llamaocr.com/)

 - llama-OCR Official Repo: [github.com/Nutlope/llama-ocr](https://github.com/Nutlope/llama-ocr)

