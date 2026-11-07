# 🎯 Choosing a Generative AI Model

## 1. Factors to Consider When Choosing a Model

Choosing the right generative AI model is an important step when developing an AI-powered application. Different models have different capabilities, limitations, resource requirements, and costs.

The best model is not necessarily the largest or most advanced one. It should be appropriate for the specific task, available resources, and intended users.

Here are seven important factors to consider when selecting a model.

### 1.1 Modality

**Modality** refers to the type of data a model can process (input) and generate (output).

Common modalities include:
- **Text** – Documents, articles, emails, and questions.
- **Images** – Photographs, illustrations, and diagrams.
- **Audio** – Speech, music, and sound recordings.
- **Video** – Moving images and video clips.

Models may be designed for a single modality or multiple modalities.

**Unimodal models** specialize in processing or generating a particular type of data.

Examples:
- A model that generates text-based articles.
- A model that converts text into speech.
- A model that generates images from text descriptions.

**Multimodal models** can process or generate multiple types of data.

Examples:
- An AI model that analyzes an image and generates a text description.
- A model that processes audio and text together.
- A model that generates a video with accompanying audio.

**When to consider it:** Choose a model based on the input and output formats required by your application. If your application needs to understand images and generate text, a text-only model may not be sufficient.

### 1.2 Context Window

The **context window** refers to the amount of information a model can process and consider at one time when generating a response.

It is commonly measured in tokens. A token may represent a complete word, part of a word, punctuation, or another unit of text.

A larger context window allows a model to process more information, such as:
- Longer conversations.
- Large documents.
- Multiple files.
- Extensive instructions.
- Complex sets of information.

**Example:**

Suppose a government researcher wants to use AI to summarize a 200-page research report.

- A model with a small context window may not be able to process the entire report in one request.
- A model with a larger context window may be able to process more of the document at once.

However, a larger context window does not automatically guarantee better answers. The relevance and quality of the supplied information still matter.

Larger inputs may also increase processing costs and latency.

**When to consider it:** Choose a model with sufficient context capacity for the size of your documents, conversations, or other inputs.

### 1.3 Security

**Security** is essential when using generative AI, particularly when processing confidential, personal, or organizational information.

Consider the following security capabilities:

- **Data encryption** – Protects information while it is being transmitted and stored.
- **Access controls** – Ensures that only authorized users can access data and services.
- **Identity and Access Management (IAM)** – Manages user identities, roles, and permissions.
- **Vulnerability management** – Helps identify and address security weaknesses.
- **Compliance** – Ensures that the service supports applicable security standards and regulatory requirements.

**Example:**

A government agency wants to use an AI model to summarize internal reports containing personal information.

Before selecting a model, the agency should evaluate:
- Whether the service is approved for the intended data classification.
- How submitted data is stored and processed.
- Whether user access can be restricted.
- Whether organizational and legal privacy requirements are met.

**When to consider it:** Evaluate security, privacy, data handling, and compliance requirements before sending sensitive information to an AI service.

### 1.4 Availability and Reliability

**Availability** refers to whether a model or service can be accessed when needed.

**Reliability** refers to its ability to operate consistently and produce dependable results.

Important considerations include:

- **Uptime** – How consistently the service remains operational.
- **Redundancy** – Availability of backup systems or resources.
- **Disaster recovery** – Ability to recover from major service disruptions.
- **Service Level Agreements (SLAs)** – Defined service commitments, where applicable.
- **Capacity** – Ability to handle the expected number of users and requests.

**Example:**

A government agency plans to deploy an AI-powered public assistance chatbot.

If the chatbot is unavailable during peak hours, citizens may be unable to access the service.

The agency should therefore evaluate the service's availability, reliability, and ability to handle varying request volumes.

**When to consider it:** Select a model and hosting service that can meet the operational requirements of your application.

### 1.5 Cost

Generative AI models can have significantly different operating costs.

Pricing may depend on:
- Number of input tokens.
- Number of output tokens.
- Model size and capabilities.
- Number of requests.
- Computing resources.
- Training and fine-tuning requirements.
- Hosting and deployment arrangements.

