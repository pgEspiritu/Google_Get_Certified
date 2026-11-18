# 🧠 Generative AI Fundamentals — Quiz Reviewer
## Topic 1: Fundamentals of Generative AI (Questions 11–20)

---

### 📝 Question #11: What type of model limitation is caused by biased or outdated training data?

A company trains a generative AI model designed to classify customer feedback as positive, negative, or neutral. However, the training dataset disproportionately includes feedback from a specific demographic and uses outdated language norms that don't reflect current customer communication styles.

When deployed, the model shows bias in sentiment analysis, misclassifying reviews from underrepresented demographics and struggling to understand current slang or phrasing.

**Choices:**

- A. Edge case
- B. Data dependency
- C. Hallucination
- D. Overfitting

**✅ Correct Answer: B. Data dependency**

**💡 Explanation:**

Generative AI and machine learning models depend heavily on the quality, diversity, relevance, and representativeness of their training data.

If training data is incomplete, outdated, imbalanced, or biased, the model may learn patterns that do not accurately represent the real-world population or current communication styles.

In this scenario:

- 👥 The dataset disproportionately represents a specific demographic.
- 🗣️ The language used in the dataset is outdated.
- 📉 The model performs poorly on underrepresented groups.
- 🔄 The model struggles with modern slang and changing expressions.

These limitations demonstrate **data dependency** because the model's behavior is influenced by the characteristics and limitations of the data it was trained on.

**📚 Why the other choices are incorrect:**

- **A. Edge case** — An unusual, rare, or unexpected situation that falls outside common scenarios or typical training examples.
- **C. Hallucination** — When an AI generates fabricated, inaccurate, or unsupported information and presents it as factual.
- **D. Overfitting** — When a model learns the training data too closely, including noise or specific patterns, and performs poorly on unseen data.

**🔑 Key takeaway:** Poor, outdated, unbalanced, or unrepresentative training data can lead to biased AI outputs and poor performance. This is a data dependency limitation.

---

### 📝 Question #12: What machine learning should the company use to classify customer reviews with labeled sentiments?

A company wants to build a model to classify customer reviews as positive, negative, or neutral.

They have collected thousands of customer reviews, and each review has been manually tagged with the corresponding sentiment:

- 😊 Positive
- 😐 Neutral
- 😞 Negative

**Choices:**

- A. Reinforcement learning
- B. Deep learning
- C. Unsupervised learning
- D. Supervised learning

**✅ Correct Answer: D. Supervised learning**

**💡 Explanation:**

Supervised learning is a machine learning approach that trains a model using labeled datasets. Each training example contains an input and its corresponding expected output.

In this scenario:

- 📥 **Input:** The customer review.
- 🏷️ **Label:** Positive, negative, or neutral.
- 🧠 **Learning process:** The model learns patterns in the reviews associated with each sentiment.
- 📤 **Output:** A predicted sentiment label for a new customer review.

Since the dataset already contains manually assigned sentiment labels, supervised learning is the appropriate approach.

This particular task is called **multiclass classification** because the model predicts one of three possible categories.

**📚 Why the other choices are incorrect:**

- **A. Reinforcement learning** — Learns through interactions, rewards, and penalties.
- **B. Deep learning** — A neural-network-based approach that may be used to implement sentiment classification, but the question asks for the learning approach based on labeled data.
- **C. Unsupervised learning** — Finds patterns or groupings without predefined labels.

**🔑 Key takeaway:** When the dataset contains inputs with known labels or correct answers, use supervised learning.

---

### 📝 Question #13: What type of agent automatically processes orders and performs fulfillment tasks?

An order fulfillment team has an agent that automatically:

- 📦 Processes orders.
- 📊 Updates inventory.
- 🚚 Sends shipping notifications.
- 🔄 Handles returns.

**Choices:**

- A. A conversational agent
- B. A customer service agent
- C. An employee productivity agent
- D. A workflow agent

**✅ Correct Answer: D. A workflow agent**

