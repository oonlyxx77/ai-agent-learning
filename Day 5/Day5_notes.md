### Day 5

Prototype to Production

- Three Fundational things
  - Automated Evaulation
  - Automated Deployment (CI/CD)
  - Comprehensive Observability
- Progressive Funnel
  - Phase1: Premerge Integration: unit test, lint, etc
  - Phase2: Postmerge Inteagration: load testing, integration test with real external service
  - Phase3: Gated deployment to Production: final human evaluation
- Prompt Ingestion, Data leakage
- Keep agent system healthy&scalable
  - Core idea: Decouple agent logic from its state
  - Speed: caching / parallelized task
  - Reliability: automated retries
  - Cost: optimize prompts, batch requests
- Agent Interation Protocals
  - MCP protocal: stateless; low level tool interations
  - A2A protocal: stateful; high level goal
    - Agent Cards
- Agent 2 Agent

Users → LLMAgent → RemoteA2aAgent(Client Proxy) → Server(Specific Agent)