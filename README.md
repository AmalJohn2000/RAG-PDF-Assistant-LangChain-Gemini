# RAG-PDF-Assistant-LangChain-Gemini
An AI-powered RAG system that answers questions from any PDF using LangChain and Google Gemini

## 🎯 What it does

- Upload any PDF document
- Ask questions in text
- AI answers ONLY from your document
- Says "I don't know" if answer is not in the document
- Zero hallucinations!

---

## 🏗️ Architecture

Your PDF
↓ PyPDFLoader (reads PDF)
↓ RecursiveCharacterTextSplitter (splits into 500-char chunks)
↓ GoogleGenerativeAIEmbeddings (converts to vectors)
↓ ChromaDB (stores vectors)
User Question (text)
↓ Retriever (finds top 3 relevant chunks)
↓ ChatPromptTemplate (combines context + question)
↓ Gemini 2.0 Flash (generates answer)
↓ StrOutputParser (cleans output)
↓ Gradio Chat UI → Final Answer ✅

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Programming language |
| LangChain | AI pipeline framework |
| Google Gemini API | LLM brain (gemini-2.0-flash) |
| Gemini Embeddings | Text to vectors (gemini-embedding-001) |
| ChromaDB | Vector database |
| PyPDF | PDF loader |
| Gradio | Chat UI with voice input |
| Google Colab | Development environment |

---
## 💡 Key concepts used

- **RAG** — Retrieval Augmented Generation
- **Vector Embeddings** — converting text to numbers
- **Similarity Search** — finding relevant chunks
- **Teacher Forcing** — training technique
- **Encoder-Decoder** — LLM architecture
- **Transformer** — base architecture of all modern LLMs

---

---

## 🔮 Future improvements

- [ ] Multi-PDF support
- [ ] Voice Input
- [ ] Conversation memory
- [ ] Deploy on Hugging Face Spaces
- [ ] Support for Excel and Word documents
- [ ] Hindi language support

---

## 👤 Author

**Amal John Kallukkaran**
- LinkedIn: https://www.linkedin.com/in/amal-john-kallukaran/
- GitHub: https://github.com/AmalJohn2000

---

## ⭐ If you found this useful, please star this repository!
