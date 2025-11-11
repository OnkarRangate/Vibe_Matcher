# 🎧 Vibe Matcher — Fashion Recommendation Prototype  

## 🧠 Overview  
**Vibe Matcher** is a mini fashion recommendation system prototype that matches user *“vibes”* to fashion products using text embeddings and cosine similarity.  
The system takes a **vibe query** (like *“energetic urban chic”*) and returns the **top-3 most relevant products** based on semantic similarity between the query and product descriptions.  

Originally designed to use OpenAI’s `text-embedding-ada-002` model, the project was adapted to run **fully locally using Hugging Face embeddings** to ensure accessibility and cost-free experimentation.  

---

## 🗂️ Features  
- 🧺 **Sample Fashion Dataset:** 5–10 mock fashion items with names, descriptions, and vibe tags (e.g., *boho*, *cozy*, *urban*).  
- 🧬 **Embeddings Generation:** Uses Hugging Face’s `sentence-transformers/all-MiniLM-L6-v2` model for local embedding generation.  
- 🔍 **Similarity Search:** Computes **cosine similarity** using `scikit-learn` to rank items by vibe relevance.  
- ⚙️ **Evaluation & Logging:** Tests multiple vibe queries, logs similarity scores, and measures query latency using `timeit`.  
- 💡 **Edge Handling:** Provides fallback behavior for unmatched vibes or low similarity scores.  

---

## 🧩 Tech Stack  
| Component | Library / Tool |
|------------|----------------|
| Language | Python 🐍 |
| Data Handling | Pandas |
| Embeddings | Sentence-Transformers (Hugging Face) |
| Similarity Search | scikit-learn |
| Visualization | Matplotlib |

---

## 🚀 Workflow  
1. **Data Preparation:** Create a small dataset of fashion products with vibe-based tags.  
2. **Embedding:** Convert product descriptions and user queries into vector embeddings.  
3. **Similarity Matching:** Compute cosine similarity between query and products.  
4. **Ranking:** Display top-3 products with their similarity scores.  
5. **Testing:** Run multiple vibe queries, log similarity thresholds (`>0.7` = good).  
6. **Reflection:** Summarize insights, edge cases, and potential improvements.  

---

## 🧭 Possible Improvements  
- 🔹 Integrate **Pinecone** or **FAISS** for scalable vector search.  
- 🔹 Add a **frontend UI** (e.g., Streamlit or Gradio) for interactive vibe matching.  
- 🔹 Expand dataset and explore **multimodal embeddings** (text + image).  
- 🔹 Use **OpenAI embeddings** for higher-quality semantic matches once API access is available.  

---

## 🗒️ Note  
> This project was built as a prototype to demonstrate the core logic of a vibe-based recommendation engine.  
> Due to API cost limitations, embeddings were generated locally using Hugging Face models instead of OpenAI’s `text-embedding-ada-002`.

---

## 💻 Author  
**Omkar Rangate**  
*AI & Data Science Engineer | Passionate about NLP, Recommender Systems, and Fintech AI*  
📧 [onkarrangate@gmail.com] | 🌐 [(https://www.linkedin.com/in/onkar-rangate-727492260/)]

