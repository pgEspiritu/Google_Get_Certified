

# 🧩 Gen AI Project Resources: People, Cost, and Time

## 🎯 1. Introduction

Building a successful Generative AI (Gen AI) solution requires more than selecting the right model or technology. Organizations must also consider the resources needed to develop, deploy, and maintain the solution.

Three important resources must be considered when planning a Gen AI project:

- 👥 **People:** The skills, expertise, and roles required to build and manage the solution.
- 💰 **Cost:** The financial resources needed for training, deployment, and model usage.
- ⏱️ **Time:** The development timeline required to deliver the solution.

Understanding these factors helps organizations determine whether a proposed Gen AI project is feasible, affordable, and aligned with their objectives.

## 👥 2. Roles and Responsibilities

The AI technology stack supports different organizational roles, each with specific responsibilities and technical requirements.

Before developing a Gen AI solution, organizations should assess whether they have the appropriate expertise and talent to implement and maintain it.

Three major groups contribute to the development and adoption of Gen AI:

### 2.1 Business Users and Leaders

Business users and leaders typically interact with **pre-built Gen AI solutions** to improve daily operations, productivity, and customer experiences.

**Primary responsibilities:**
- Identify business problems that Gen AI can help address.
- Use existing AI-powered applications to improve workflows.
- Apply Gen AI to content creation, data analysis, and document summarization.
- Identify opportunities to improve customer experiences and organizational efficiency.

**Example tools:**
- **Google Workspace with Gemini:** Helps users create content, analyze information, summarize documents, and improve productivity.

💡 **Key idea:** Business users primarily leverage existing AI solutions rather than building complex AI systems from scratch.

### 2.2 Developers

Developers are responsible for building and deploying custom AI-powered applications and agents.

They integrate AI capabilities into existing systems or develop new applications that address specific organizational needs.

**Primary responsibilities:**
- Build and deploy custom AI agents.
- Integrate AI capabilities into existing applications.
- Develop AI-powered workflows and automation.
- Use pre-trained APIs to add AI features quickly.
- Connect AI applications with databases, tools, and external services.

**Example tools and platforms:**

- **AI Applications:** Supports custom agent creation, AI-assisted code generation, and AI-driven data processing.
- **Pre-trained APIs:** Allow developers to integrate existing AI capabilities into applications without training models from scratch.
- **Agent Platform:** Provides tools for building and deploying AI agents, including orchestration, grounding, and action capabilities.

💡 **Key idea:** Developers focus on building, integrating, and deploying AI-powered applications and agents.

### 2.3 AI Practitioners

AI practitioners have specialized expertise in developing, customizing, deploying, and optimizing AI and machine learning models.

They work on more technically complex aspects of AI implementation.

**Primary responsibilities:**
- Customize and optimize generative AI models.
- Train, evaluate, and deploy AI models.
- Scale AI workloads to support organizational requirements.
- Integrate models with data platforms such as BigQuery.
- Implement responsible AI practices.
- Conduct bias detection and adversarial testing.
- Monitor model performance and reliability.

**Example tools and platforms:**

- **Agent Platform:** Supports model development, training, evaluation, deployment, and MLOps.
- **BigQuery:** Supports large-scale data analysis and integration with AI workloads.

💡 **Key idea:** AI practitioners focus on the technical development, optimization, and responsible deployment of AI models.

### 📊 2.4 Comparison of Roles

| Role | Primary Focus | Typical Activities |
|---|---|---|
| 👔 Business Users / Leaders | Business productivity and adoption | Using pre-built AI tools, identifying use cases, improving workflows |
| 💻 Developers | Application and agent development | Building custom agents, integrating APIs, deploying applications |
| 🧠 AI Practitioners | Model development and optimization | Training, fine-tuning, evaluating, monitoring, and securing models |

### 🤝 2.5 Why Collaboration Matters

These roles work together to maximize the value of AI across an organization.

For example, when developing an AI-powered government research assistant:

1. 👔 **Business users** identify the need for a tool that helps employees search and summarize research documents.
2. 💻 **Developers** build the application and integrate it with document repositories and AI services.
3. 🧠 **AI practitioners** evaluate model performance, improve responses, and implement safeguards against bias and inaccurate outputs.

The result is a solution that addresses an actual business need while meeting technical and responsible AI requirements.

