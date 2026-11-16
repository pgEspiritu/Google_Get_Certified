
# 🧠 Prompt Engineering Techniques

## 📖 Introduction

Prompt engineering provides different techniques for guiding how Large Language Models (LLMs) reason, solve problems, and interact with their environment.

This lesson focuses on two common prompting frameworks:

1. **ReAct (Reason + Act) Prompting**
2. **Chain-of-Thought (CoT) Prompting**

## 1. 🔄 ReAct Prompting (Reason + Act)

- ReAct is a prompting framework that enables an LLM to **reason and take actions** in response to a user's query.
- It allows the model to interact with external tools and resources.
- It can work with or without in-context examples.

### 🔁 ReAct Workflow

ReAct follows a continuous **Think → Act → Observe → Respond** cycle.

| Component | Description | Example |
|---|---|---|
| 🧠 **Think** | The LLM considers the problem and determines what information or action is needed. | Find nearby Italian restaurants with good reviews. |
| ⚙️ **Act** | The LLM selects and executes an action using an available tool. | Search online for Italian restaurants in the area. |
| 👀 **Observe** | The LLM receives and evaluates feedback from the action. | Review the search results and ratings. |
| 💬 **Respond** | The LLM provides an answer, takes another action, or begins another reasoning cycle. | Recommend the best restaurant based on the user's preferences. |

**Example of an iterative ReAct process:**

1. **Think:** Find nearby Italian restaurants with good reviews.
2. **Act:** Search online for Italian restaurants.
3. **Observe:** Identify restaurants with high ratings.
4. **Think:** Determine which restaurant best matches the user's preferences.
5. **Act:** Check restaurant menus.
6. **Observe:** Review available dishes and other relevant information.
7. **Respond:** Recommend the most suitable restaurant.

### ⭐ Why Is ReAct Important?

- **Dynamic Problem Solving**
  - Handles complex tasks requiring external resources.
  - Adapts to new information gathered through interactions.

- **Reduced Hallucination**
  - Grounds responses in information retrieved from external sources.
  - Helps reduce incorrect or nonsensical answers.

- **Increased Trustworthiness**
  - Makes tool interactions and information sources more transparent.
  - Helps users understand how answers are supported by external information.

### 🧩 Key Components of ReAct

- **Think:** The LLM determines what needs to be done.
- **Act:** The LLM selects a tool and specifies the required input, such as a search query or database command.
- **Observe:** The LLM receives feedback, such as search results or database entries.
- **Respond:** The LLM provides an answer, performs another action, or continues the reasoning loop.

### 🌍 ReAct Applications

- **Question Answering:** Access external knowledge sources to answer questions more accurately.
- **Fact Verification:** Search for evidence to verify claims.
- **Decision Making:** Gather information from interactive environments to make informed decisions.

### ⚙️ How ReAct Works in an Agent

The agent prompts the model to determine its next step and generate the corresponding output, which may include:

- A thought.
- An action.
- A selected tool.
- An action input.
- An observation.

The process repeats as needed until the agent reaches its goal or stopping condition.

## 2. 🔗 Chain-of-Thought (CoT) Prompting

- Chain-of-Thought (CoT) is a prompting technique that guides an LLM through a problem-solving process using intermediate reasoning steps.
- It helps the model approach unfamiliar problems in a more structured and logical way.
- Examples of similar problems and their intermediate steps can be provided to guide the model.

**Concept:** Instead of asking an LLM to produce an answer immediately, CoT encourages a structured approach to solving the problem.

### ⭐ Why Is CoT Important?

- **Improved Reasoning**
  - Helps LLMs solve complex problems requiring logical thinking.

- **Better Accuracy**
  - Breaks complex problems into smaller, manageable steps.
  - Can improve the quality of solutions.

- **Enhanced Explainability**
  - Structured explanations can help users understand how an answer was developed.
  - Makes it easier to identify potential errors.

### 🧩 Key Components and Techniques of CoT

Some popular techniques include:

- **Self-Consistency**
  - Encourages the LLM to generate multiple possible solutions.
  - Selects the answer that is most consistent across the generated solutions.

- **Active-Prompting**
  - Allows the LLM to ask clarifying questions or request additional information.
  - Helps address missing or unclear details.

- **Multimodal CoT**
  - Combines text with other forms of data, such as images and videos.
  - Provides additional information to support reasoning.

### 🌍 CoT Applications

- **Complex Reasoning Tasks**
  - Breaks complicated problems into smaller steps.
  - Useful for mathematics, word problems, and logical reasoning puzzles.

- **Explanation Generation**
  - Produces structured explanations for answers.
  - Helps users understand results and identify potential errors.

- **Multi-Step Planning**
  - Supports planning and execution of tasks involving multiple steps.
  - Examples include:
    - Writing a story.
    - Planning a trip.
    - Debugging code.

## 3. ⚖️ Choosing a Prompting Framework

The best prompting framework depends on the task and intended use case.

### ReAct vs. Chain-of-Thought

| Attribute | ReAct | Chain-of-Thought (CoT) |
|---|---|---|
| **Primary Focus** | Reasoning and external actions | Internal problem-solving and reasoning |
| **Approach** | Think → Act → Observe → Respond | Break a problem into intermediate reasoning steps |
| **External Tools** | Uses tools such as search engines, APIs, and databases | Does not inherently require external tools |
| **Main Purpose** | Interact with the environment and gather information | Solve complex problems through structured reasoning |
| **Common Applications** | Question answering, fact verification, decision-making | Mathematics, logical reasoning, explanations, multi-step planning |

### 🤝 Combining ReAct and CoT

- ReAct and CoT are not mutually exclusive.
- They can be combined to create more capable AI agents.
- **CoT** supports structured reasoning and problem-solving.
- **ReAct** enables the agent to interact with external tools and gather real-world information.

Combining both techniques allows an agent to:
- Reason through complex problems.
- Plan the necessary steps.
- Access external information.
- Take actions using available tools.
- Evaluate results and adjust its next actions.

## 🔑 Key Takeaways

- **ReAct** combines reasoning with actions and observations, enabling LLMs to interact with external tools.
- **CoT** guides LLMs through intermediate reasoning steps to solve complex problems.
- ReAct follows the cycle: **Think → Act → Observe → Respond**.
- CoT techniques include **Self-Consistency, Active-Prompting, and Multimodal CoT**.
- ReAct is particularly useful when tasks require external information or interaction.
- CoT is useful when tasks require structured reasoning and problem-solving.
- Combining ReAct and CoT can create agents capable of both deeper reasoning and dynamic interaction with the environment.

💡 **Remember:**
- **CoT = Think through the problem.**
- **ReAct = Think, take action, observe results, and respond.**
