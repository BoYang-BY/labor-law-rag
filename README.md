# Labor Law RAG Question Answering System

以《勞動基準法 Q&A 百問百答》為知識來源，建立 RAG（Retrieval-Augmented Generation）問答系統，
透過向量檢索與 Reranker 找出與使用者問題相關的文件內容，再交由 LLM 生成回答。

## Tech Stack
- Python
- LangGraph
- Chroma
- OpenAI API
- BGE Reranker
- Gradio

## Project Workflow
PDF Document
→ Text Chunking
→ Vector Database
→ Top-K Retrieval
→ BGE Reranking
→ LLM Generation
→ Answer

## Key Features
- 將勞動法規 Q&A 文件建立為向量知識庫
- 使用 Chroma 進行語意檢索
- 加入 BGE Reranker 重新排序檢索結果
- 以測試問題與 Ground Truth Pages 評估檢索效果
- 使用 Gradio 建立互動式問答介面

## Knowledge Source
《勞動基準法 Q&A 百問百答第二版》

## Notebook
完整的文件處理、檢索、Reranking、回答生成與測試流程，
請參考本 Repository 中的 Jupyter Notebook。

## Note
API keys and other sensitive credentials are not included in this repository.
