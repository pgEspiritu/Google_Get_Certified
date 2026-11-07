# How Agents Work

## 1. Conversational and Workflow Agents

Generative AI agents can be used in different ways depending on the tasks they are designed to perform.

Most agents fall into two major categories:

1. **Conversational agents** – Focus on understanding user requests and providing relevant responses through natural language interaction.
2. **Workflow agents** – Focus on automating tasks and executing a sequence of actions to complete a process.

Both types can use AI models, external tools, APIs, and other systems. However, they differ in their primary objectives and how they interact with users and their environment.

## 2. Conversational Agents

**Conversational agents** are designed to understand the meaning and intent behind a user's message and respond naturally.

They allow users to interact with AI through text or voice rather than relying on rigid commands or predefined menus.

### How Conversational Agents Work

The process generally involves five steps:

1. **User provides input:** The user types a message or speaks to the agent.
2. **Agent understands:** The agent processes the input and identifies the user's intent using AI.
3. **Agent calls a tool:** If additional information or an action is required, the agent may use tools such as web searches, databases, or external applications.
4. **Agent generates a response:** It formulates an answer based on the user's request and the available information.
5. **Agent delivers the response:** The answer is presented to the user through text or voice.

### Examples of Conversational Agents

**A. Answering Questions**

A user asks:

"What is the weather like in Paris?"

The agent can retrieve current weather information and provide details such as temperature, forecast, and suggested clothing.

**B. Casual Conversation**

A conversational agent can engage in informal discussions, tell jokes, recommend books or movies, and respond to everyday questions.

**C. Accessing Information**

A user asks:

"What is the capital of Australia?"

The agent provides the answer: Canberra.

It can also summarize historical events, explain technical concepts, or retrieve information from available knowledge sources.

**Key takeaway:** Conversational agents primarily focus on understanding user intent and providing relevant responses through natural language interaction.

## 3. Workflow Agents

**Workflow agents** are designed to automate tasks and execute multi-step processes efficiently.

Unlike conversational agents, which primarily focus on dialogue, workflow agents focus on getting things done by following a defined process or determining the actions needed to complete a task.

They can interact with different systems, process data, transfer files, send notifications, and execute other operations using tools and APIs.

### How Workflow Agents Work

The process generally involves five steps:

1. **User provides input:** A user defines a task or triggers a process. This may involve submitting a form, uploading a file, initiating a scheduled event, or placing an online order.
2. **Agent understands:** The agent interprets the task requirements and determines the sequence of steps needed to complete it.
3. **Agent calls tools:** The agent executes the required actions using available tools, APIs, and external systems.
4. **Agent generates a result:** It compiles the outcome, such as a report, processed data file, confirmation message, or updated status.
5. **Agent delivers the result:** The output is sent to the appropriate recipient or system, such as an email account, dashboard, database, or file storage location.

### Examples of Workflow Agents

**A. E-commerce Order Fulfillment**

A workflow agent can automate the order processing cycle:

1. Receives a customer order.
2. Checks product availability.
3. Updates inventory records.
4. Initiates shipping arrangements.
5. Sends shipping notifications.
6. Processes return requests when necessary.

**B. Customer Onboarding**

An agent can automate the process of registering and assisting new customers.

It may:
- Guide customers through account setup.
- Collect required information.
- Provide tutorials and instructions.
- Answer frequently asked questions.
- Update customer records.

**C. Automated Research**

An agent can conduct research on a specific topic by:
1. Understanding the research objective.
2. Searching relevant websites and documents.
3. Gathering and organizing information.
4. Summarizing relevant findings.
5. Generating a comprehensive report.

An example of this capability is Gemini Deep Research.

**D. Security Log Parsing**

A security agent can inspect incoming security logs to identify unusual activities.

It may:
- Analyze security logs.
- Detect and flag suspicious events.
- Open an incident ticket.
- Begin an initial investigation or triage.
- Assign the incident to human security personnel for further review.

**Key takeaway:** Workflow agents focus on executing tasks and automating processes, often involving multiple systems and actions.

## 4. Conversational Agents vs. Workflow Agents

| Aspect | Conversational Agents | Workflow Agents |
|---|---|---|
| Primary purpose | Understand and respond to user requests. | Automate tasks and complete processes. |
| Main interaction | Text or voice conversations. | Task triggers, forms, files, schedules, or system events. |
| Main activities | Understand intent, retrieve information, and generate responses. | Execute actions, process data, and coordinate multiple steps. |
| Tool usage | Retrieves information or performs actions when needed. | Uses tools and APIs to execute workflow steps. |
| Output | Answers, explanations, recommendations, or information. | Reports, processed files, notifications, confirmations, or system updates. |
| Example | Chatbot answering questions about government services. | Agent automatically processing applications and updating records. |

