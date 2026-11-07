# Techniques to Overcome Foundation Model Limitations

## 1. Introduction

Previously, we explored common limitations of foundation models, including hallucinations, bias, knowledge cutoffs, and edge cases.

Several techniques can help address these challenges and improve the reliability, accuracy, and usefulness of generative AI applications.

The key approaches covered in this lesson are:

1. Grounding
2. Retrieval-Augmented Generation (RAG)
3. Prompt Engineering
4. Fine-Tuning
5. Humans in the Loop (HITL)

Each technique addresses different aspects of model performance. They can also be combined depending on the application's requirements.

## 2. Grounding

Generative AI models can produce creative and useful content, but they may sometimes generate information that is inaccurate or fabricated.

**Grounding** is the process of connecting an AI model's responses to verifiable sources of information. It provides additional context and evidence to help ensure that generated responses are based on relevant, real-world information.

Think of grounding as giving an AI model a reference material or a reality check before it answers a question.

### How Grounding Works

Instead of relying exclusively on information learned during training, an AI application can provide access to specific and trusted data sources.

Examples include:
- Enterprise documents and internal reports.
- Organizational policies and procedures.
- Databases and knowledge repositories.
- Official government publications.
- Updated statistical datasets.
- Google Search results.

**Example:**

Suppose an employee asks an AI assistant:

> What are the requirements for processing a business permit?

Without grounding, the model may provide a generic answer based on its existing knowledge, which might not reflect the latest local government requirements.

With grounding, the AI can reference the LGU's official business permit guidelines and use those documents to formulate its response.

### Benefits of Grounding

| Benefit | Explanation |
|---|---|
| Reduces hallucinations | Helps prevent the model from generating fabricated or unsupported information. |
| Anchors responses | Connects answers to relevant information from provided data sources. |
| Improves relevance | Enables the model to provide organization-specific answers instead of generic responses. |
| Builds trust | Allows users to verify answers through citations and supporting references when available. |

Grounding may also provide citations or confidence-related information, depending on the tools and implementation. However, citations and confidence scores do not automatically guarantee correctness.

> **Key takeaway:** Grounding helps make AI responses more accurate and relevant by connecting them to reliable information sources.

## 3. Retrieval-Augmented Generation (RAG)

One common method of grounding generative AI models is **Retrieval-Augmented Generation (RAG)**.

RAG is a technique that retrieves relevant information from an external knowledge base and provides it to a large language model (LLM) as additional context when generating a response.

Instead of relying only on the model's existing knowledge, RAG allows the AI application to search for relevant information before answering a question.

### How RAG Works

RAG generally follows three main stages:

<text weight="semibold" color="default">1. Retrieval</text>

When a user submits a question, the system searches a knowledge base for relevant information.

The search process may use semantic search, which identifies information based on meaning and context rather than relying only on exact keyword matches.

For example, searching for:

> How can an employee request vacation leave?

May retrieve a document containing:

> Procedures for filing an application for leave.

Although the wording is different, the search system recognizes that the two statements are related.

<text weight="semibold" color="default">2. Augmentation</text>

The retrieved information is added to the prompt or context provided to the LLM.

This gives the model relevant reference material that it can use when preparing its response.

<text weight="semibold" color="default">3. Generation</text>

The LLM processes the user's original question together with the retrieved information and generates a response based on the additional context.

### RAG Workflow

<box border radius="lg" padding={3} gap={3}>
  <box background="rgba(59,130,246,0.10)" radius="md" padding={3} align="center">
    **User Question**

    <text color="secondary" size="sm">"What is the procedure for filing leave?"</text>
  </box>
  <box align="center">
    <icon name="arrow-down" color="secondary" size="lg"/>
  </box>
  <box background="rgba(16,185,129,0.10)" radius="md" padding={3} align="center">
    **1. Retrieval**

    <text color="secondary" size="sm">Searches the knowledge base for relevant leave policies and procedures.</text>
  </box>
  <box align="center">
    <icon name="arrow-down" color="secondary" size="lg"/>
  </box>
  <box background="rgba(245,158,11,0.10)" radius="md" padding={3} align="center">
    **2. Augmentation**

    <text color="secondary" size="sm">Adds retrieved policy documents to the model's prompt as context.</text>
  </box>
  <box align="center">
    <icon name="arrow-down" color="secondary" size="lg"/>
  </box>
  <box background="rgba(139,92,246,0.10)" radius="md" padding={3} align="center">
    **3. Generation**

    <text color="secondary" size="sm">The LLM uses the question and retrieved information to formulate an answer.</text>
  </box>
  <box align="center">
    <icon name="arrow-down" color="secondary" size="lg"/>
  </box>
  <box background="rgba(16,185,129,0.10)" radius="md" padding={3} align="center">
    **Grounded Response**

    <text color="secondary" size="sm">Provides the leave procedure based on the available policy documents.</text>
  </box>
</box>

### Example Applications of RAG

- **Government policy assistant:** Retrieves official government circulars, memoranda, and guidelines to answer employee inquiries.
- **Research assistant:** Searches institutional research papers, reports, and statistical publications.
- **Customer support chatbot:** Retrieves product manuals, FAQs, and service documentation.
- **Human resource assistant:** Searches employee handbooks and organizational policies.

