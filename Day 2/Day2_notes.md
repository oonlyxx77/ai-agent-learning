### Day 2

- Tools: a function or a program that a LLM based application uses to do something that the model itself can't do natively
  - Usage: know sth / do sth
  - Type:
    - function tools
    - built-in tools
    - agent tools

- Model Context Protocol (MCP) - connect brains and hands
  - Goal: unified plug and play way to connect tools
  - Components:
    - host: manage whole process, orchestrate agent thinking process
    - client: dedicated communication module to server, send cmd to server
    - server: actual program, execute cmd, send result back
  - Avoid context blow
    - RAG: Tool retrieval augmented generation