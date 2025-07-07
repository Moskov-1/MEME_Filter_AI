# 🧠 Meme Filter AI

A lightweight AI-powered meme filtering tool that retrieves and analyzes memes using a combination of image and text features. It aims to support text-based meme retrieval (e.g., search by keywords like "crying girl") to find the most relevant memes from a dataset.

---

## 📌 Overview

This notebook:

- Downloads memes from the [Imgflip API](https://api.imgflip.com/get_memes).
- Extracts and processes text (if present) from memes.
- Embeds meme content using CLIP (Contrastive Language–Image Pre-training) from OpenAI.
- Supports search via natural language queries (e.g., `"spongebob meme"` or `"crying baby"`).
- Evaluates relevance by comparing CLIP text/image embeddings.

> ⚠️ Current limitation: The Imgflip API mostly provides memes **without overlaid text**, which reduces performance. To get the best results, use memes **with visible text**.

---

## ⚙️ Features

- ✅ Meme scraping with `requests`
- ✅ CLIP model usage for vision-language understanding
- ✅ Cosine similarity-based ranking
- ✅ Basic search functionality to find memes by text
- ✅ Colab-ready (includes folder creation, saving assets, etc.)

---

## 🚀 Usage

1. **Download the Notebook**
   - Clone this repo or download `memes.ipynb`.

2. **Run in Google Colab**
   - Upload the notebook to [Google Colab](https://colab.research.google.com).
   - All meme images will be saved to `content/memes`.

3. **Run all cells**
   - It will:
     - Fetch memes from the web
     - Extract features via CLIP
     - Allow you to search using keywords

---

## 🔍 Sample Search Queries

Try searches like:

- `"crying girl"`
- `"angry cat"`
- `"SpongeBob"`
- `"funny office"`

> The AI model *really* likes SpongeBob memes. 😄

---

## 🧪 Future Work

- Improve OCR to extract overlaid text from image.
- Support additional meme sources (e.g., Reddit).
- Deploy a minimal web interface.

---

## 📁 Folder Structure