## 💰 3. Understanding Gen AI Project Costs

The pricing model for Gen AI varies depending on the technology, service, provider, and deployment approach.

Organizations should establish a realistic budget before starting a project because costs can arise throughout the AI lifecycle.

### 3.1 Three Primary Cost Activities

When building and operating Gen AI solutions, organizations generally incur costs from three major activities:

#### 🏋️ A. Model Training

Training involves using data and computing resources to teach a model to recognize patterns and perform specific tasks.

Potential costs include:
- Compute resources used during training.
- Storage for training datasets.
- Storage for model outputs, checkpoints, and artifacts.
- Data preparation and processing.

#### ☁️ B. Model Deployment

Deployment involves making a trained model available through an endpoint or another serving environment so applications and users can access it.

Potential costs include:
- Computing resources for hosting and serving models.
- Storage for model files and related resources.
- Infrastructure and networking.
- Scaling resources based on demand.

#### 🔮 C. Model Usage and Predictions

Once deployed, a model incurs costs when users or applications send requests and receive predictions or generated outputs.

Potential costs include:
- Input and output tokens.
- Characters processed.
- Number of requests.
- Compute time used to process requests.

💡 **Remember:** Training, deployment, and usage are three distinct activities that may contribute to the total cost of a Gen AI project.

## 💳 4. Pricing Models for Using Gen AI Models

AI providers use different pricing approaches depending on their products and services.

### 4.1 Usage-Based Pricing

You pay according to the amount of service consumed.

Common pricing measurements include:
- Tokens processed.
- Characters processed.
- Number of requests.
- Compute resources or processing time.

**Example:** An application using a Gemini API may incur charges based on the number of input and output tokens processed.

### 4.2 Subscription-Based Pricing

You pay a recurring fee, usually monthly or annually, to access a service.

Subscription plans may differ based on:
- Usage limits.
- Available features.
- Number of users.
- Service capabilities.

**Example:** An organization subscribes to an AI-powered productivity service with different plans for individual users and enterprise customers.

### 4.3 Licensing Fees

You pay a one-time or recurring fee for permission to use a model or software under specific licensing terms.

Licensing may apply when:
- Using a model commercially.
- Embedding a model into a commercial product.
- Redistributing or deploying a model under specific terms.

**Example:** A company obtains a commercial license to incorporate a proprietary AI model into its software product.

### 4.4 Free Tiers

Some providers offer limited free access for experimentation, development, or personal use.

Free tiers may include:
- Limited API requests.
- Restricted token usage.
- Limited access to model features.
- Usage restrictions or non-commercial conditions.

**Example:** A developer uses a provider's free API quota to test an AI-powered prototype before moving to a paid plan.

### 📊 4.5 Pricing Model Comparison

| Pricing Model | How You Pay | Common Use Case |
|---|---|---|
| 💳 Usage-Based | Based on actual consumption | AI APIs and model inference |
| 📅 Subscription-Based | Recurring monthly or annual fee | AI productivity applications |
| 📜 Licensing Fees | One-time or recurring license fee | Commercial model integration |
| 🆓 Free Tier | No charge within defined limits | Experimentation and prototyping |

## 📏 5. Pricing Metrics for Using Models

For usage-based pricing, providers may use different measurements to determine how much a customer pays.

### 5.1 Tokens

A **token** represents a piece of text processed by a language model. It may be a complete word, part of a word, punctuation mark, or other text unit.

For example, a sentence is divided into multiple tokens before being processed by an LLM.

**Why it matters:**
- Input tokens represent the text sent to the model.
- Output tokens represent the text generated by the model.
- Some providers charge separately for input and output tokens.

**Example:** A user submits a long research document and asks an AI model to summarize it. The document contributes to input token usage, while the generated summary contributes to output token usage.

### 5.2 Characters

Some AI services calculate charges based on the number of characters processed.

This is common in certain language, translation, and text-processing services.

**Example:** A translation service processes 10,000 characters of text and calculates the cost based on its character-based pricing rate.

### 5.3 Requests

Some services charge based on the number of API requests made, regardless of the amount of content processed in each request.

**Example:** An application sends 1,000 individual requests to an AI service, and the provider charges based on the total number of requests.

### 5.4 Compute Time

