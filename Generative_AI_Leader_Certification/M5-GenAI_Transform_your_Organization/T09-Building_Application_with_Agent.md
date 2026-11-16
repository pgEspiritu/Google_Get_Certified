
# 🏗️ Building Applications from Your Agents

## 1. Introduction
- Generative AI agents can be integrated into applications using:
  - **Gemini API** with default settings.
  - **Customized Gemini models** using parameters configured in Google AI Studio.
- Developers can use APIs and generated code to incorporate AI capabilities into their own applications.

## 2. Using the Gemini API

### 🔑 Getting API Access
Two primary options are presented:

| Platform | Purpose | Documentation |
|---|---|---|
| **Google AI Studio** | Generate an API key and use the Gemini API in applications. | [Gemini API Quickstart](https://ai.google.dev/gemini-api/docs/quickstart?lang=python) |
| **Agent Studio** | Send text prompts to Gemini through the Google Cloud agent development environment. | [Agent Studio Quickstart](https://docs.cloud.google.com/gemini-enterprise-agent-platform/agent-studio/quickstart) |

### 🚀 Application Integration Options

Once you have an API key or application code, you can integrate the agent into different environments:

- **Cloud Run functions**
  - Run event-driven serverless functions.
  - Connect Gemini API calls to application workflows.
- **Cloud Run**
  - Deploy applications and services in serverless containers.
  - Host more complex applications that use generative AI.
- **HTTP-based applications**
  - The Gemini API can be integrated into virtually any application capable of making HTTP requests.
  - Examples:
    - Web applications
    - Mobile applications
    - Desktop software
    - Embedded systems

### 🧩 No-Code and Low-Code Integration

Google also provides tools for incorporating AI capabilities with less manual coding:

| Tool | Purpose |
|---|---|
| **Apps Script** | Automate and extend Google Workspace applications using scripts and APIs. |
| **AppSheet** | Build no-code or low-code applications that can incorporate AI-powered workflows. |

## 3. 🤖 Multi-Agent Applications

### What Are Multi-Agent Systems?
- Applications that use **multiple specialized AI agents**, each responsible for a particular task.
- Agents can:
  - Work independently on assigned tasks.
  - Communicate or interact with other agents.
  - Coordinate activities to complete a larger objective.
- An agent can also function as a **tool within another agent**.

### Example: Travel Booking Application

A travel booking application can use multiple agents:

| Agent | Responsibility |
|---|---|
| ✈️ Flight Agent | Searches for available flights. |
| 🏨 Hotel Agent | Finds suitable hotels. |
| 📍 Attractions Agent | Recommends local attractions and activities. |

These agents work together to provide a seamless travel-planning experience.

### Example: Customer Service Application
- **Customer Service Agent:** Handles customer conversations and inquiries.
- **Sentiment Analysis Agent:** Evaluates customer sentiment and satisfaction.
- The customer service agent can use the sentiment analysis agent as a tool to understand the customer's feelings and improve its responses.

### Benefits of Multi-Agent Systems
- **Specialization:** Each agent focuses on a specific task.
- **Efficiency:** Tasks can be distributed among agents.
- **Flexibility:** Agents can operate independently or collaborate.
- **Scalability:** Additional specialized agents can be integrated as application requirements grow.
- **Modularity:** Individual agents can be improved or replaced without redesigning the entire application.

## 4. 🔑 Key Takeaways

- Generative AI can be integrated into applications through APIs and application code.
- **Cloud Run functions** and **Cloud Run** provide deployment and execution options for AI-powered workflows.
- **Apps Script** and **AppSheet** offer no-code and low-code integration possibilities.
- The Gemini API can support web, mobile, desktop, and embedded applications that can make HTTP requests.
- **Multi-agent systems** improve application capabilities by assigning specialized tasks to different agents.
- An agent can also serve as a tool for another agent.

### 🧠 Overall Concept

| Component | Role |
|---|---|
| Gemini API / Agent Studio | Provides access to generative AI models. |
| Application integration | Connects AI capabilities to applications and workflows. |
| Cloud Run / Cloud Run functions | Runs and deploys AI-powered application components. |
| Apps Script / AppSheet | Enables low-code and no-code integration. |
| Multi-agent system | Coordinates specialized agents to accomplish complex tasks. |

**Remember:** APIs connect AI models to applications, cloud services support deployment, and multi-agent systems allow specialized agents to collaborate on complex tasks.
