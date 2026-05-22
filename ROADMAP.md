# Complete Learning Roadmap: Agentic AI for Beginners

This roadmap breaks your journey into 4 phases, each with clear learning objectives, estimated duration, prerequisites, and hands-on projects.

## Phase 1: Foundations (Weeks 1–2, ~15 hours)

### Learning Objectives
- [ ] Understand Python classes, inheritance, and composition
- [ ] Use type hints and Python typing module
- [ ] Create and manage virtual environments
- [ ] Use Git and GitHub workflows
- [ ] Understand async/await for concurrent operations

### Estimated Time
- **Class basics:** 2 hours  
- **Type hints:** 2 hours  
- **Virtual environments & packaging:** 1.5 hours  
- **Git & GitHub:** 2 hours  
- **Async programming basics:** 2 hours  
- **Hands-on project:** 5.5 hours

### Prerequisites
- Basic Python knowledge (loops, functions, dictionaries)
- A text editor or IDE (VS Code, PyCharm, etc.)
- Command-line familiarity

### Recommended Resources

**Videos:**
1. [Real Python: Object-Oriented Programming](https://realpython.com/python-class-attributes/) – Class design fundamentals
2. [Corey Schafer: Python Type Hints](https://www.youtube.com/watch?v=-m2mtyKlGnw) – Comprehensive type annotation guide
3. [Tech with Tim: Async Python](https://www.youtube.com/watch?v=2IW6Kgp8NME) – Async/await explained

**Articles & Docs:**
1. [PEP 484 – Type Hints](https://www.python.org/dev/peps/pep-0484/) – Official Python type hints specification
2. [Real Python: Virtual Environments](https://realpython.com/python-virtual-environments-a-primer/) – venv and poetry
3. [GitHub Docs: Hello World](https://docs.github.com/en/get-started) – GitHub basics

### Hands-On Project 1: "Build a Simple Chatbot Class"

**Difficulty:** Beginner  
**Duration:** 5.5 hours

**Requirements:**
- Create a `SimpleChatbot` class with type hints
- Implement `add_response(trigger: str, response: str)` method
- Implement `chat(user_input: str) -> str` method that matches triggers
- Use a virtual environment and Git workflow
- Write unit tests using pytest

**Deliverables:**
- `src/chatbot.py` with class implementation
- `tests/test_chatbot.py` with ≥5 test cases
- Git history with 3+ meaningful commits
- `README.md` explaining how to run the chatbot

**Resources:**
- [Python Classes Tutorial](https://docs.python.org/3/tutorial/classes.html)
- [Pytest Intro](https://docs.pytest.org/en/stable/getting_started.html)

---

## Phase 2: Data Validation with Pydantic (Week 3, ~10 hours)

### Learning Objectives
- [ ] Model data with Pydantic `BaseModel`
- [ ] Validate input and output using field validators
- [ ] Handle type coercion and custom validators
- [ ] Serialize/deserialize models to JSON
- [ ] Use Pydantic in ML/AI pipelines

### Estimated Time
- **Pydantic basics:** 2.5 hours  
- **Field validators:** 2 hours  
- **Serialization:** 1.5 hours  
- **Custom validators:** 2 hours  
- **Hands-on project:** 2 hours

### Prerequisites
- Phase 1 completed (Python, type hints)

### Recommended Resources

**Official Docs:**
1. [Pydantic Docs: Models](https://docs.pydantic.dev/latest/concepts/models/) – Core model API
2. [Pydantic Docs: Validators](https://docs.pydantic.dev/latest/concepts/validators/) – Validation patterns
3. [Pydantic GitHub](https://github.com/pydantic/pydantic) – Source code and examples

**Videos:**
1. [Tech with Tim: Pydantic in 30 Minutes](https://www.youtube.com/watch?v=U7F0mC0Y6I8) – Quick start with examples
2. [Validation Best Practices](https://www.youtube.com/watch?v=r4-3A1RFHpM) – Real-world validation patterns

### Hands-On Project 2: "Build a User Registration API with Validation"

**Difficulty:** Beginner  
**Duration:** 2 hours

**Requirements:**
- Create a `User` Pydantic model with fields: `email`, `username`, `age`, `password`
- Validate email format, username uniqueness (mock), age range (18+)
- Create a `UserValidator` function that handles errors gracefully
- Serialize users to JSON
- Test with invalid inputs

**Deliverables:**
- `src/models/user_model.py`
- `tests/test_user_model.py` with validation tests
- Example usage in `examples/02_pydantic_basics.py`

**Citation:**  
[Pydantic Best Practices](https://docs.pydantic.dev/latest/usage/models/) – Official validation guide

---

## Phase 3: LLMs & Agents Fundamentals (Weeks 4–6, ~25 hours)

### Subphase 3a: LangChain Basics (Week 4)

#### Learning Objectives
- [ ] Understand LLMs and API-based model interaction
- [ ] Build prompts and prompt templates
- [ ] Chain LLM calls together
- [ ] Handle outputs and structured responses
- [ ] Integrate external tools (API calls)

#### Estimated Time
- **LLM fundamentals:** 2 hours  
- **LangChain core concepts:** 2.5 hours  
- **Prompts & chains:** 2 hours  
- **Output parsing:** 1.5 hours  
- **Hands-on:** 3 hours

#### Recommended Resources

**Official Docs:**
1. [LangChain: Get Started](https://docs.langchain.com/docs/get_started/introduction) – Quick introduction
2. [LangChain: LLMs](https://docs.langchain.com/docs/modules/model_io/llms/) – LLM integration patterns
3. [LangChain: Chains](https://docs.langchain.com/docs/modules/chains/) – Chain composition

**Videos:**
1. [LangChain Tutorial Series](https://www.youtube.com/playlist?list=PLqZTnrySJwjyJfqpBqYvXjN63Jz-gKm4Z) – Official YouTube tutorials
2. [Building with LLMs (YouTube)](https://www.youtube.com/watch?v=zaJH-sKTvIE) – Practical patterns

#### Hands-On Project 3a: "Build a Summarization Chain"

**Difficulty:** Beginner  
**Duration:** 3 hours

**Requirements:**
- Create a LangChain chain that takes a long document and summarizes it
- Use a `ChatPromptTemplate` with a system prompt and user input
- Chain multiple LLM calls (main summary + key points)
- Handle token limits gracefully
- Test with sample documents

**Deliverables:**
- `src/examples/03_langchain_chain.py`
- Test with documents in `data/`
- Document the chain architecture

---

### Subphase 3b: Agents & Tool Use (Weeks 5–6)

#### Learning Objectives
- [ ] Understand agent architecture and reasoning loops
- [ ] Define tools and their schemas
- [ ] Implement ReAct (Reason, Act, Observe) pattern
- [ ] Handle tool errors and retries
- [ ] Build multi-tool agents
- [ ] Understand function calling (OpenAI, Anthropic)

#### Estimated Time
- **Agent architecture:** 2.5 hours  
- **Tool definitions:** 2 hours  
- **ReAct pattern:** 2 hours  
- **Function calling:** 2 hours  
- **Debugging agents:** 1.5 hours  
- **Hands-on:** 6 hours

#### Recommended Resources

**Official Documentation:**
1. [LangChain: Agents](https://docs.langchain.com/docs/modules/agents/) – Agent frameworks
2. [LangChain: Tools](https://docs.langchain.com/docs/modules/tools/) – Tool integration
3. [OpenAI: Function Calling](https://platform.openai.com/docs/guides/function-calling) – Structured tool use

**Papers & References:**
1. [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) – Foundational ReAct paper (cite: Yao et al., NeurIPS 2022)
2. [Agents: Autonomous Reasoning and Action](https://www.anthropic.com/research/agents) – Anthropic's agent research

**Videos:**
1. [Building Agents with LLMs](https://www.youtube.com/watch?v=wSZt-D5uDSI) – Harrison Chase (LangChain creator)
2. [OpenAI Function Calling](https://www.youtube.com/watch?v=BwmTLV9kGqY) – Practical examples

#### Hands-On Project 3b: "Build a Math Agent with Tools"

**Difficulty:** Intermediate  
**Duration:** 6 hours

**Requirements:**
- Create calculator, unit converter, and symbolic math tools
- Build an agent that can solve multi-step math problems
- Implement tool error handling (e.g., division by zero)
- Use LangChain's `AgentExecutor`
- Add logging to trace agent reasoning
- Test with 10+ math problems of varying complexity

**Deliverables:**
- `src/tools/calculator.py`, `src/tools/converter.py`
- `src/agents/tool_agent.py`
- `examples/04_agent_with_tools.py`
- `tests/test_agents.py`
- Agent trace logs showing reasoning

---

## Phase 4: Memory, Orchestration & Production (Weeks 7–9, ~20 hours)

### Subphase 4a: Memory & State (Week 7, ~8 hours)

#### Learning Objectives
- [ ] Understand memory types: short-term (conversation buffer), long-term (vector DB)
- [ ] Implement conversation memory
- [ ] Use semantic search for relevant memory retrieval
- [ ] Handle memory size limits and pruning
- [ ] Store and retrieve agent state

#### Estimated Time
- **Memory architectures:** 2 hours  
- **Conversation buffers:** 1.5 hours  
- **Vector memory & embeddings:** 2 hours  
- **Hands-on:** 2.5 hours

#### Recommended Resources

**Documentation:**
1. [LangChain: Memory](https://docs.langchain.com/docs/modules/memory/) – Memory module overview
2. [Chroma: Vector Database](https://www.trychroma.com/) – Semantic search backend
3. [Pinecone: Vector DB](https://www.pinecone.io/learn/vector-database/) – Scalable memory

**Papers:**
1. [Retrieval-Augmented Generation (RAG)](https://arxiv.org/abs/2005.11401) – Lewis et al., Facebook Research
2. [Long-Form Question Answering with RAG](https://arxiv.org/abs/2005.11401) – Extended retrieval patterns

#### Hands-On Project 4a: "Conversational Agent with Memory"

**Difficulty:** Intermediate  
**Duration:** 2.5 hours

**Requirements:**
- Build a chatbot that remembers conversation history
- Implement a conversation buffer with token limits
- Use semantic search to retrieve relevant past interactions
- Handle multiple conversation sessions
- Persist memory to disk

**Deliverables:**
- `src/agents/memory_agent.py`
- `examples/05_memory_conversation.py`
- Memory storage in `data/conversations/`

---

### Subphase 4b: LangGraph & Orchestration (Week 8, ~8 hours)

#### Learning Objectives
- [ ] Understand state graphs and node/edge patterns
- [ ] Build linear, branching, and looping workflows
- [ ] Implement conditional logic in workflows
- [ ] Combine multiple agents in a graph
- [ ] Handle errors and retries in workflows
- [ ] Persist and resume graph execution

#### Estimated Time
- **Graph fundamentals:** 1.5 hours  
- **StateGraph API:** 2 hours  
- **Conditional routing:** 1.5 hours  
- **Multi-agent graphs:** 2 hours  
- **Hands-on:** 2 hours

#### Recommended Resources

**Official Docs:**
1. [LangGraph Docs](https://docs.langchain.com/oss/python/langgraph/) – Complete API reference
2. [LangGraph Examples](https://github.com/langchain-ai/langgraph/tree/main/examples) – Real-world patterns
3. [GitHub: LangGraph](https://github.com/langchain-ai/langgraph) – Source code

**Videos:**
1. [LangGraph Tutorial](https://www.youtube.com/watch?v=w4RBhKDHcVw) – Walkthrough from LangChain team
2. [Building Workflows with StateGraph](https://www.youtube.com/watch?v=kRJH6hxvjXg) – Advanced patterns

#### Hands-On Project 4b: "Multi-Agent Workflow with LangGraph"

**Difficulty:** Intermediate-Advanced  
**Duration:** 2 hours

**Requirements:**
- Design a 2-agent workflow: Researcher agent + Writer agent
- Researcher finds information; Writer creates a summary
- Implement conditional routing (if confident, finalize; else, research more)
- Add error handling and retry logic
- Visualize the graph structure

**Deliverables:**
- `src/workflows/simple_graph.py`
- `examples/06_graph_workflow.py`
- Graph visualization (PNG/SVG)
- `tests/test_workflows.py`

---

### Subphase 4c: Production & Deployment (Week 9, ~4 hours)

#### Learning Objectives
- [ ] Write unit and integration tests for agents
- [ ] Set up CI/CD pipelines
- [ ] Monitor and log agent behavior
- [ ] Handle cost and rate limits
- [ ] Deploy to cloud (AWS, GCP, Azure, or Docker)
- [ ] Implement observability and tracing

#### Estimated Time
- **Testing strategies:** 1 hour  
- **Logging & monitoring:** 1 hour  
- **CI/CD setup:** 1 hour  
- **Deployment options:** 1 hour

#### Recommended Resources

**Documentation:**
1. [Pytest Docs](https://docs.pytest.org/) – Testing framework
2. [GitHub Actions: CI/CD](https://docs.github.com/en/actions) – Automated testing/deployment
3. [LangSmith Observability](https://smith.langchain.com/) – Agent monitoring (from LangChain team)
4. [Docker for Python](https://docs.docker.com/language/python/) – Containerization

**Guides:**
1. [Twelve-Factor App](https://12factor.net/) – Best practices for app design
2. [Monitoring LLM Applications](https://python.langchain.com/docs/modules/callbacks/) – Observability patterns

#### Hands-On Project 4c: "Production-Ready Agent"

**Difficulty:** Advanced  
**Duration:** 4 hours

**Requirements:**
- Write ≥80% test coverage for agents and tools
- Set up GitHub Actions CI for tests + linting
- Configure logging with `structlog` or `logging`
- Add rate-limit handling for API calls
- Create a Dockerfile for containerization
- Deploy to AWS Lambda or Docker Hub
- Document production deployment steps

**Deliverables:**
- Updated `tests/` with comprehensive coverage
- `.github/workflows/ci.yml`
- `Dockerfile` and `docker-compose.yml`
- `scripts/deploy.sh`
- `docs/07-production-checklist.md`
- Deployment logs and monitoring dashboard

---

## 📊 Milestone Checklist

- [ ] **Week 1–2:** Completed Phase 1 project (chatbot class + Git history)
- [ ] **Week 3:** Completed Phase 2 project (user model with validation)
- [ ] **Week 4:** Completed Phase 3a project (summarization chain)
- [ ] **Weeks 5–6:** Completed Phase 3b project (math agent with tools)
- [ ] **Week 7:** Completed Phase 4a project (memory-enabled chatbot)
- [ ] **Week 8:** Completed Phase 4b project (multi-agent LangGraph workflow)
- [ ] **Week 9:** Completed Phase 4c project (production-ready deployment)

---

## 🎓 Next Steps After Completion

1. **Build Your Own Project:** Combine concepts to create a novel agent (e.g., research assistant, code reviewer)
2. **Explore Advanced Topics:** Model fine-tuning, multi-modal agents, real-time voice agents
3. **Contribute:** Submit examples or improvements back to this repo
4. **Join Communities:** [LangChain Discord](https://discord.gg/6adMQxSpJS), [Anthropic Forums](https://community.anthropic.com/)

---

## 📖 Additional Resources by Topic

### Python & Type Hints
- [Real Python: Type Hints Cheat Sheet](https://realpython.com/python-type-checking/)
- [PEP 484 – Type Hints](https://www.python.org/dev/peps/pep-0484/)

### Pydantic
- [Pydantic GitHub](https://github.com/pydantic/pydantic)
- [Pydantic Docs](https://docs.pydantic.dev/)

### LLMs & Prompting
- [OpenAI API Docs](https://platform.openai.com/docs)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)

### Agent Frameworks
- [LangChain](https://github.com/langchain-ai/langchain)
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [CrewAI](https://github.com/crewAIInc/crewAI)
- [Pydantic AI](https://github.com/pydantic/pydantic-ai)

### Production & Deployment
- [LangSmith](https://smith.langchain.com/)
- [Hugging Face Spaces](https://huggingface.co/spaces)
- [AWS Lambda](https://aws.amazon.com/lambda/)