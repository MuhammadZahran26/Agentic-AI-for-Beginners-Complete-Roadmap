# Syllabus: Agentic AI for Beginners

## Course Overview

| Metric | Details |
|--------|----------|
| **Duration** | 9 weeks (15–20 hours/week recommended) |
| **Level** | Beginner to Intermediate |
| **Prerequisites** | Basic Python (loops, functions, dictionaries) |
| **Time Commitment** | ~135–180 hours total |
| **Certification** | None (self-paced) |
| **Tools Used** | Python 3.9+, LangChain, LangGraph, Pydantic, Git |

## Learning Outcomes

By the end of this course, you will:

1. **Design and implement** Python classes and type-safe data structures
2. **Validate** data using Pydantic models in real-world scenarios
3. **Build LLM applications** using LangChain (prompts, chains, parsing)
4. **Create agents** that use tools and reason through problems
5. **Implement memory** systems for conversational AI
6. **Orchestrate** complex multi-agent workflows with LangGraph
7. **Deploy** production-grade agents with tests, monitoring, and CI/CD

## Weekly Schedule

### Week 1: Python Fundamentals – Part 1
**Topics:** Classes, inheritance, composition  
**Time:** 4 hours  
**Key Concepts:**
- Class definition and instantiation
- Instance and class variables
- Methods and `self`
- Inheritance and method overriding
- Composition vs. inheritance