**Important:** These categories are not mutually exclusive. A conversational agent can trigger a workflow, while a workflow agent can use conversational AI to communicate with users.

For example, a government service chatbot may answer an applicant's questions and also initiate an application-processing workflow.

## 5. Common Agent Use Cases

Both conversational and workflow agents can support different organizational functions.

### A. Customer Service Agents

Customer service agents help organizations improve customer support and communication.

They can:
- Answer frequently asked questions.
- Resolve common customer issues.
- Provide personalized recommendations.
- Retrieve customer or service information.
- Escalate complex concerns to human representatives.

**Example:** A government service chatbot that answers questions about application requirements, processing procedures, and service availability.

### B. Employee Productivity Agents

Employee productivity agents help workers access information, manage tasks, and automate routine activities.

They can:
- Search internal documents and knowledge bases.
- Summarize reports and meeting notes.
- Organize tasks and information.
- Assist with administrative workflows.
- Retrieve information from organizational systems.

**Example:** An internal PSRTI assistant that searches research publications, training materials, and statistical references to help employees find relevant information.

### C. Creative Agents

Creative agents assist users in developing ideas and generating different types of content.

They can:
- Generate ideas and suggestions.
- Create written content.
- Develop presentation materials.
- Translate languages.
- Assist with creative brainstorming.

**Example:** An agent that helps develop initial concepts for a research forum presentation or training activity.

### D. Code Agents

Code agents assist software developers and technical teams with programming tasks.

They can:
- Generate code from natural language descriptions.
- Explain existing code.
- Review programming logic.
- Identify and troubleshoot errors.
- Suggest code improvements.

**Example:** A developer asks an agent to generate a Python script that cleans an Excel dataset by removing duplicate records and standardizing column values.

### E. Data Agents

Data agents help users analyze large datasets and extract meaningful insights.

They can:
- Query databases.
- Analyze datasets.
- Identify patterns and trends.
- Generate summaries and reports.
- Assist with data visualization and interpretation.

**Example:** A data agent analyzes CBMS-related datasets to summarize household characteristics, identify patterns in service access, and generate statistical reports.

### F. Security Agents

Security agents help automate security-related activities and support cybersecurity operations.

They can:
- Summarize security incident information.
- Research emerging threats.
- Generate security-related queries.
- Analyze suspicious activities.
- Create detection rules or initiate other security actions, subject to authorization and safeguards.

**Example:** A security agent analyzes system logs, identifies suspicious login attempts, and creates an incident ticket for investigation by the IT security team.

## 6. Summary of Agent Use Cases

| Agent Type | Primary Function | Example Application |
|---|---|---|
| Customer service agent | Answers questions and resolves customer concerns. | Government service chatbot |
| Employee productivity agent | Helps employees find information and automate tasks. | Internal document assistant |
| Creative agent | Generates ideas and creative content. | Presentation and content development |
| Code agent | Assists with programming and debugging. | Python code generation |
| Data agent | Analyzes datasets and identifies insights. | Statistical data analysis |
| Security agent | Supports threat detection and security operations. | Security log analysis and incident triage |

## 7. Key Takeaways

- Generative AI agents can be broadly categorized into conversational agents and workflow agents.
- **Conversational agents** focus on understanding user intent and responding through natural language.
- **Workflow agents** focus on automating tasks and executing multi-step processes.
- Both types can use tools, APIs, databases, and external applications.
- Conversational and workflow capabilities can be combined within a single AI solution.
- Agents can be applied to customer service, employee productivity, creative work, programming, data analysis, and cybersecurity.

## 8. Quick Review

**1. What are the two major categories of generative AI agents?**

Conversational agents and workflow agents.

**2. What is the primary purpose of conversational agents?**

To understand user intent and provide relevant responses through natural language interaction.

**3. What is the primary purpose of workflow agents?**

To automate tasks and execute multiple actions to complete a defined process.

**4. What happens when an agent calls a tool?**

It uses an available resource, such as a web search, database, API, or external application, to retrieve information or perform an action.

**5. What type of agent can automate order processing, inventory updates, and shipping notifications?**

A workflow agent.

**6. What type of agent is designed to answer questions and engage in natural language conversations?**

A conversational agent.

**7. What type of agent analyzes datasets, identifies trends, and extracts insights?**

A data agent.

**8. Can conversational agents and workflow agents work together?**

Yes. A conversational agent can understand a user's request and trigger a workflow agent to execute the required tasks.

**9. What is the difference between generating a response and executing a workflow?**

Generating a response primarily involves producing information for the user, while executing a workflow involves performing a sequence of actions to accomplish a task or update a system.
