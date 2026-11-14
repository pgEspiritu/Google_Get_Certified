
# 🤖 A Brief History of Agents

## 📖 Introduction

Generative AI has transformed agents from simple, predefined virtual assistants into intelligent systems capable of **achieving goals by observing their environment, reasoning, and taking actions using available tools**.

### 🔄 Evolution of Agents

- **Early virtual agents**
  - Followed predefined paths and rules.
  - Had limited understanding of user intent.
  - Could not dynamically adapt to different situations.

- **Modern generative AI agents**
  - Understand user intent more naturally.
  - Access relevant information through techniques such as **Retrieval-Augmented Generation (RAG)**.
  - Observe their environment and use tools to perform actions.
  - Make decisions and adapt their actions to achieve specific goals.

## 🧩 Three Foundational Components of an AI Agent

### 1. 🧠 Foundational Model

- The underlying language model (LLM) that powers the agent.
- Can be:
  - Small or large language models.
  - Google's Gemini models.
  - Models from other AI providers.
- **Key consideration:** Select a model whose training data and capabilities are relevant to the agent's intended use case.

### 2. 🛠️ Tools

- Enable the agent to interact with the outside world.
- Allow the agent to both **observe information and perform actions**.
- Examples include:
  - **Extensions:** Connect agents to external APIs.
  - **Functions:** Perform specific operations or simulate API calls.
  - **Data stores:** Store and retrieve information, such as through vector databases.

### 3. 🔁 Reasoning Loop

- The core component responsible for decision-making and taking actions.
- An iterative process in which the agent:
  1. Considers its goal.
  2. Evaluates available tools.
  3. Gathers and analyzes information.
  4. Decides what action to take.
  5. Repeats the process until the goal is achieved.

- **ReAct (Reason and Act):** A commonly used framework that guides agents through reasoning and action.

## 🔑 Key Takeaways

- Modern AI agents go beyond predefined instructions and can dynamically work toward goals.
- **Foundational Model** provides intelligence and language understanding.
- **Tools** enable interaction with external systems and information.
- **Reasoning Loop** guides decisions and actions.
- These three components work together to make AI agents more capable, adaptive, and useful.