**Example:**

An organization wants to generate short summaries of thousands of documents.

Using a highly advanced model for every document may be unnecessarily expensive if a smaller, less costly model can perform the task accurately enough.

This highlights an important principle:

**Bigger isn't always better. Choose the model that provides the appropriate capabilities at a reasonable cost.**

Also, multimodal capabilities are not always necessary. If an application only processes text, paying for capabilities that it does not use may not be cost-effective.

**When to consider it:** Compare expected performance and business value against the total cost of operating the model.

### 1.6 Performance

**Performance** refers to how effectively and efficiently a model performs its intended task.

Important performance considerations include:

- **Accuracy** – How correctly the model performs a task.
- **Speed** – How quickly it processes requests and generates responses.
- **Latency** – The time between submitting a request and receiving a response.
- **Efficiency** – How effectively it uses computing resources.
- **Consistency** – Whether it produces dependable results across similar requests.

**Example:**

An organization wants to use an AI model to classify incoming government service requests.

It should evaluate whether the model:
- Correctly identifies the category of each request.
- Processes requests quickly enough.
- Handles different ways of expressing the same concern.
- Produces consistent classifications.

Models should be evaluated using datasets and benchmarks relevant to the actual application rather than relying only on general benchmark scores.

**When to consider it:** Test models using realistic examples from your intended use case and compare their accuracy, speed, and efficiency.

### 1.7 Fine-Tuning and Customization

**Fine-tuning** is the process of further training a pretrained model using additional task-specific data to adapt its behavior or performance to a particular application.

Customization is a broader concept that may include:
- Fine-tuning.
- Prompt engineering.
- Providing additional context.
- Connecting the model to external information sources.
- Configuring model behavior and parameters.

**Example:**

A government agency wants to develop an AI assistant that can respond to questions about its internal administrative procedures.

Possible approaches include:

- **Prompting** – Giving the model clear instructions on how to respond.
- **Retrieval-Augmented Generation (RAG)** – Connecting the model to relevant internal documents so it can retrieve information before generating answers.
- **Fine-tuning** – Further training a suitable model using task-specific examples to adapt its behavior.

These approaches serve different purposes. Fine-tuning is not always necessary to make a model useful for a specialized application.

**When to consider it:** Determine whether the model needs additional training, external knowledge, or simply better instructions to meet your requirements.

### 1.8 Ease of Integration

The ease of integrating a model into existing systems and workflows is another important consideration.

A model may have excellent capabilities, but implementing it can be difficult if it does not work well with the organization's existing technology.

Consider:
- **APIs** – Interfaces that allow applications to communicate with the model.
- **SDKs** – Software development kits that simplify integration.
- **Documentation** – Guides and technical references for developers.
- **Compatibility** – Support for existing applications, databases, and infrastructure.
- **Deployment options** – Availability of cloud, local, or other deployment arrangements.

**Example:**

An agency wants to integrate a generative AI model into its existing document management system.

A model with a well-documented API and supported SDKs may make integration easier and reduce development effort.

**When to consider it:** Choose a model that can be integrated into your existing infrastructure without unnecessary complexity.

## 2. Summary: Model Selection Criteria

| Factor | Key Question | What to Evaluate |
|---|---|---|
| Modality | What types of data must the model process and generate? | Text, images, audio, video, or multiple modalities |
| Context Window | How much information must the model consider at once? | Token capacity and input limitations |
| Security | Can the model safely handle the intended data? | Encryption, access controls, privacy, and compliance |
| Availability and Reliability | Will the model be available when needed? | Uptime, redundancy, disaster recovery, and capacity |
| Cost | Is the model cost-effective? | Usage pricing, computing resources, and operating costs |
| Performance | Can the model perform the task effectively? | Accuracy, speed, latency, and efficiency |
| Fine-Tuning and Customization | Can the model be adapted to the use case? | Fine-tuning, prompting, and external knowledge integration |
| Ease of Integration | Can it work with existing systems? | APIs, SDKs, documentation, and compatibility |

## 3. Google Cloud's Machine Learning Models

