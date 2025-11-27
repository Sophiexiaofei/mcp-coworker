# mcp-coworker



User Input
   │
   ▼
┌────────────────────┐
│   Frontend UI       │
└────────────────────┘
   │  sends message
   ▼
┌────────────────────┐
│   FastAPI Backend   │
└────────────────────┘
   │ forwards message
   ▼
┌────────────────────┐
│    OpenAI Agent     │
│  (Reasoning + Tools)│
└────────────────────┘
   │ decides tool usage
   ▼
┌────────────────────┐      ┌──────────────────────┐
│  FastMCP Tool Hub   │◀───▶│ Tool Execution Engine │
└────────────────────┘      └──────────────────────┘
   │ returns structured data
   ▼
┌────────────────────┐
│   OpenAI Agent      │
└────────────────────┘
   │ chat + structured output
   ▼
┌────────────────────┐
│  FastAPI Backend    │
└────────────────────┘
   │
   ▼
┌────────────────────┐
│  Frontend UI (two   │
│  panels update)     │
└────────────────────┘



