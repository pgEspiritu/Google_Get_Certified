
# 🛠️ Adding in Tooling

## 📖 Introduction

Agent tooling enables generative AI agents to interact with the real world by providing the resources they need to accomplish tasks.

Think of tools as the agent's **skills, connections, and knowledge** that allow it to:

- 🔍 Access information.
- ⚙️ Perform actions.
- 🌐 Interact with external systems and services.

## 🧩 Four Types of Agent Tools

### 1. 🔌 Extensions (APIs)

- Connect agents to external APIs.
- APIs (Application Programming Interfaces) define rules that allow different software systems to communicate.
- Extensions provide a standardized way for agents to interact with APIs, regardless of their specific design.
- Simplify access to external services and data.

**Example: Travel Booking Agent**
- Uses an extension to communicate with a travel company's API.
- Searches for available flights and handles booking-related interactions.
- The extension manages the complexity of communicating with the travel company's systems.

### 2. ⚙️ Functions

- Represent specific actions an agent can perform.
- The agent's reasoning system selects the appropriate function based on the task.
- Can encapsulate complex logic or interactions.
- Make operations reusable and easier to manage.

**Example: `calculate_price` Function**
- Accepts flight details and passenger information as inputs.
- Calculates the total flight cost.
- Returns the calculated price to the agent.

### 3. 🗄️ Data Stores

- Provide agents with access to relevant information.
- Can contain:
  - Real-time data.
  - Historical data.
  - Knowledge bases.
  - Other structured or unstructured information.
- Help agents generate accurate, relevant, and up-to-date responses.

**Examples:**
- Current weather conditions.
- Stock prices.
- Customer information databases.

### 4. 🧩 Plugins

- Extend an agent's capabilities by adding new skills and integrations.
- Connect agents to specific services and platforms.
- Enable interaction with specialized tools.

**Examples:**
- **Calendar Plugin:** Allows an agent to schedule appointments.
- **Payment Gateway Plugin:** Enables an agent to process transactions.

## 🔄 How the Reasoning Loop Works with Tools

The **ReAct (Reason and Act)** framework describes how agents select, execute, and evaluate tools during task completion.

### ReAct Tool Interaction Cycle

#### 1. 🧠 Tool Selection

- The agent analyzes the user's task.
- Determines which tools are necessary.
- Evaluates available extensions, functions, and data stores.
- Selects the most appropriate resources.

#### 2. ⚙️ Tool Execution

- The agent executes the selected tool.
- Provides the required inputs.
- Examples:
  - Calling an API through an extension.
  - Invoking a function.
  - Querying a data store.

#### 3. 👀 Observation

- The agent receives the tool's output.
- The returned information becomes the **observation** in the ReAct cycle.
- The agent uses this information to evaluate the result.

#### 4. 🔁 Reasoning and Next Action

- The agent analyzes the observation.
- Determines whether the task is complete or requires additional actions.
- It may:
  - Select another tool.
  - Refine its approach.
  - Gather more information.
- The cycle repeats until the task is completed or a stopping condition is reached.

### 📌 ReAct Workflow Summary

```text
User Request
     ↓
🧠 Analyze Task and Select Tool
     ↓
⚙️ Execute Selected Tool
     ↓
👀 Observe Tool Output
     ↓
🔁 Reason About the Result
     ↓
Task Complete?
     ├── No → Select and Execute Another Tool
     └── Yes → 💬 Respond to User
```

## 🔑 Key Takeaways

- Agent tooling enables AI agents to access information, perform actions, and interact with external systems.
- The four key types of agent tools are:
  1. **Extensions (APIs):** Connect agents to external APIs and services.
  2. **Functions:** Perform specific, reusable operations.
  3. **Data Stores:** Provide access to information and knowledge.
  4. **Plugins:** Add specialized skills and integrations.
- The ReAct reasoning loop guides how agents select, execute, and evaluate tools.
- Tool outputs become observations that help agents determine their next actions.
- Agents can use multiple tools in sequence until the task is completed.

💡 **Remember:** Models provide the intelligence, reasoning loops guide decisions, and tools allow agents to interact with the outside world.