Google Cloud provides access to different AI models through its AI development platform, allowing organizations to discover, evaluate, deploy, and customize models for their applications.

The course refers to **Agent Platform** as the platform for accessing and integrating different models.

Instead of developing every AI model from scratch, organizations can use existing models developed by Google, third-party providers, and the open-source community.

This provides flexibility when selecting a model based on the requirements of a particular project.

### Types of Models Available

The course introduces four models from Google's AI model ecosystem:

1. Gemini
2. Gemma
3. Nano Banana
4. Veo

### 3.1 Gemini

<text weight="semibold">Model type: Multimodal foundation model</text>

<AsyncImage query="Google Gemini AI logo official" aspectRatio="16:9" fit="contain" maxHeight={120}/>

**Gemini** is Google's family of multimodal AI models designed to understand and work with different types of information.

It can support tasks involving:
- Text
- Images
- Audio
- Video
- Code

Because of its multimodal capabilities, Gemini can support applications requiring more than text-based interaction.

**Common applications:**
- Conversational AI assistants.
- Document analysis and summarization.
- Image understanding and description.
- Audio and video analysis.
- Question answering.
- Content generation.

**Example:**

A researcher uploads a chart showing regional poverty indicators and asks Gemini to explain the major trends.

The model can analyze the visual information and generate a text-based explanation.

**Key idea:** Gemini is suitable for applications requiring advanced reasoning, conversational interaction, and multimodal understanding.

### 3.2 Gemma

<text weight="semibold">Model type: Lightweight, openly available model family</text>

<AsyncImage query="Google Gemma AI logo official" aspectRatio="16:9" fit="contain" maxHeight={120}/>

**Gemma** is a family of lightweight, openly available models developed using research and technology associated with Google's Gemini models.

Gemma models provide developers with options for building customized AI applications, including deployments in environments where greater control over the model and infrastructure is important.

**Common applications:**
- Custom AI assistants.
- Text generation and summarization.
- Specialized language-processing applications.
- Local or self-managed AI deployments, depending on the model and hardware requirements.

**Example:**

An organization wants to develop a specialized AI assistant that helps employees search and understand internal guidelines.

A suitable Gemma model could be evaluated for deployment in an environment controlled by the organization.

**Key idea:** Gemma provides developers with more flexibility for customization and deployment compared with relying exclusively on hosted proprietary models.

### 3.3 Nano Banana

<text weight="semibold">Model type: AI image generation and editing</text>

<AsyncImage query="Google Nano Banana AI image generation example" aspectRatio="16:9" maxHeight={180}/>

**Nano Banana** is Google's image-generation and image-editing model family.

It can generate or modify images using natural-language instructions and reference images.

**Common applications:**
- Creative design.
- Product visualization.
- Marketing materials.
- E-commerce imagery.
- Image editing and transformation.
- Visual content creation.

**Example:**

An online store wants to create product images showing a particular item in different environments.

Users can provide an image and describe the desired changes, allowing the model to generate modified visuals.

**Key idea:** Nano Banana is useful for applications involving image generation and editing.

### 3.4 Veo

<text weight="semibold">Model type: AI video generation</text>

<AsyncImage query="Google Veo AI video generation cinematic example" aspectRatio="16:9" maxHeight={180}/>

**Veo** is Google's generative AI model family for creating video content.

It can generate videos based on:
- Text descriptions.
- Still images.
- Other supported inputs and editing instructions, depending on the model version.

**Common applications:**
- Film and video production.
- Advertising.
- Educational content.
- Social media videos.
- Creative storytelling.
- Marketing campaigns.

**Example:**

A training team wants to create a short instructional video illustrating proper workplace safety procedures.

A video generation model such as Veo can help create visual scenes based on text descriptions or reference images.

**Key idea:** Veo is designed for generating video content using AI.

## 4. Comparing Google's Foundation Models

| Model | Main Capability | Typical Output | Example Application |
|---|---|---|---|
| Gemini | Multimodal understanding and generation | Text and other supported modalities | Conversational AI and document analysis |
| Gemma | Lightweight, customizable AI models | Depends on model variant | Specialized AI applications |
| Nano Banana | Image generation and editing | Images | Product visualization and creative design |
| Veo | Video generation | Videos | Advertising and educational videos |