**💡 Explanation:**

A workflow agent is designed to automate a sequence of tasks or business processes. It can coordinate multiple actions, systems, and steps to complete a defined workflow.

In this scenario, the agent handles a series of interconnected operations related to order fulfillment.

A workflow agent may:

1. 🛒 Receive an order.
2. ✅ Validate order details.
3. 📦 Process the order.
4. 📊 Update inventory records.
5. 🚚 Notify customers about shipping.
6. 🔄 Manage return requests.

These activities follow a structured business process, making a workflow agent the best fit.

**📚 Why the other choices are incorrect:**

- **A. Conversational agent** — Primarily designed to interact with users through natural language conversations.
- **B. Customer service agent** — Primarily focused on customer inquiries, support, and resolving customer issues.
- **C. Employee productivity agent** — Helps employees accomplish individual work tasks, such as writing, summarizing, searching, or organizing information.
- **D. Workflow agent** — Automates and coordinates a sequence of tasks or business processes.

**🔑 Key takeaway:** When an AI agent automates a series of interconnected operational tasks, think of a workflow agent.

---

### 📝 Question #14: What should the company prioritize to mitigate privacy risks involving personally identifiable information (PII)?

A company is developing a generative AI application to analyze customer feedback collected through online surveys.

The feedback contains personally identifiable information (PII), and stakeholders are concerned about privacy risks before using the data to train the AI model.

**Choices:**

- A. Focusing on collecting only quantitative feedback data in future surveys.
- B. Implementing strong access controls to limit which teams can view the raw survey data.
- C. Ensuring that the AI model is trained on a large and diverse dataset.
- D. Applying data anonymization techniques to remove or obscure sensitive data.

**✅ Correct Answer: D.** Applying data anonymization techniques to remove or obscure sensitive data.

**💡 Explanation:**

Personally identifiable information (PII) refers to information that can identify an individual directly or indirectly, such as:

- 👤 Full name.
- 📧 Email address.
- 📱 Phone number.
- 🏠 Address.
- 🪪 Government-issued identification numbers.
- 🔎 Other information that can be linked to a specific individual.

Before using survey feedback to train an AI model, the company should prioritize minimizing the exposure of sensitive personal information.

Data anonymization involves removing, altering, masking, or transforming identifying information so that individuals cannot readily be identified from the resulting dataset.

Examples include:

| Original Data | Anonymized Data |
|---|---|
| Juan Dela Cruz | Customer 001 |
| juan@email.com | `[REDACTED]` |
| 09171234567 | `[REDACTED]` |
| Exact home address | Removed |
| Exact birth date | Age range, if needed |

This reduces the risk of exposing personal information during training and processing.

**📚 Why the other choices are incorrect:**

- **A.** Quantitative-only data collection does not automatically eliminate PII. Numerical data may still be identifying or sensitive.
- **B.** Access controls are important for data security, but they do not directly remove PII from the training dataset.
- **C.** Dataset diversity improves representation and model quality, but it does not directly address the privacy risk of sensitive information.

**🔑 Key takeaway:** When the problem specifically concerns PII in training data, prioritize anonymization or de-identification before using the data.

---

### 📝 Question #15: What type of data is collected through open-ended survey questions?

A company collects customer feedback through open-ended survey questions where customers can write detailed responses in their own words.

Example:

> "The product was easy to use, and the customer support was excellent, but the delivery took longer than expected."

**Choices:**

- A. Quantitative data
- B. Structured data
- C. Labeled data
- D. Unstructured data

**✅ Correct Answer: D. Unstructured data**

**💡 Explanation:**

Unstructured data is information that does not follow a predefined tabular format or fixed schema for its content.

Open-ended survey responses are typically unstructured because customers can freely express their opinions, experiences, and observations using natural language.

Examples of unstructured data include:

- 💬 Customer comments and feedback.
- 📧 Emails.
- 📄 Documents.
- 🖼️ Images.
- 🎙️ Audio recordings.
- 🎥 Videos.
- 📝 Social media posts.

