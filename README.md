# ChannelGPT

This project integrates **ChannelGPT** with **Open WebUI**, enabling natural language querying and analysis of YouTube channel content. 

To promote flexibility and reduce dependency on external services, the reliance on proprietary models like **OpenAI** has been replaced with free, open-source alternatives such as **vLLM** and **LM Studio**, allowing for independent, localized deployment. The **Google API Client Discovery** has been replaced by **yt-dlp**, a web scraping tool that extracts video data directly from YouTube’s web interface. For content analysis and embedding generation, models from **Hugging Face** are utilized, ensuring high-quality insights and accurate query handling.

<a href="#"><img alt="last-commit" src="https://img.shields.io/github/last-commit/NotYuSheng/ChannelGPT?color=red"></a>

> [!WARNING]  
> This project is incomplete and still a work in progress.

---

## Features

- **Natural Language Querying:** Enables users to query YouTube channels' content using plain language.
- **Open WebUI Integration:** Supports querying through a user-friendly web interface.
- **Free Alternatives:** Replaces proprietary APIs and models (OpenAI, Google) with open-source and free alternatives (vLLM, LM Studio, Hugging Face models).
- **yt-dlp for Web Scraping:** Uses **yt-dlp** to gather YouTube video data without relying on the Google API.
- **Flexible Embedding Models:** Uses and evaluates various models from Hugging Face for embedding channel content.
- **Dockerized Backend:** The backend **FastAPI server** has been containerized using Docker for easy deployment.

---

## Embedding Models Considered

| Model Name                                   | Description                                   | Status  |
|---------------------------------------------|---------------------------------------------|---------|
| `sentence-transformers/all-mpnet-base-v2`   | General-purpose embedding model from Sentence Transformers | ❌ Untested |
| `distiluse-base-multilingual-cased-v1`      | Multilingual embedding model from Sentence Transformers   | ❌ Untested |
| `BAAI/bge-large-en-v1.5`                    | Large English embedding model from BAAI                  | ❌ Untested |
| `BAAI/bge-base-en-v1.5`                     | Base English embedding model from BAAI                   | ✅ Tested   |

---

## Reference

This project is inspired by the original [ChannelGPT repository](https://github.com/a2ashraf/ChannelGPT) by [a2ashraf](https://github.com/a2ashraf). Significant modifications have been made, including:

- Replacing reliance on OpenAI models with **vLLM** or **LM Studio**.
- Replacing the Google API Client Discovery with **yt-dlp** for web scraping YouTube data.
- Using **Hugging Face models** for embedding channel content.
