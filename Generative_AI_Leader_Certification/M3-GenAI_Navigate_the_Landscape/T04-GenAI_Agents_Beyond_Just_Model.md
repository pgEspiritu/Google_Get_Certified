# Generative AI Agents: Beyond Just Models

## 1. Understanding AI Agents Beyond Language Models

AI agents are designed to **observe their environment, take actions, and achieve specific goals**.

Although agents use AI models, they offer capabilities beyond those of standalone models, particularly when handling complex tasks that require multiple steps, external information, and interaction with other systems.

Two key elements distinguish AI agents from standalone models:

1. **Reasoning loop** – The continuous process of observing, interpreting, planning, and acting to accomplish a goal.
2. **Tools** – Functionalities that allow agents to interact with external information, applications, services, and physical devices.

By combining these two elements, agents can move beyond generating text or other content and perform actions to solve problems.

## 2. The Two Key Elements of AI Agents

### A. Reasoning Loop

The **reasoning loop** is the agent's decision-making process. It allows the agent to evaluate information, determine what needs to be done, execute actions, and adjust its approach based on the results.

Unlike a standalone language model that typically generates an output in response to an input, an agent can repeat this process until it reaches its goal or a defined stopping point.

The reasoning loop generally consists of four stages:

1. **Observe:** Gather information about the environment, available resources, and task requirements.
2. **Interpret:** Process the gathered information and assess the current situation.
3. **Plan:** Determine the appropriate actions needed to achieve the goal.
4. **Act:** Execute the planned actions using available tools or capabilities.

The process then repeats as necessary.

### How the Reasoning Loop Works

Consider an AI agent responsible for monitoring a company's inventory.

| Stage | Agent Activity |
|---|---|
| Observe | Checks the current inventory records. |
| Interpret | Identifies products with stock levels below the required threshold. |
| Plan | Determines which products need replenishment. |
| Act | Creates a purchase request or initiates an authorized reorder. |
| Repeat | Checks the updated inventory status to determine whether further action is necessary. |

<escape>```mermaid
flowchart TD
    A([Start: Receive Goal]) --> B[Observe]
    B --> C[Interpret]
    C --> D[Plan]
    D --> E[Act]
    E --> F{Goal Achieved?}
    F -- No --> B
    F -- Yes --> G([Complete Task])
```</escape>

**Important:** The reasoning loop continues until the agent reaches its objective, encounters a stopping condition, or requires human intervention.

The complexity of the loop depends on the agent and its assigned task:
- **Simple agents:** May follow predefined rules and straightforward decision-making processes.
- **Advanced agents:** May use more complex reasoning, additional algorithms, and probabilistic techniques to determine appropriate actions.

### B. Tools

**Tools** are functionalities that allow AI agents to interact with their environment and perform tasks beyond generating responses.

They act as connections between the agent and external resources, systems, and services.

Examples of tools include:
- Web search tools for retrieving information.
- Database connections for accessing and updating records.
- APIs for communicating with external applications.
- Calendar applications for scheduling meetings.
- File processing tools for reading, editing, and generating documents.
- Sensors and actuators for interacting with physical devices and robots.

### Examples of How Agents Use Tools

| Tool | What the Agent Can Do |
|---|---|
| Inventory system | Access stock records and update inventory. |
| Calendar application | Check availability and schedule meetings. |
| Ordering system | Automatically request supplies when stock is low. |
| Database | Retrieve, analyze, and update information. |
| Robot sensors and actuators | Receive environmental information and execute physical movements. |

**Example: Scheduling a Meeting**

A user asks an agent:

"Schedule a meeting with the project team next week when everyone is available."

The agent can:
1. Access the calendar application.
2. Check the availability of team members.
3. Identify a suitable meeting time.
4. Create a calendar event.
5. Send meeting invitations.

Without calendar tools, a standalone language model could suggest a meeting schedule but could not independently check actual availability or create the event.

**Key distinction:** The reasoning loop helps the agent determine what to do, while tools enable it to interact with external systems and carry out the actions.

## 3. How Agents Go Beyond Standalone Language Models

Large Language Models (LLMs) are capable of understanding and generating human language, summarizing information, answering questions, and assisting with many other tasks.

However, a standalone LLM does not automatically have access to external systems or the ability to execute real-world actions.

AI agents extend these capabilities by combining models with reasoning processes and tools.

| Capability | Standalone LLM | AI Agent |
|---|---|---|
| Understand natural language | Yes | Yes |
| Generate text and explanations | Yes | Yes |
| Analyze information | Yes | Yes |
| Access external systems | Requires an integration or tool | Can use available tools and integrations |
| Execute actions | Not inherently | Yes, when authorized tools are available |
| Perform multi-step tasks | Can describe the steps | Can coordinate and execute multiple steps |
| Adapt based on action results | Not inherently | Can repeat its reasoning loop and adjust actions |

### Three Ways Agents Extend Model Capabilities

**A. Solving Complex Problems**

Agents can analyze situations, gather information through tools, and make decisions based on available results.

Example:
- An agent gathers information from several sources.
- It compares the findings.
- It identifies relevant patterns.
- It recommends or executes an appropriate action.