Although survey responses may be stored in a structured database column, the actual written content is still considered unstructured text.

**📚 Why the other choices are incorrect:**

- **A. Quantitative data** — Numerical data that can be measured or counted, such as age, sales, ratings, or number of purchases.
- **B. Structured data** — Data organized according to a predefined schema, such as rows and columns with consistent fields.
- **C. Labeled data** — Data associated with predefined categories, tags, or target values for machine learning.

**🔑 Key takeaway:** Free-form text responses are unstructured data.

---

### 📝 Question #16: Which product can generate a podcast-style AI audio overview of uploaded research papers?

Analysts want an AI audio overview, similar to a podcast, summarizing a set of research papers they upload.

**Choices:**

- A. Cloud Storage
- B. Chirp
- C. AutoML
- D. NotebookLM

**✅ Correct Answer: D. NotebookLM**

**💡 Explanation:**

NotebookLM is an AI-powered research and learning assistant designed to work with user-provided sources.

Users can upload or provide research materials such as:

- 📄 Research papers.
- 📚 Documents.
- 📝 Notes.
- 🌐 Source materials.

NotebookLM can help users:

- Summarize uploaded materials.
- Answer questions grounded in their sources.
- Identify key concepts and insights.
- Organize information.
- Generate Audio Overviews, which present content in a podcast-style discussion.

The Audio Overview feature is especially useful for listening to a synthesized discussion of research materials instead of reading the entire collection.

**📚 Why the other choices are incorrect:**

- **A. Cloud Storage** — A storage service for saving and managing files and data.
- **B. Chirp** — A Google speech model family associated with speech recognition and audio-related tasks.
- **C. AutoML** — Tools for automating aspects of machine learning model development and training.

**🔑 Key takeaway:** For AI-generated podcast-style discussions of uploaded documents, think of NotebookLM.

---

### 📝 Question #17: Who should be involved in deciding whether a generative AI use case is acceptable from a risk perspective?

**Choices:**

- A. Only the data scientists
- B. A cross-functional group: business, legal, security, privacy, and technical owners
- C. Only the vendor
- D. Nobody, if the model is accurate

**✅ Correct Answer: B.** A cross-functional group: business, legal, security, privacy, and technical owners.

**💡 Explanation:**

Generative AI risk is multidimensional. It can involve technical, operational, legal, ethical, privacy, security, financial, and reputational risks.

A single team cannot fully evaluate all these aspects.

A cross-functional team brings together different perspectives to assess:

- ⚖️ **Legal:** Regulatory compliance, liability, contractual obligations, and applicable laws.
- 🔐 **Security:** Cybersecurity risks, unauthorized access, data exposure, and vulnerabilities.
- 🛡️ **Privacy:** Personal data processing, consent, privacy risks, and data protection.
- 💼 **Business:** Use-case suitability, business value, operational impact, and user requirements.
- 🧑‍💻 **Technical owners:** Architecture, feasibility, reliability, model limitations, and implementation.
- 👥 **End users or process owners:** Practical workflow needs, usability, and potential impacts on affected people.

This collaborative approach supports responsible AI governance and more informed decisions about whether a use case should be approved, restricted, redesigned, or rejected.

**📚 Why the other choices are incorrect:**

- **A.** Data scientists may understand model behavior, but they cannot independently evaluate every business, legal, security, or privacy risk.
- **C.** Vendors can provide technical guidance, but organizational risk ownership remains with the company.
- **D.** Model accuracy alone does not guarantee safety, fairness, privacy, compliance, or appropriateness.

**🔑 Key takeaway:** AI risk decisions require cross-functional governance, not just technical evaluation.

---

### 📝 Question #18: What is most likely missing when a technically successful AI pilot has low employee adoption?

A pilot works technically, but employees don't use it.

**Choices:**

- A. Higher temperature
- B. More TPUs
- C. A larger model
- D. Change management: training, champions, and communication

