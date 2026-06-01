# Awesome RAG [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of retrieval-augmented generation tools, vector databases, embedding models, chunking strategies, retrieval techniques, re-ranking tools, evaluation methods, and production guides.

Awesome RAG is a focused list for exploring how retrieval-augmented generation is built and improved in practice. It is a companion repository for AI Tools Hub.

## Main hub

- Main site: https://asdfgh12345123.github.io/awesome-ai-tools/
- AI Tools Directory: https://asdfgh12345123.github.io/awesome-ai-tools/tools/generated.html
- RAG Guide: https://asdfgh12345123.github.io/awesome-ai-tools/guides/rag-tools-comparison.html

## Support this project

- Ko-fi: https://ko-fi.com/aitoolshub
- 爱发电: https://ifdian.net/a/aitoolshub

## Table of Contents
- [Frameworks](#frameworks)
- [Vector Databases](#vector-databases)
- [Embedding Models](#embedding-models)
- [Chunking Strategies](#chunking-strategies)
- [Retrieval Techniques](#retrieval-techniques)
- [Re-ranking](#re-ranking)
- [Evaluation](#evaluation)
- [Tutorials](#tutorials)
- [Research Papers](#research-papers)
- [Production Guides](#production-guides)

---

## Frameworks
| Name | Stars | Description |
|------|-------|-------------|
| [LangChain](https://github.com/langchain-ai/langchain) | 138k+ | Build context-aware LLM applications |
| [LlamaIndex](https://github.com/run-llama/llama_index) | 50k+ | Data framework for LLM apps |
| [Haystack](https://github.com/deepset-ai/haystack) | 25k+ | End-to-end NLP framework |
| [RAGFlow](https://github.com/infiniflow/ragflow) | 82k+ | Open-source RAG engine |
| [Dify](https://github.com/langgenius/dify) | 143k+ | LLM app development platform |
| [R2R](https://github.com/SciPhi-AI/R2R) | 8k+ | RAG to production |
| [Verba](https://github.com/weaviate/Verba) | 16k+ | RAG chatbot by Weaviate |
| [FastRAG](https://github.com/IntelLabs/fastRAG) | 2k+ | Optimized RAG framework |
| [Canopy](https://github.com/pinecone-io/canopy) | 1k+ | RAG framework by Pinecone |
| [Kotaemon](https://github.com/Cinnamon/kotaemon) | 25k+ | Open-source RAG UI |
| [DocsGPT](https://github.com/arc53/DocsGPT) | 18k+ | RAG for documentation |
| [PrivateGPT](https://github.com/zylon-ai/private-gpt) | 57k+ | Private RAG solution |

## Vector Databases
| Name | Type | Description |
|------|------|-------------|
| [Weaviate](https://github.com/weaviate/weaviate) | 16k+ | Vector search engine |
| [Milvus](https://github.com/milvus-io/milvus) | 45k+ | High-performance vector DB |
| [Chroma](https://github.com/chroma-core/chroma) | 28k+ | AI-native embedding DB |
| [Qdrant](https://github.com/qdrant/qdrant) | 32k+ | High-performance vector search |
| [Pinecone](https://www.pinecone.io/) | Managed | Serverless vector database |
| [pgvector](https://github.com/pgvector/pgvector) | 22k+ | Vector similarity for PostgreSQL |
| [LanceDB](https://github.com/lancedb/lancedb) | 10k+ | Developer-friendly vector DB |
| [Redis](https://redis.io/) | Open-source | Vector search in Redis |
| [Elasticsearch](https://www.elastic.co/elasticsearch) | Open-source | Vector search in ES |
| [Vespa](https://github.com/vespa-engine/vespa) | 7k+ | Full-text and vector search |
| [Typesense](https://github.com/typesense/typesense) | 26k+ | Fast typo-tolerant search |
| [Marqo](https://github.com/marqo-ai/marqo) | 5k+ | Tensor-based search |

## Embedding Models
| Model | Provider | Dims | Description |
|-------|----------|------|-------------|
| [text-embedding-3-large](https://platform.openai.com/docs/guides/embeddings) | OpenAI | 3072 | Best OpenAI embedding |
| [text-embedding-3-small](https://platform.openai.com/docs/guides/embeddings) | OpenAI | 1536 | Cost-effective OpenAI |
| [voyage-3](https://www.voyageai.com/) | Voyage | 1024 | High-performance embeddings |
| [Cohere Embed v3](https://cohere.com/embed) | Cohere | 1024 | Multilingual embeddings |
| [BGE-M3](https://github.com/FlagOpen/FlagEmbedding) | 12k+ | 1024 | Multilingual, multi-granularity |
| [E5-Mistral](https://huggingface.co/intfloat/e5-mistral-7b-instruct) | Open-source | 4096 | Strong open embedding |
| [GTE-Qwen2](https://huggingface.co/Alibaba-NLP/gte-Qwen2-7B-instruct) | Open-source | 3584 | Alibaba embedding model |
| [Jina Embeddings v3](https://jina.ai/embeddings/) | Jina | 1024 | Flexible embedding model |
| [Nomic Embed](https://www.nomic.ai/) | Open-source | 768 | Open-source embedding |

## Chunking Strategies
| Strategy | Best For | Description |
|----------|----------|-------------|
| Fixed-size | Quick start | Simple character/token-based splitting |
| Recursive character | General use | LangChain default, respects structure |
| Semantic | High quality | Embedding-based boundary detection |
| Document structure | Structured docs | Uses headings, paragraphs, sections |
| Agentic | Complex docs | LLM-powered intelligent chunking |
| Parent-child | Context window | Small chunks for retrieval, large for context |

### Chunking Best Practices
1. Start with 512 tokens, 50 token overlap
2. Test different sizes (256, 512, 1024)
3. Use metadata enrichment (source, page, section)
4. Consider hybrid chunking for mixed content

## Retrieval Techniques
| Technique | Description |
|-----------|-------------|
| Dense retrieval | Vector similarity search |
| Sparse retrieval | BM25, TF-IDF keyword search |
| Hybrid search | Combine dense + sparse |
| Multi-query | Generate multiple query variations |
| Parent-document | Retrieve small, return large |
| Self-query | LLM extracts filters from query |
| Contextual compression | Extract relevant passages |
| Ensemble | Combine multiple retrievers |

## Re-ranking
| Name | Description |
|------|-------------|
| [Cohere Rerank](https://cohere.com/rerank) | API-based re-ranking |
| [BGE Reranker](https://github.com/FlagOpen/FlagEmbedding) | 12k+ |
| [ColBERT](https://github.com/stanford-futuredata/ColBERT) | 4k+ |
| [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) | 980 |
| [RankLLM](https://github.com/castorini/rank_llm) | 600 |
| [LLM Re-ranking](https://python.langchain.com/docs/integrations/retrievers/LLM-Reranker) | Use any LLM for re-ranking |

## Evaluation
| Tool | Description |
|------|-------------|
| [RAGAS](https://github.com/explodinggradients/ragas) | 14k+ |
| [DeepEval](https://github.com/confident-ai/deepeval) | 16k+ |
| [TruLens](https://github.com/truera/trulens) | 3k+ |
| [LangSmith](https://smith.langchain.com/) | LangChain tracing & eval |
| [Phoenix](https://github.com/Arize-ai/phoenix) | 10k+ |
| [RAGChecker](https://github.com/tonywu71/RAGChecker) | Fine-grained RAG evaluation |

## Tutorials
- [RAG from Scratch (LangChain)](https://github.com/langchain-ai/rag-from-scratch)
- [LlamaIndex RAG Tutorial](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html)
- [Haystack RAG Pipeline](https://haystack.deepset.ai/tutorials/rag)
- [RAG with Weaviate](https://weaviate.io/developers/weaviate/quickstart)
- [Advanced RAG Techniques](https://www.youtube.com/results?search_query=advanced+rag+techniques)
- [Production RAG Guide](https://www.pinecone.io/learn/series/rag/)

## Research Papers
- [RAG (Original Paper, 2020)](https://arxiv.org/abs/2005.11401)
- [REALM (2020)](https://arxiv.org/abs/2002.08909)
- [RETRO (2021)](https://arxiv.org/abs/2112.04426)
- [Atlas (2022)](https://arxiv.org/abs/2208.03299)
- [Self-RAG (2023)](https://arxiv.org/abs/2310.11511)
- [RAPTOR (2024)](https://arxiv.org/abs/2401.18059)
- [CRAG (2024)](https://arxiv.org/abs/2401.15884)
- [GraphRAG (2024)](https://arxiv.org/abs/2404.16130)

## Production Guides
- [RAG in Production (Pinecone)](https://www.pinecone.io/learn/series/rag/)
- [Scaling RAG (Weaviate)](https://weaviate.io/developers/weaviate)
- [RAG Architecture Patterns](https://www.anthropic.com/engineering/building-effective-agents)
- [Chunking for Production](https://www.llamaindex.ai/blog/a-cheat-sheet-and-some-recipes-for-building-advanced-rag-803a9d94c41b)
