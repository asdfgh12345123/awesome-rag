# Awesome RAG [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Best practices, tools, and frameworks for Retrieval-Augmented Generation.

## Frameworks
| Name | Stars | Description |
|------|-------|-------------|
| [LlamaIndex](https://github.com/run-llama/llama_index) | 30k+ | Data framework for LLM apps |
| [Haystack](https://github.com/deepset-ai/haystack) | 15k+ | End-to-end NLP framework |
| [LangChain](https://github.com/langchain-ai/langchain) | 90k+ | Build context-aware LLM apps |
| [RAGFlow](https://github.com/infiniflow/ragflow) | 20k+ | Open-source RAG engine |

## Vector Databases
| Name | Type | Description |
|------|------|-------------|
| [Weaviate](https://github.com/weaviate/weaviate) | Open-source | Vector search engine |
| [Milvus](https://github.com/milvus-io/milvus) | Open-source | High-performance vector DB |
| [Chroma](https://github.com/chroma-core/chroma) | Open-source | AI-native embedding DB |
| [Qdrant](https://github.com/qdrant/qdrant) | Open-source | High-performance vector search |
| [Pinecone](https://www.pinecone.io/) | Managed | Serverless vector database |
| [pgvector](https://github.com/pgvector/pgvector) | Extension | Vector similarity for PostgreSQL |

## Chunking Strategies
- **Fixed-size**: Simple, fast, good baseline
- **Recursive character**: LangChain default, respects structure
- **Semantic**: Embedding-based, highest quality
- **Document structure-aware**: Uses headings/sections

## Best Practices
1. Start with simple retrieval, optimize later
2. Use hybrid search (vector + keyword) for best results
3. Implement re-ranking for quality
4. Monitor retrieval quality metrics
5. Cache frequent queries

## Tutorials
- [RAG from Scratch (YouTube)](https://www.youtube.com/results?search_query=rag+from+scratch)
- [LlamaIndex RAG Tutorial](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html)
- [LangChain RAG Guide](https://python.langchain.com/docs/tutorials/rag/)

---

**If you find this useful, consider [sponsoring me](https://github.com/sponsors/asdfgh12345123)!**

*Last updated: 2026-05-29*