**✅ Correct Answer: D.** Change management: training, champions, and communication.

**💡 Explanation:**

A technically successful AI pilot does not automatically translate into successful adoption across an organization.

Employees may not use the tool if:

- 🤔 They do not understand how it works.
- 📚 They have not received adequate training.
- 😟 They are concerned about AI replacing their jobs.
- 🔄 The tool does not fit their existing workflow.
- 🧩 They do not know which tasks are appropriate for AI.
- 📢 The benefits have not been clearly communicated.
- 👥 There are no internal advocates or champions to support adoption.

Change management helps organizations transition from experimentation to practical usage.

It may include:

- 🎓 Training and onboarding.
- 📢 Clear communication about purpose and benefits.
- 👥 AI champions who help their colleagues.
- 🧪 Demonstrations and hands-on activities.
- 📋 Guidelines for responsible AI use.
- 🔄 Feedback mechanisms and continuous improvement.
- 🛠️ Integrating AI into actual workflows.

**📚 Why the other choices are incorrect:**

- **A. Higher temperature** — Changes the randomness or variability of model outputs; it does not directly solve employee adoption.
- **B. More TPUs** — Increases computational capacity when needed; it does not address user acceptance or organizational readiness.
- **C. A larger model** — May improve some capabilities, but it does not automatically make employees adopt the tool.

**🔑 Key takeaway:** If AI works but employees do not use it, focus on people, training, communication, and workflow integration.

---

### 📝 Question #19: Which Google model family should be selected for each use case?

Match each task with the appropriate Google model family.

| Use Case | Correct Model Family | Explanation |
|---|---|---|
| 🎨 Generate marketing images | **Imagen** | Designed for image generation from text prompts and other supported inputs. |
| 🎬 Generate a short product video | **Veo** | Google's generative video model family for creating video content. |
| 🎙️ Transcribe customer calls | **Chirp** | Speech model family associated with speech recognition and transcription. |
| 💻 Run a lightweight open model on your own infrastructure | **Gemma** | Open model family designed for flexible deployment and customization across different environments. |

**💡 Explanation:**

Google offers different AI model families specialized for different types of tasks.

#### 🎨 Imagen — Image Generation

Imagen is Google's image generation model family.

**Use it for:**

- Generating marketing visuals.
- Creating product concepts.
- Producing images from text prompts.
- Developing creative visual content.

**Example prompt:**

> Create a premium product advertisement featuring a modern wireless headset on a minimalist white background with soft studio lighting.

---

#### 🎬 Veo — Video Generation

Veo is Google's generative video model family.

**Use it for:**

- Creating short videos.
- Generating cinematic scenes.
- Producing promotional video concepts.
- Turning creative descriptions into video content.

**Example prompt:**

> Generate a 10-second cinematic product video showing a smartwatch rotating slowly against a dark premium background.

---

#### 🎙️ Chirp — Speech and Audio

Chirp is associated with Google's speech model capabilities.

**Use it for:**

- Speech recognition.
- Transcription.
- Converting spoken language into text.
- Processing audio input for speech-related tasks.

**Example:**

> Transcribe a recorded customer service call and convert the conversation into readable text.

---

#### 💻 Gemma — Lightweight and Open Models

Gemma is Google's family of open models designed for developers and researchers to use, customize, and deploy in different environments, subject to the specific model's license and requirements.

**Use it for:**

- Running models on your own infrastructure.
- Developing customized AI applications.
- Fine-tuning or adapting models for specific tasks.
- Exploring local or resource-conscious deployment options.

**Example:**

> Deploy a lightweight language model on an organization's own server to assist with internal document classification.

**🔑 Key takeaway:**

- 🎨 Imagen = Images
- 🎬 Veo = Videos
- 🎙️ Chirp = Speech
- 💻 Gemma = Open models

---

### 📝 Question #20: What is it called when a chatbot confidently cites a nonexistent company policy?

A chatbot confidently cites a company policy that does not exist.