### Important Characteristics of RAG

- It provides access to information outside the model's original training data.
- It can use updated information without requiring the model to be retrained every time a document changes.
- It can improve response relevance by supplying context specific to the user's question.
- Its effectiveness depends on the quality of the knowledge base and retrieval process.

> **Key takeaway:** RAG combines information retrieval with generative AI. It searches for relevant information, adds that information to the model's context, and then generates a response.

## 4. Prompt Engineering

**Prompt engineering** is the process of designing and refining instructions or inputs to guide a generative AI model toward a desired output.

It is one of the quickest and simplest ways to provide supplementary background information and improve the relevance of generated responses.

A prompt can include:
- Instructions about what the model should do.
- Background information and context.
- The user's question or task.
- Examples of the desired output.
- Formatting requirements and constraints.

### Example

**Basic prompt:**

> Explain data quality.

**Improved prompt:**

> Explain the five dimensions of data quality: accuracy, completeness, consistency, relevance, and representativeness. Use simple language and provide examples related to government statistical data.

The second prompt provides more context and clearer instructions, helping the model produce a more targeted response.

### Limitations of Prompt Engineering

Although prompt engineering can improve responses, it has limitations:

- It depends on the model's existing knowledge and capabilities.
- It cannot reliably provide information the model does not know.
- It does not automatically update the model's training data.
- Poorly written or ambiguous prompts may produce irrelevant responses.
- It cannot guarantee that generated information is accurate.

For example, asking a model to provide the latest 2026 government statistics will not guarantee an accurate answer if the model does not have access to updated data.

In such cases, grounding or RAG may be more appropriate.

> **Key takeaway:** Prompt engineering improves how we communicate with AI models, but it cannot independently solve limitations involving missing or outdated knowledge.

## 5. Fine-Tuning

When prompt engineering alone does not produce the desired results, **fine-tuning** can help improve a model's performance for specialized tasks.

Foundation models are generally designed for broad applications. Fine-tuning allows an existing pre-trained model to become more specialized by training it further using a dataset specific to a particular task or domain.

### How Fine-Tuning Works

Fine-tuning involves:

1. Starting with an existing pre-trained or foundation model.
2. Preparing a specialized dataset containing examples relevant to the intended task.
3. Further training the model using the prepared dataset.
4. Adjusting the model's parameters based on the additional training.
5. Evaluating the fine-tuned model to determine whether its performance has improved.

Unlike prompt engineering, which changes the instructions given to a model, fine-tuning modifies the model through additional training.

### Examples of Fine-Tuning

| Application | Example |
|---|---|
| Creative writing | Fine-tune a language model to generate content using a specific writing style. |
| Code generation | Fine-tune a code generation model to produce code in a particular programming language or follow specific coding conventions. |
| Translation | Fine-tune a translation model to handle specialized terminology or particular language domains. |
| Document classification | Fine-tune a model to classify government documents into predefined categories. |

### When Is Fine-Tuning Useful?

Fine-tuning is particularly useful when:
- A model needs to perform a specialized or repetitive task.
- A consistent output format or style is required.
- The organization has sufficient examples of the desired outputs.
- Prompt engineering alone does not consistently produce the required results.

### Fine-Tuning vs. Prompt Engineering vs. RAG

| Technique | How It Works | Main Purpose |
|---|---|---|
| Prompt Engineering | Provides instructions and context through prompts. | Guides the model's behavior and output. |
| RAG | Retrieves external information and adds it to the model's context. | Provides relevant and potentially updated knowledge. |
| Fine-Tuning | Further trains an existing model using specialized data. | Adapts the model to specific tasks, styles, or patterns. |

**Practical example:**

Imagine PSRTI wants to develop an AI assistant for preparing statistical research summaries.

- **Prompt engineering:** Instruct the AI to summarize research findings using a standard format.
- **RAG:** Allow the AI to retrieve relevant PSRTI research reports, statistical publications, and methodological references.
- **Fine-tuning:** Further train a model using approved examples of research summaries to encourage consistent writing style and structure.

These techniques can also be combined in one AI application.

> **Important:** Fine-tuning is not always the best solution for adding new factual information. When the primary requirement is access to updated documents or knowledge, RAG is often more suitable.

## 6. Humans in the Loop (HITL)

Beyond technical approaches such as grounding, RAG, prompt engineering, and fine-tuning, human expertise remains essential in the development and deployment of AI systems.

**Humans in the Loop (HITL)** refers to an approach in which people provide input, review, feedback, or decisions as part of the machine learning process.

Although AI models can process large amounts of information and automate repetitive tasks, they may still struggle with situations requiring human judgment, specialized knowledge, contextual understanding, or ethical considerations.

HITL combines machine capabilities with human expertise to improve the quality, reliability, and accountability of AI applications.

### Applications of HITL

#### 6.1 Content Moderation

HITL helps ensure that user-generated content is reviewed accurately and appropriately.

Automated moderation systems may detect harmful or inappropriate material, but some content requires human interpretation to understand its context.