Compute time refers to the amount of processing time or computing resources consumed when executing a task.

This may affect costs, particularly for resource-intensive workloads.

**Example:** A company runs a large AI model on cloud infrastructure for several hours to process a large dataset.

### 📊 5.5 Comparison of Pricing Metrics

| Metric | What Is Measured | Example |
|---|---|---|
| 🔤 Tokens | Text units processed | Input and output tokens in an LLM |
| 🔠 Characters | Number of characters processed | Translation or text-processing services |
| 📩 Requests | Number of service calls | API requests made by an application |
| ⚙️ Compute Time | Processing time or computing resources consumed | Running an AI model on cloud infrastructure |

## 📈 6. Factors Affecting Gen AI Costs

The total cost of using an AI model depends on several factors.

### 6.1 Model Size and Complexity

Larger and more capable models generally require more computing resources and may have higher usage costs.

Factors include:
- Model architecture and size.
- Computational requirements.
- Model capabilities.
- Complexity of the requested tasks.

**Example:** A complex reasoning task may require a more capable model than a simple text classification task.

💡 **Tip:** Choose a model based on the requirements of the task. A larger model is not always necessary.

### 6.2 Context Window

The **context window** refers to the amount of information, usually measured in tokens, that a model can consider during a single interaction.

A larger context window allows a model to process longer prompts, documents, and conversation histories.

However:
- More input tokens can increase usage-based costs.
- Longer conversations may require more context to be processed.
- A larger context window does not automatically guarantee better responses.

**Example:** Summarizing a 200-page research report may require more input tokens than summarizing a one-page document.

### 6.3 Features

Specialized model capabilities and additional services may have separate pricing.

Examples include:
- Fine-tuning.
- Text embeddings.
- Image generation.
- Audio processing.
- Advanced model capabilities.
- Additional data processing services.

**Example:** An organization may incur additional charges when generating vector embeddings for thousands of documents to support semantic search.

### 6.4 Deployment

The deployment environment can also affect project costs.

Potential expenses include:
- Cloud computing resources.
- Model hosting and serving.
- Storage.
- Networking.
- Container infrastructure.
- Monitoring and maintenance.

**Example:** Hosting an AI model on a cloud virtual machine may incur ongoing infrastructure costs even when the application receives relatively few requests.

### 📊 6.5 Summary of Cost Factors

| Factor | How It Affects Cost |
|---|---|
| 🧠 Model Size and Complexity | More capable models may require more computing resources. |
| 📚 Context Window | Processing more tokens can increase usage costs. |
| 🛠️ Features | Specialized capabilities may have additional charges. |
| ☁️ Deployment | Hosting, compute, storage, and networking contribute to operating expenses. |

## ⏱️ 7. Time Requirements for Gen AI Projects

The time required to develop a Gen AI solution depends on its complexity, customization requirements, available resources, and technical expertise.

Generally, **the more customized a solution is, the more time and resources it may require.**

### 7.1 Pre-built Gen AI Applications

<badge color="success">Fastest to adopt</badge>

Using an existing Gen AI application requires little to no development.

**Examples:**
- Using Gemini to summarize documents.
- Using Google Workspace with Gemini to draft emails.
- Using an existing AI assistant for research or content generation.

**Typical timeline:** Seconds to minutes for initial use, depending on setup and access requirements.

### 7.2 Custom AI Agents

<badge color="info">Moderate development effort</badge>

Building a custom AI agent requires configuring its instructions, tools, knowledge sources, and workflows.

**Examples:**
- An AI agent that searches internal documents.
- A customer service agent that retrieves information from a database.
- A research assistant that summarizes reports and generates references.

**Typical timeline:** Can range from days to weeks or longer, depending on integrations, testing, and complexity.

### 7.3 Custom AI Models

<badge color="warning">Highest development effort</badge>

Developing a custom AI model requires more extensive technical work and resources.

Activities may include:
- Collecting and preparing datasets.
- Selecting model architectures.
- Training and tuning models.
- Evaluating model performance.
- Deploying and monitoring the model.
- Implementing security and responsible AI safeguards.

**Typical timeline:** May take weeks to months or longer, depending on the model, dataset, and project requirements.

### 📊 7.4 Comparing Development Time