**Choices:**

- A. Grounding
- B. Hallucination
- C. Tokenization
- D. Overfitting

**✅ Correct Answer: B. Hallucination**

**💡 Explanation:**

A hallucination occurs when a generative AI model produces false, fabricated, or unsupported information and presents it as though it were true.

In this scenario, the chatbot invents a company policy and confidently refers to it despite the policy not existing.

Hallucinations may include:

- 📄 Inventing policies, rules, or procedures.
- 🔗 Providing nonexistent citations or references.
- 📊 Generating incorrect statistics.
- 👤 Creating fictional names or events.
- ⚖️ Misrepresenting laws, regulations, or organizational requirements.

Organizations can reduce hallucination risks through:

- 📚 Grounding responses in approved sources.
- 🔎 Retrieval-Augmented Generation (RAG).
- 📝 Providing reliable and updated knowledge bases.
- 👥 Human review for high-impact decisions.
- ⚠️ Clearly communicating model limitations.
- 🔐 Restricting AI from answering when reliable information is unavailable.

**📚 Why the other choices are incorrect:**

- **A. Grounding** — Connecting AI responses to trusted information, sources, or contextual data to improve factual accuracy.
- **C. Tokenization** — Breaking text into smaller units called tokens that models process.
- **D. Overfitting** — Learning training data too closely and failing to generalize well to new data.

**🔑 Key takeaway:** A chatbot inventing a nonexistent policy or confidently providing fabricated information is hallucinating.

---

# 📚 Quick Review: Questions 11–20

| # | Concept | Correct Answer | Remember |
|---|---|---|---|
| 11 | Model limitation | **B. Data dependency** | Biased, outdated, or poor-quality data affects AI results. |
| 12 | Machine learning | **D. Supervised learning** | Uses labeled data to learn predictions. |
| 13 | Agent type | **D. Workflow agent** | Automates interconnected business processes. |
| 14 | Data privacy | **D. Data anonymization** | Removes or obscures PII. |
| 15 | Data type | **D. Unstructured data** | Free-form text has no fixed content structure. |
| 16 | Google product | **D. NotebookLM** | Generates Audio Overviews from provided sources. |
| 17 | AI governance | **B. Cross-functional group** | Risk requires business, legal, security, privacy, and technical input. |
| 18 | AI adoption | **D. Change management** | Training, champions, communication, and workflow integration. |
| 19 | Google models | **Imagen, Veo, Chirp, Gemma** | Images, video, speech, open models. |
| 20 | AI limitation | **B. Hallucination** | Fabricated information presented as factual. |

---

# 🧠 Memory Guide: Questions 11–20

| Keyword in the Question | Concept to Remember |
|---|---|
| 📉 Biased or outdated training data | Data dependency |
| 🏷️ Reviews with sentiment labels | Supervised learning |
| 📦 Processing orders, inventory, shipping, and returns | Workflow agent |
| 🔐 Personally identifiable information (PII) in training data | Data anonymization |
| 💬 Open-ended survey responses | Unstructured data |
| 🎧 Podcast-style summary of uploaded research | NotebookLM |
| ⚖️ AI use-case risk assessment | Cross-functional governance |
| 👥 Pilot works, but employees do not use it | Change management |
| 🎨 Image generation | Imagen |
| 🎬 Video generation | Veo |
| 🎙️ Speech recognition / transcription | Chirp |
| 💻 Open model for custom deployment | Gemma |
| 📄 Fake or nonexistent company policy | Hallucination |

---

# 🚀 Topic 1 — Important Concepts to Master

## 🤖 AI Agents

AI agents are goal-oriented systems capable of analyzing inputs, making decisions, using tools, and taking actions toward achieving objectives.

### Common agent types

- 💬 **Conversational agents** — Interact with people through natural language.
- 👥 **Customer service agents** — Handle customer inquiries, support, and assistance.
- 🧑‍💻 **Employee productivity agents** — Help employees perform work more efficiently.
- 🔄 **Workflow agents** — Automate and coordinate sequences of tasks or business processes.