**Example:** A human moderator reviews content flagged by an AI system to determine whether it actually violates community guidelines.

#### 6.2 Sensitive Applications

In sensitive fields such as healthcare and finance, human oversight is important because errors can have significant consequences.

**Examples:**
- Healthcare professionals reviewing AI-generated medical recommendations.
- Financial analysts validating AI-generated risk assessments.
- Government personnel checking AI-assisted eligibility assessments.

#### 6.3 High-Risk Decision-Making

When AI systems support decisions with significant consequences, human review provides an additional safeguard.

**Examples:**
- Medical diagnosis and treatment decisions.
- Criminal justice assessments.
- Public assistance eligibility and resource allocation.

AI should support qualified decision-makers rather than independently determine outcomes in high-risk situations without appropriate safeguards.

#### 6.4 Pre-Generation Review

Human experts can review information, instructions, and inputs before AI-generated content or decisions are released.

This helps identify potential problems before they affect users.

**Example:** A research officer checks the source data and instructions before using AI to generate a statistical report.

#### 6.5 Post-Generation Review

Human review continues after the AI system produces or deploys its outputs.

Feedback can help identify recurring errors, biases, and areas requiring improvement.

**Example:** A statistical researcher checks AI-generated interpretations against official datasets and provides feedback when the model misinterprets a statistical indicator.

### Summary of HITL Applications

| Application | Role of Human Oversight |
|---|---|
| Content moderation | Reviews flagged content and interprets context. |
| Sensitive applications | Checks AI outputs in areas such as healthcare and finance. |
| High-risk decision-making | Provides review, accountability, and safeguards. |
| Pre-generation review | Validates inputs and instructions before outputs are generated or released. |
| Post-generation review | Evaluates outputs and provides feedback for continuous improvement. |

> **Key takeaway:** HITL ensures that AI does not operate without appropriate human oversight, particularly when accuracy, fairness, safety, and accountability are important.

## 7. Comparing Techniques to Overcome Foundation Model Limitations

| Technique | Primary Function | What It Helps Address |
|---|---|---|
| Grounding | Connects AI responses to reliable information sources. | Hallucinations and irrelevant answers |
| RAG | Retrieves relevant external information and supplies it as context. | Knowledge gaps and outdated information |
| Prompt Engineering | Provides clear instructions and supplementary context. | Ambiguous instructions and inconsistent outputs |
| Fine-Tuning | Further trains a model using specialized examples. | Task-specific performance and output consistency |
| Humans in the Loop | Integrates human review, judgment, and feedback. | Errors, bias, fairness, and high-risk decisions |

## 8. Practical Application: Building a Government AI Research Assistant

Imagine a government statistical institution wants to develop an AI assistant to help researchers find information, summarize reports, and prepare initial research drafts.

The following techniques can work together:

| Technique | Possible Implementation |
|---|---|
| Grounding | Connect the AI assistant to official statistical publications and institutional references. |
| RAG | Retrieve relevant sections from research papers, reports, and methodological documents based on user questions. |
| Prompt Engineering | Instruct the assistant to use formal research language, cite references, and follow a prescribed summary format. |
| Fine-Tuning | Adapt a model using approved examples of institutional research summaries, if consistent specialized behavior is needed. |
| Humans in the Loop | Require researchers to validate statistical figures, citations, interpretations, and final outputs. |

This approach allows AI to assist with research activities while retaining human responsibility for the accuracy and quality of official outputs.

## 9. Key Takeaways

- **Grounding** connects AI responses to reliable and verifiable information sources.
- **RAG** retrieves relevant information from an external knowledge base and provides it to the model as context.
- **Prompt engineering** improves outputs through clear instructions, background information, and examples.
- **Fine-tuning** further trains a pre-existing model to improve its performance on specialized tasks.
- **Humans in the Loop (HITL)** ensures that human expertise, judgment, and feedback remain part of the AI process.
- These techniques can be combined to develop more reliable, relevant, and responsible generative AI applications.
- No single technique completely eliminates hallucinations, bias, or other model limitations.

## 10. Quick Review Questions

**1. What is grounding?**

Connecting AI-generated responses to specific, verifiable information sources to improve accuracy and relevance.

**2. What does RAG stand for?**

Retrieval-Augmented Generation.

**3. What are the three main stages of RAG?**

1. Retrieval – searches for relevant information.
2. Augmentation – adds retrieved information to the model's prompt or context.
3. Generation – uses the augmented context to produce a response.

**4. What is the primary purpose of prompt engineering?**

To guide an AI model toward desired outputs through clear instructions, context, examples, and constraints.

**5. What is fine-tuning?**

Further training an existing pre-trained model using specialized data to adapt it to specific tasks or requirements.

**6. What is the difference between fine-tuning and RAG?**

Fine-tuning changes the model through additional training, while RAG retrieves external information and provides it to the model during response generation.

**7. What does HITL mean?**

Humans in the Loop. It integrates human input, review, and feedback into the AI or machine learning process.

**8. Why is human oversight important in AI applications?**

It helps detect errors, address bias, interpret context, and ensure accountability, particularly in sensitive and high-risk applications.
