# Top 20 Authoritative Sources

**Search Date:** May 22, 2026

## 1. LangChain Documentation
**URL:** https://docs.langchain.com/  
**Type:** Official Documentation  
**Why:** Official LangChain framework docs. Essential for chains, agents, tools, memory, and evaluation. All code examples reference this.

## 2. LangGraph Documentation & GitHub
**URL:** https://docs.langchain.com/oss/python/langgraph/ | https://github.com/langchain-ai/langgraph  
**Type:** Official Docs + GitHub Repo (32.6k stars)  
**Why:** LangGraph is the modern orchestration layer for stateful agent workflows. Canonical examples and StateGraph API reference.

## 3. LangChain GitHub Repository
**URL:** https://github.com/langchain-ai/langchain  
**Type:** GitHub Repo (137.3k stars)  
**Why:** Official LangChain source code. Houses agents, memory, tools, and production examples. Reference implementation for all frameworks.

## 4. Pydantic Documentation
**URL:** https://docs.pydantic.dev/  
**Type:** Official Documentation  
**Why:** Complete guide to data validation with type hints. Essential for AI system data modeling. Examples cover validators, serialization, JSON schema.

## 5. Pydantic GitHub Repository
**URL:** https://github.com/pydantic/pydantic  
**Type:** GitHub Repo (27.8k stars)  
**Why:** Official Pydantic source. Reference for `BaseModel`, field validators, and Rust-based v2 implementation.

## 6. Pydantic AI Framework
**URL:** https://github.com/pydantic/pydantic-ai | https://ai.pydantic.dev  
**Type:** GitHub Repo (17.2k stars) + Official Docs  
**Why:** New Pydantic-native agent framework. Shows modern Pydantic integration patterns with agents and tools.

## 7. ReAct: Synergizing Reasoning and Acting in Language Models
**URL:** https://arxiv.org/abs/2210.03629  
**Type:** Academic Paper (NeurIPS 2023, Yao et al.)  
**Why:** Foundational agent reasoning pattern. Explains Thought→Action→Observation loop used in all agent examples.

## 8. OpenAI API Documentation
**URL:** https://platform.openai.com/docs  
**Type:** Official API Docs  
**Why:** Standard LLM provider. Function calling, chat completeness, token counting, rate limits all documented here.

## 9. CrewAI GitHub Repository
**URL:** https://github.com/crewAIInc/crewAI  
**Type:** GitHub Repo (51.9k stars)  
**Why:** Production multi-agent orchestration framework. Role-based agent patterns, delegation, and team dynamics.

## 10. Microsoft AutoGen Framework
**URL:** https://github.com/microsoft/autogen  
**Type:** GitHub Repo (58.2k stars)  
**Why:** Industrial-scale multi-agent framework. Conversation-based orchestration, code execution, and reproducibility.

## 11. Python Official Documentation: Classes
**URL:** https://docs.python.org/3/tutorial/classes.html  
**Type:** Official Documentation  
**Why:** Core Python language docs. Object-oriented programming, inheritance, method resolution order (MRO).

## 12. PEP 484 – Type Hints
**URL:** https://www.python.org/dev/peps/pep-0484/  
**Type:** Python Enhancement Proposal (Official)  
**Why:** Specification for Python type annotations. Canonical reference for `typing` module and static type checking.

## 13. Real Python: Type Hints Cheat Sheet
**URL:** https://realpython.com/python-type-checking/  
**Type:** Tutorial / Guide  
**Why:** Practical walkthrough of type hints, generics, and common patterns. Beginner-friendly with examples.

## 14. GitHub Documentation: Getting Started
**URL:** https://docs.github.com/en/get-started  
**Type:** Official Documentation  
**Why:** Git and GitHub workflows, branching strategies, PR reviews, collaborative development.

## 15. Prompt Engineering Guide
**URL:** https://www.promptingguide.ai/  
**Type:** Community-Curated Guide  
**Why:** Comprehensive prompt techniques: few-shot prompting, chain-of-thought, role-playing, output formatting.

## 16. Retrieval-Augmented Generation (RAG)
**URL:** https://arxiv.org/abs/2005.11401  
**Type:** Academic Paper (Lewis et al., Facebook Research, 2020)  
**Why:** Foundational RAG paper. Explains memory retrieval, embedding-based search, and long-context question answering.

## 17. Chroma Vector Database
**URL:** https://www.trychroma.com/ | https://github.com/chroma-core/chroma  
**Type:** Official Docs + GitHub  
**Why:** Lightweight vector database for semantic memory. Used in memory examples for embedding storage and retrieval.

## 18. Pytest Documentation
**URL:** https://docs.pytest.org/  
**Type:** Official Documentation  
**Why:** Standard Python testing framework. Fixtures, parametrization, coverage reporting, mocking.

## 19. GitHub Actions: CI/CD
**URL:** https://docs.github.com/en/actions  
**Type:** Official Documentation  
**Why:** Automated testing and deployment. YAML workflow configuration, secrets management, matrix builds.

## 20. Twelve-Factor App Methodology
**URL:** https://12factor.net/  
**Type:** Best Practices Guide  
**Why:** Production app design patterns. Config management, logging, concurrency, dependency isolation—all applied to agent deployment.

---

## Supplementary Sources (by Topic)

### Advanced Agent Patterns
- [Anthropic: Agents Intro](https://www.anthropic.com/research/agents)
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) (26.5k stars)
- [Agent Zero AI Framework](https://github.com/agent0ai/agent-zero) (17.7k stars)

### Multi-Agent Frameworks
- [CAMEL: Multi-Agent Framework](https://github.com/camel-ai/camel) (17k stars)
- [Swarms Framework](https://github.com/kyegomez/swarms) (6.7k stars)
- [Agent Squad](https://github.com/2FastLabs/agent-squad) (7.6k stars)

### Observability & Monitoring
- [LangSmith](https://smith.langchain.com/) – LangChain's native observability
- [AgentOps](https://github.com/AgentOps-AI/agentops) (5.5k stars) – Multi-framework agent monitoring

### Voice & Multimodal Agents
- [LiveKit Agents](https://github.com/livekit/agents) (10.5k stars) – Real-time voice AI
- [TEN Framework](https://github.com/TEN-framework/ten-framework) (10.5k stars) – Multimodal agent orchestration

### Specialized Frameworks
- [PraisonAI](https://github.com/MervinPraison/PraisonAI) (7.8k stars) – Autonomous agents with RAG
- [Griptape](https://github.com/griptape-ai/griptape) (2.5k stars) – Modular agent framework
- [Cheshire Cat](https://github.com/cheshire-cat-ai/core) (3k stars) – Microservice agent architecture

---

## Excluded Sources (Insufficient Verification)

The following were considered but excluded due to insufficient authoritative evidence or outdated information:
- Medium posts (not verified; subject to outdated advice)
- Twitter/X threads (ephemeral, not citable)
- Non-peer-reviewed blog posts without institutional backing

---

## How to Use This Sources List

1. **Learning:** Start with official docs (LangChain, Pydantic, Python). Then read papers for deep understanding.
2. **Code Examples:** Reference GitHub repos for production patterns (LangChain, LangGraph, CrewAI).
3. **Troubleshooting:** Search GitHub Issues/Discussions first, then Stack Overflow.
4. **Citation:** When adding content, cite using the format: `[Source Title](URL) – Brief context`.

---

## Future Updates

This list is maintained as of **May 22, 2026**. New frameworks and papers are emerging rapidly in agentic AI. Check GitHub stars and publication dates to find the latest authoritative resources.

Contributions of verified sources are welcome via GitHub Issues or PRs!