---

## 📊 Machine Learning Types

### 🏷️ Supervised Learning

- Uses labeled data.
- Learns from examples with known outcomes.
- Commonly used for classification and regression.

**Example:** Predicting whether a customer review is positive, negative, or neutral.

### 🔎 Unsupervised Learning

- Uses unlabeled data.
- Discovers patterns, clusters, and relationships.
- Commonly used for segmentation and anomaly detection.

**Example:** Grouping customers based on purchasing behavior.

### 🎮 Reinforcement Learning

- Learns through interaction.
- Receives rewards and penalties.
- Improves decisions through trial and error.

**Example:** Training an AI character to navigate a game.

### 🧠 Deep Learning

- Uses multilayer neural networks.
- Learns complex patterns.
- Commonly used in computer vision, speech, and generative AI.

---

## ⚠️ Common Gen AI Limitations

### 📚 Data Dependency

AI performance depends on the quality, diversity, accuracy, relevance, and representativeness of its data.

**Problems:**

- Biased training datasets.
- Outdated information.
- Missing data.
- Poor-quality data.
- Underrepresented groups.

### 👻 Hallucination

AI generates fabricated, false, or unsupported information.

**Examples:**

- Inventing policies.
- Creating fake citations.
- Giving false facts confidently.
- Making up scientific explanations.

### 🎯 Overfitting

The model learns training data too closely and performs poorly on new or unseen data.

### 🧩 Edge Cases

Rare, unusual, or unexpected situations that the model may not handle correctly.

---

## 🔐 Responsible AI and Data Privacy

### Personally Identifiable Information (PII)

PII is information that can identify a person directly or indirectly.

Examples:

- Full name.
- Email address.
- Phone number.
- Home address.
- Identification numbers.

### Privacy protection measures

- 🧹 Anonymization and de-identification.
- 🔐 Access controls.
- 🔒 Encryption.
- 📋 Data governance.
- 🛡️ Privacy safeguards.
- ⚖️ Regulatory compliance.

### AI Governance

AI decisions should involve multiple stakeholders, including:

- Business owners.
- Legal teams.
- Security teams.
- Privacy officers.
- Technical teams.
- Operational owners.

---

## 🏢 AI Adoption and Change Management

Successful AI implementation is not just about building a technically capable model.

Organizations also need:

- 🎓 Employee training.
- 📢 Communication.
- 👥 AI champions.
- 🧪 Pilot programs.
- 🔄 Feedback loops.
- 🛠️ Workflow integration.
- 📋 Responsible AI guidelines.

> 💡 A successful AI implementation requires both technical readiness and organizational readiness.

---

## 🌐 Google AI Model Families

| Model Family | Primary Use |
|---|---|
| 🎨 Imagen | Image generation |
| 🎬 Veo | Video generation |
| 🎙️ Chirp | Speech and audio-related tasks |
| 💻 Gemma | Open models for development, customization, and deployment |

---

## 🎯 Final Exam Strategy

When answering Fundamentals of Generative AI questions, identify the main keyword in the scenario first.

1. **Rewards and penalties** → Reinforcement Learning
2. **Labeled examples** → Supervised Learning
3. **Unlabeled patterns** → Unsupervised Learning
4. **Creates new content** → Generative AI
5. **Uses tools and performs tasks autonomously** → AI Agent
6. **Automates a sequence of business operations** → Workflow Agent
7. **Invents information** → Hallucination
8. **Poor, biased, or outdated training data** → Data Dependency
9. **Protects personally identifiable information** → Anonymization / Data Privacy
10. **Podcast-style research summary** → NotebookLM
11. **Employees are not adopting AI** → Change Management
12. **Images** → Imagen
13. **Videos** → Veo
14. **Speech transcription** → Chirp
15. **Open model for custom deployment** → Gemma
16. **Strict, predictable, rule-based decisions** → Deterministic Systems

---