| Approach | Development Effort | General Timeline | Example |
|---|---|---|---|
| 🧩 Pre-built Gen AI Application | Low | Seconds to minutes for initial use | Using Gemini to summarize a document |
| 🤖 Custom AI Agent | Moderate | Days to weeks or longer | Building an internal research assistant |
| 🧠 Custom AI Model | High | Weeks to months or longer | Training a specialized predictive model |

*These timelines are illustrative, not fixed estimates. Actual project duration depends on scope, resources, integrations, testing, and deployment requirements.*

## 🏛️ 8. Example: Planning a Gen AI Project in a Government Agency

Imagine a government agency wants to develop an AI-powered research assistant that helps employees search, summarize, and retrieve information from internal reports and statistical publications.

Before starting, the agency should assess its available people, budget, and time.

### 👥 People

| Role | Responsibility |
|---|---|
| Business Users / Researchers | Identify requirements and evaluate whether outputs are useful. |
| Developers | Build the application, integrate document repositories, and configure agent workflows. |
| AI Practitioners | Evaluate models, configure grounding or RAG, and implement responsible AI safeguards. |
| Project Manager | Coordinate activities, resources, deliverables, and timelines. |

### 💰 Cost

Potential expenses include:
- AI model API usage.
- Cloud storage for research documents.
- Computing resources for deployment.
- Embedding generation and semantic search.
- Security, monitoring, and maintenance.

### ⏱️ Time

The agency could begin with a pre-built Gen AI application for an initial proof of concept, then develop a custom agent if the initial results demonstrate value.

A fully customized model should only be considered if existing models and approaches cannot adequately meet the agency's requirements.

### 💡 Recommended Approach

Start with the simplest solution that meets the requirements.

1. Identify the actual problem and expected outcomes.
2. Evaluate available pre-built Gen AI tools.
3. Build a small proof of concept.
4. Assess performance, cost, and user feedback.
5. Develop a custom agent or model only when necessary.
6. Establish ongoing monitoring and responsible AI controls.

## 💡 9. Key Takeaways

- 👥 **People:** Gen AI projects require different skill sets. Business users identify needs and use AI tools, developers build applications and agents, and AI practitioners develop and optimize models.
- 💰 **Cost:** Three primary cost activities are model training, deployment, and usage.
- 💳 **Pricing Models:** Providers may use usage-based pricing, subscriptions, licensing fees, or free tiers.
- 📏 **Pricing Metrics:** Common measurements include tokens, characters, requests, and compute time.
- 📈 **Cost Factors:** Model size, context window, specialized features, and deployment requirements affect total costs.
- ⏱️ **Time:** Pre-built applications are generally the fastest to adopt, while custom agents and models require progressively more development effort.
- 🎯 **Project Planning:** Evaluate people, cost, and time against the project's actual requirements before selecting a solution.

## 📝 10. Quick Review Questions

**1. What are the three major resources to consider when planning a Gen AI project?**

- 👥 People
- 💰 Cost
- ⏱️ Time

**2. Who typically uses pre-built Gen AI applications to improve business operations?**

Business users and leaders.

**3. Who builds and deploys custom AI agents and integrates AI into existing applications?**

Developers.

**4. Who specializes in customizing, training, evaluating, and optimizing AI models?**

AI practitioners.

**5. What are the three primary cost activities in a Gen AI project?**

- Model training.
- Model deployment.
- Model usage and predictions.

**6. What is usage-based pricing?**

A pricing approach where customers pay according to the amount of service consumed, such as tokens, characters, requests, or compute resources.

**7. What is the difference between subscription-based pricing and licensing fees?**

Subscription-based pricing involves recurring payments for access to a service, while licensing fees provide permission to use a model or software under specified terms.

**8. What is a token?**

A unit of text processed by a language model. It may represent a complete word, part of a word, or punctuation.

**9. What are four factors that affect Gen AI model costs?**

- Model size and complexity.
- Context window.
- Features.
- Deployment.

**10. Which approach generally takes the least time to implement?**

Using a pre-built Gen AI application.

**11. Why does a custom AI model generally require more time and resources?**

It may require data collection, preparation, model selection, training, tuning, evaluation, deployment, and monitoring.

**12. What should an organization do before building a custom Gen AI solution?**

Assess its requirements, available expertise, budget, and project timeline, then determine whether an existing solution can already meet its needs.

