# mcp-coworker


## System Workflow

```mermaid
flowchart LR
    U[User Input] --> FE[Frontend UI]

    FE --> API[FastAPI Backend]

    API --> AG[OpenAI Agent<br/>(Reasoning + Tools)]
    
    AG --> HUB[FastMCP Tool Hub]
    HUB --> TE[Tool Execution Engine]
    TE --> HUB
    
    HUB --> AG
    AG --> API
    API --> FE[Frontend UI<br/>(Two panels update)]




