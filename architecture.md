# ASMOS Architecture

## High-Level Architecture

ASMOS is designed to optimize contextual memory management in multi-agent LLM systems by storing only high-value semantic information instead of complete conversation histories.

The system consists of the following components:

### 1. Multi-Agent System
Multiple AI agents collaborate to solve a task while generating contextual information.

### 2. Semantic Checkpoint Manager
Extracts meaningful semantic checkpoints from ongoing conversations, eliminating redundant context while preserving important information.

### 3. Memory Scoring Engine
Evaluates each checkpoint using:
- Confidence Score
- Utility Score

These scores determine the importance of a memory for future retrieval.

### 4. Memory Lifecycle Manager
Based on the computed scores, memories are:
- Promoted
- Retained
- Archived

This keeps the memory store efficient and relevant.

### 5. Context Retrieval
When a new query arrives, only the highest-value memories are retrieved instead of the entire conversation history.

### 6. Prompt Construction
Retrieved memories are combined with the current user query to construct an optimized prompt.

### 7. Large Language Model
The optimized prompt is sent to the LLM, producing an accurate response with significantly fewer tokens.

---

## Key Benefits

- Reduced redundant context
- Adaptive memory management
- Improved retrieval efficiency
- Lower LLM token consumption
- Better scalability for long-running multi-agent systems