**B. Managing Multi-Step Tasks**

Agents can coordinate several activities that would otherwise require manual intervention.

Examples include:
- Conducting in-depth research.
- Troubleshooting programming code.
- Processing documents.
- Automating tasks across multiple applications.
- Managing business workflows.

**C. Producing Results Beyond Text and Media**

An agent can use tools to produce practical outcomes, not just generated content.

Examples:
- Updating a database.
- Creating a calendar event.
- Generating and saving a report.
- Submitting an authorized request.
- Controlling a connected robot.

**Key takeaway:** An LLM primarily provides the intelligence to understand and generate information, while an agent combines that intelligence with tools and iterative decision-making to accomplish tasks.

## 4. Advanced Prompt Engineering Frameworks

The reasoning loop can use advanced prompt engineering frameworks to guide how an agent processes information, evaluates situations, and determines its next action.

These approaches may involve:

- **Simple rule-based calculations:** Uses predefined conditions and rules to determine actions.
- **Complex thought chains:** Breaks complex problems into smaller reasoning steps.
- **Machine learning algorithms:** Uses learned patterns to support predictions and decisions.
- **Probabilistic reasoning techniques:** Evaluates possible outcomes based on probabilities and available evidence.

### Examples of Prompt Engineering Frameworks

**A. ReAct (Reason + Act)**

ReAct is a prompting framework that combines reasoning and action.

It allows an AI system to alternate between reasoning about a task and taking actions through available tools.

For example, a research agent may:
1. Determine what information is needed.
2. Search for relevant sources.
3. Examine the retrieved information.
4. Decide whether additional searches are necessary.
5. Prepare a response based on the findings.

**B. Chain-of-Thought (CoT) Prompting**

Chain-of-Thought prompting encourages a model to break a complex problem into intermediate reasoning steps before producing an answer.

For example, instead of immediately answering a mathematical problem, the model works through the relevant calculations and reaches a result.

**Important distinction:**
- ReAct combines reasoning with external actions and tool usage.
- Chain-of-Thought focuses on breaking a problem into intermediate reasoning steps.

These frameworks are discussed in greater detail in Course 5 of the learning path.

## 5. Practical Example: A Government Research Assistant Agent

Consider a generative AI agent designed to help PSRTI employees research statistical topics and prepare initial research summaries.

**Goal:** Find relevant statistical publications and prepare a summary about regional poverty indicators.

| Reasoning Loop Stage | Agent Activity | Tools Used |
|---|---|---|
| Observe | Receives the research request and identifies the information needed. | User interface |
| Interpret | Determines relevant keywords, indicators, and source requirements. | AI model |
| Plan | Develops a search and information-gathering strategy. | AI model |
| Act | Searches publications and retrieves relevant documents. | Search tool, document repository |
| Observe again | Examines retrieved documents and identifies missing information. | Document reader |
| Interpret and plan | Determines whether additional sources are needed. | AI model |
| Act | Organizes findings and generates an initial research summary. | Document processing and generation tools |
| Complete | Delivers the summary with references for human verification. | Application interface |

This example demonstrates how an agent combines an AI model, a reasoning loop, and tools to perform a multi-step research task.

Human review remains important, particularly when verifying statistical figures, source reliability, and research interpretations.

## 6. Key Takeaways

- AI agents go beyond standalone AI models by combining reasoning processes with tools.
- The **reasoning loop** is the continuous cycle of observing, interpreting, planning, and acting.
- **Tools** allow agents to access external information, interact with applications, process data, and perform actions.
- Agents can solve complex problems, coordinate multi-step workflows, and produce practical results beyond text generation.
- ReAct combines reasoning and action, while Chain-of-Thought prompting focuses on intermediate reasoning steps.
- The reasoning loop continues until the agent achieves its goal, reaches a stopping condition, or requires human intervention.

## 7. Quick Review

**1. What are the two key elements that distinguish AI agents from standalone models?**

A reasoning loop and tools.

**2. What are the four stages of the reasoning loop?**

1. Observe
2. Interpret
3. Plan
4. Act

**3. What is the purpose of the reasoning loop?**

To help an agent continuously evaluate information, plan actions, execute tasks, and adapt based on the results.

**4. What are tools in an AI agent?**

Functionalities that allow an agent to interact with external systems, information sources, applications, and devices.

**5. What is the difference between the reasoning loop and tools?**

The reasoning loop determines what the agent should do, while tools allow the agent to perform actions and interact with its environment.

**6. Why can agents handle tasks that standalone LLMs cannot independently complete?**

Because agents combine AI models with reasoning processes and tools, allowing them to gather external information, execute actions, and coordinate multi-step workflows.

**7. What is ReAct?**

A prompting framework that combines reasoning and action, allowing an AI system to use tools as part of solving a task.

**8. What is Chain-of-Thought prompting?**

A prompting approach that encourages a model to break complex problems into intermediate reasoning steps.

**9. Does an AI agent always operate without human intervention?**

No. Agents may operate autonomously within defined boundaries, but human approval or intervention may be required for sensitive, high-impact, or restricted actions.