**Required Reading:**
- [Python Docs: Classes](https://docs.python.org/3/tutorial/classes.html)
- [Real Python: OOP](https://realpython.com/intro-to-python-object-oriented-programming/)

**Assignment:**
- Create a `Vehicle` class with subclasses `Car` and `Bike`
- Add 5+ methods demonstrating OOP concepts

**Resources:**
- Video: [CampusX: Python OOP](https://youtu.be/Mf2RdpEiXjU?si=JQLB7x3LgcIZzAhz)

---

### Week 2: Python Fundamentals – Part 2
**Topics:** Type hints, virtual environments, async basics  
**Time:** 4 hours  
**Key Concepts:**
- Type annotations and `typing` module
- Function signatures with types
- Generic types (`List`, `Dict`, `Optional`)
- Virtual environments (`venv`, `poetry`)
- Async/await and `asyncio`

**Required Reading:**
- [PEP 484: Type Hints](https://www.python.org/dev/peps/pep-0484/)
- [Real Python: Async Python](https://realpython.com/ref/glossary/oop/)

**Assignment:**
- Refactor Phase 1 project with full type hints
- Create async version of chatbot class
- Set up development environment with `pyproject.toml`

**Resources:**
- Video: [Real Python: Type Hints](https://www.youtube.com/watch?v=Ybn3_0qAI8I)

---

### Week 2 (cont.): Git & GitHub Workflow
**Topics:** Git basics, GitHub, version control  
**Time:** 2 hours  
**Key Concepts:**
- Git workflow: init, add, commit, push
- Branches and pull requests
- GitHub fork and collaboration
- `.gitignore` and repository setup

**Required Reading:**
- [GitHub Docs: Hello World](https://docs.github.com/en/get-started)
- [Atlassian: Git Tutorial](https://www.atlassian.com/git/tutorials)

**Assignment:**
- Initialize repo with proper `.gitignore`
- Create 3+ branches for Phase 1 project
- Submit PR with meaningful commit messages

**Resources:**
- Video: [Git & GitHub Crash Course](https://www.youtube.com/watch?v=RGOj5yH7evk)

---

### Week 3: Pydantic & Data Validation
**Topics:** Pydantic models, validators, serialization  
**Time:** 5 hours  
**Key Concepts:**
- `BaseModel` and field definitions
- Field validators and root validators
- Type coercion and custom types
- Serialization to JSON/dict
- Pydantic in AI pipelines

**Required Reading:**
- [Pydantic Docs: Models](https://docs.pydantic.dev/latest/concepts/models/)
- [Pydantic Docs: Validators](https://docs.pydantic.dev/latest/concepts/validators/)

**Assignment:**
- Complete Phase 2 project: User registration model with full validation

**Resources:**
- Video: [Pydantic Master Class](https://www.youtube.com/watch?v=ahL-rCQ_Oms)
- Article: [Pydantic for ML Engineers](https://realpython.com/pydantic/)

---

### Week 4: LangChain Fundamentals
**Topics:** LLMs, prompts, chains, output parsing  
**Time:** 7 hours  
**Key Concepts:**
- LLM interfaces (ChatOpenAI, etc.)
- `PromptTemplate` and `ChatPromptTemplate`
- Chain composition with `|` (pipe operator)
- Output parsing (JSON, structured output)
- Token limits and cost management

**Required Reading:**
- [LangChain: Get Started](https://docs.langchain.com/docs/get_started/introduction)
- [LangChain: LLMs & Chat Models](https://docs.langchain.com/docs/modules/model_io/llms/)
- [LangChain: Chains](https://docs.langchain.com/docs/modules/chains/)

**Assignment:**
- Complete Phase 3a project: Summarization chain with multi-step reasoning

**Resources:**
- Video: [LangChain Beginner Course](https://www.youtube.com/watch?v=aywZrzNZSsY)
- Docs: [LangChain Expression Language (LCEL)](https://docs.langchain.com/docs/expression_language/get_started)

---

### Week 5: Agents & Tool Use – Part 1
**Topics:** Agent architecture, tool definitions, ReAct pattern  
**Time:** 5 hours  
**Key Concepts:**
- Agent reasoning loop (Thought → Action → Observation)
- Tool schema and `@tool` decorator
- `BaseTool` and tool validation
- Agent types: ReAct, conversational, structured chat
- Function calling (OpenAI, Anthropic)

**Required Reading:**
- [LangChain: Agents](https://docs.langchain.com/docs/modules/agents/)
- [LangChain: Tools](https://docs.langchain.com/docs/modules/tools/)
- [ReAct Paper](https://arxiv.org/abs/2210.03629)

**Assignment:**
- Build 3–4 tools: calculator, web search mock, date/time
- Create a ReAct agent that chains tools together

**Resources:**
- Video: [LangChain Agents Explained](https://www.youtube.com/watch?v=rGR6cMWDfh0)

---

### Week 6: Agents & Tool Use – Part 2
**Topics:** Multi-tool agents, error handling, observability  
**Time:** 5 hours  
**Key Concepts:**
- AgentExecutor and execution loops
- Error handling and retries
- Max iterations and early stopping
- Logging and debugging agents
- Agent evaluation and testing

**Assignment:**
- Complete Phase 3b project: Math agent with tool chains
- Add logging, error handling, and test suite

**Resources:**
- Article: [Debugging Agents](https://python.langchain.com/docs/modules/callbacks/)
- Video: [Building Robust Agents](https://www.youtube.com/watch?v=TFr7QQvWc_Q)

---

### Week 7: Memory & State Management
**Topics:** Conversation memory, semantic retrieval, state persistence  
**Time:** 5 hours  
**Key Concepts:**
- `ConversationBufferMemory` and token-limited variants
- Semantic search with embeddings
- Vector databases (Chroma, Pinecone)
- Conversation state in agents
- Memory persistence and cleanup

**Required Reading:**
- [LangChain: Memory](https://docs.langchain.com/docs/modules/memory/)
- [RAG Paper](https://arxiv.org/abs/2005.11401)
- [Embeddings Guide](https://docs.langchain.com/docs/modules/data_connection/text_embedding/)

**Assignment:**
- Complete Phase 4a project: Conversational agent with memory
- Implement token-aware buffer and semantic search

**Resources:**
- Video: [Memory in LLM Apps](https://www.youtube.com/watch?v=dIE3W4oYjhQ)

---

### Week 8: LangGraph & Orchestration
**Topics:** State graphs, workflows, multi-agent patterns  
**Time:** 5 hours  
**Key Concepts:**
- `StateGraph` and node/edge design
- Conditional routing and branching
- Graph visualization
- Multi-agent graphs (supervisor, consensus, sequential)
- Checkpointing and resumption

**Required Reading:**
- [LangGraph Docs](https://docs.langchain.com/oss/python/langgraph/)
- [LangGraph Examples](https://github.com/langchain-ai/langgraph/tree/main/examples)

**Assignment:**
- Complete Phase 4b project: Multi-agent LangGraph workflow
- Build researcher + writer agents with conditional logic

**Resources:**
- Video: [LangGraph Tutorial](https://www.youtube.com/watch?v=w4RBhKDHcVw)
- Blog: [Building Graphs with LangChain](https://blog.langchain.dev/)

---

### Week 9: Production & Deployment
**Topics:** Testing, CI/CD, monitoring, cloud deployment  
**Time:** 6 hours  
**Key Concepts:**
- Unit and integration testing (pytest)
- GitHub Actions for CI/CD
- Logging and observability (LangSmith, custom logs)
- Rate limiting and cost control
- Containerization (Docker) and cloud deployment (AWS Lambda, Cloud Run)
- Monitoring and alerting

**Required Reading:**
- [Pytest Docs](https://docs.pytest.org/)
- [GitHub Actions: CI/CD](https://docs.github.com/en/actions)
- [Twelve-Factor App](https://12factor.net/)
- [LangSmith](https://smith.langchain.com/)

**Assignment:**
- Complete Phase 4c project: Production-ready agent with full CI/CD

**Resources:**
- Video: [Testing Python Code](https://www.youtube.com/watch?v=6tNS--WetLI)
- Guide: [AWS Lambda with Python](https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html)

---

## Grading & Assessment

This is a **self-paced, project-based** course. Progress is measured by:

| Milestone | Weight |
|-----------|--------|
| Phase 1 Project (Chatbot Class) | 15% |
| Phase 2 Project (Pydantic Validation) | 15% |
| Phase 3a Project (LangChain Chain) | 15% |
| Phase 3b Project (Agent with Tools) | 20% |
| Phase 4a Project (Memory Agent) | 15% |
| Phase 4b Project (LangGraph Workflow) | 15% |
| Phase 4c Project (Production Deployment) | 10% |

**Passing Criteria:**
- All 7 projects completed
- ≥80% test coverage for code
- All code has inline documentation
- GitHub repository shows meaningful commit history

---

## Resources & Support

### Official Documentation
- [Python Docs](https://docs.python.org/)
- [LangChain Docs](https://docs.langchain.com/)
- [LangGraph Docs](https://docs.langchain.com/oss/python/langgraph/)
- [Pydantic Docs](https://docs.pydantic.dev/)

### Community & Help
- [LangChain Discord](https://discord.gg/6adMQxSpJS)
- [GitHub Discussions](https://github.com/MuhammadZahran26/Agentic-AI-for-Beginners-Complete-Roadmap/discussions)
- [Stack Overflow: langchain, pydantic](https://stackoverflow.com/questions/tagged/langchain)

### Supplementary Videos
- [LangChain YouTube](https://www.youtube.com/channel/UCDyH__SsB66GaQSGJLpVjkw)
- [Harrison Chase Talks](https://www.youtube.com/results?search_query=harrison+chase+langchain)

### Books & Papers
- [Anthropic: Introduction to Agentic AI](https://www.anthropic.com/research/agents)
- [ReAct: Synergizing Reasoning and Acting](https://arxiv.org/abs/2210.03629)

---

## Course Policies

### Academic Integrity
- Projects must be your own work
- You may reference tutorials and official docs
- Cite all external sources and code

### Time Management
- Allocate 15–20 hours per week
- Complete phases in order
- Reach out on GitHub Discussions if stuck

### Feedback & Improvement
- Submit issues for unclear sections
- Contribute improvements via PRs
- Join discussions to help others
