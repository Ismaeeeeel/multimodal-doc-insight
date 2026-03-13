# Multimodal Document Insight 👁️📄

An advanced framework for **Document Intelligence** that leverages Vision-Language Models (VLMs) and layout-aware processing to extract structured information from complex documents (invoices, forms, research papers).

## 🌟 Overview

Traditional OCR often fails to capture the spatial relationships and visual context of complex documents. This project uses a **Vision-first** approach to "read" documents as humans do, combining visual features with textual context.

## 🚀 Features

- **Visual Question Answering (VQA):** Query your documents naturally (e.g., "What is the total amount in this invoice?").
- **Layout Analysis:** Detects tables, headers, and key-value pairs using coordinate-aware embeddings.
- **Multimodal LLM Integration:** Supports models like CLIP, LayoutLMv3, and GPT-4o-mini for visual reasoning.
- **Table Extraction:** Specialized logic for high-fidelity table-to-JSON conversion.

## 🛠️ Tech Stack

- **Models:** LayoutLM, Donut, CLIP.
- **Libraries:** Transformers, Pillow, PyMuPDF (fitz), OpenCV.
- **Data:** Support for PDF, PNG, JPEG, and TIFF.

## 📦 Installation

```bash
pip install -r requirements.txt
python processor.py --image invoice.png --query "Summarize the line items"
```