## 5. Choosing the Right Model for Different Use Cases

The best model depends on the task you want to accomplish.

| Use Case | Suitable Model | Reason |
|---|---|---|
| Answering questions about documents | Gemini | Understands text and supports document analysis |
| Developing a customized AI assistant | Gemma | Offers openly available models for customization |
| Generating product images | Nano Banana | Specializes in image generation and editing |
| Creating instructional videos | Veo | Generates video content |
| Analyzing images and generating explanations | Gemini | Supports multimodal input and text generation |

These are examples of suitable model choices, not exclusive limitations. Actual capabilities depend on the specific model version and deployment environment.

## 6. Applying Model Selection to Government and Statistical Work

Consider a government agency that wants to use generative AI to improve research, training, and public service delivery.

Different applications may require different models.

| Government Application | Possible Model | Important Selection Criteria |
|---|---|---|
| Summarizing research reports | Gemini | Context window, accuracy, and security |
| Developing an internal AI assistant | Gemma or Gemini | Customization, privacy, and integration |
| Creating infographics and illustrations | Nano Banana | Image quality and editing capabilities |
| Producing training videos | Veo | Video quality, cost, and output requirements |
| Analyzing charts and visual data | Gemini | Multimodal capabilities and accuracy |

### Example: AI Assistant for Statistical Research

Suppose PSRTI wants to develop an AI assistant to help researchers locate and understand institutional research materials.

The following considerations would be important:

1. **Modality:** The assistant should process text-based reports, PDFs, and possibly tables or charts.
2. **Context window:** It should handle sufficiently large documents and multiple sources.
3. **Security:** Internal and confidential research materials must be protected.
4. **Availability:** Researchers should be able to access the system when needed.
5. **Cost:** The service should fit within the organization's budget.
6. **Performance:** Answers should be accurate and supported by relevant source documents.
7. **Customization:** The system should use institutional materials and follow appropriate response guidelines.
8. **Integration:** It should work with existing document repositories and applications.

The organization should evaluate candidate models using actual research tasks before selecting one for production.

## 7. Key Takeaways

1. Selecting a generative AI model requires evaluating its capabilities, limitations, cost, and suitability for the intended application.
2. **Modality** determines the types of information a model can process and generate.
3. The **context window** determines how much information a model can consider at one time.
4. **Security, availability, and reliability** are especially important for enterprise and government applications.
5. **Cost and performance** should be evaluated together. A larger model is not automatically the best choice.
6. **Fine-tuning and customization** allow models to be adapted to specific requirements, but additional training is not always necessary.
7. **Ease of integration** determines how effectively a model can work with existing systems.
8. Google offers different model families for different tasks:
   - Gemini – Multimodal AI.
   - Gemma – Lightweight, openly available models.
   - Nano Banana – Image generation and editing.
   - Veo – Video generation.

## 8. Quick Review Questions

**1. What does modality mean when selecting an AI model?**

Answer: The type of data a model can process and generate, such as text, images, audio, and video.

**2. What is a context window?**

Answer: The amount of information, commonly measured in tokens, that a model can consider at one time.

**3. Why is security important when selecting a model?**

Answer: It helps protect sensitive information through encryption, access controls, and appropriate privacy and compliance safeguards.

**4. Does a larger model always provide better results?**

Answer: No. The model should be appropriate for the task, and its performance should be balanced against cost and resource requirements.

**5. What is fine-tuning?**

Answer: Further training a pretrained model using task-specific data to adapt its behavior or performance.

**6. Which Google model is designed for multimodal understanding?**

Answer: Gemini.

**7. Which Google model family provides lightweight, openly available models?**

Answer: Gemma.

**8. Which Google model is used for image generation and editing?**

Answer: Nano Banana.

**9. Which Google model is designed for video generation?**

Answer: Veo.

**10. What should an organization consider before deploying a generative AI model?**

Answer: Modality, context window, security, availability, reliability, cost, performance, customization requirements, and ease of integration.
