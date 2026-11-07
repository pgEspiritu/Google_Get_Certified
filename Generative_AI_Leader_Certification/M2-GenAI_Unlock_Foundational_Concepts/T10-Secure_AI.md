# Secure AI

## 1. Introduction

Artificial Intelligence (AI) systems enable computers to recognize, understand, and interpret information in increasingly sophisticated ways. These technologies are developing rapidly and are being applied across different industries, including healthcare, finance, education, and government.

However, despite their capabilities, AI systems are not infallible. They can be exposed to security threats, misuse, privacy violations, and malicious attacks.

Building responsible AI means ensuring that technology:
- Provides benefits without causing harm.
- Protects the privacy and sensitive information of users.
- Avoids spreading misinformation and harmful content.
- Treats individuals and groups fairly and ethically.
- Is protected against malicious attacks and unauthorized access.

This lesson focuses on **Secure AI** and the security considerations involved in developing, deploying, and maintaining AI applications.

## 2. What Does Secure AI Mean?

**Secure AI** refers to protecting AI systems from intentional harm, malicious attacks, unauthorized access, and misuse.

Security must be considered throughout the entire AI lifecycle, from development and data collection to deployment, monitoring, and maintenance.

This involves protecting three major areas:

1. **Data:** Ensuring that training data, input data, and generated information are protected against unauthorized access, manipulation, and disclosure.
2. **Infrastructure:** Securing the hardware, software, networks, cloud resources, and systems used to develop and operate AI applications.
3. **AI applications and models:** Protecting models from theft, manipulation, adversarial attacks, and unauthorized use.

### 2.1 Security Across the Machine Learning Lifecycle

Security must be integrated into every stage of the machine learning lifecycle.

### Stage 1: Gather Your Data

The foundation of a secure AI system is properly protected data.

Organizations must implement access controls to determine:
- Who can access the data.
- Who can add, modify, or delete records.
- Which systems and applications can use the data.
- What activities users are authorized to perform.

These controls help prevent unauthorized changes and protect the integrity of training datasets.

**Security concern: Data Poisoning**

Data poisoning is a malicious attack in which an attacker introduces manipulated, incorrect, or harmful information into an AI model's training dataset.

This can cause the model to learn incorrect patterns and produce flawed, biased, or harmful predictions.

**Example:**

Suppose an organization trains an AI model to identify defective products using thousands of labeled images.

An attacker secretly introduces incorrectly labeled images, marking defective products as acceptable.

As a result, the model may learn incorrect patterns and classify defective products as acceptable during actual inspections.

**Recommended security practices:**
- Implement access controls for datasets.
- Restrict permissions for adding or modifying training data.
- Verify the sources of collected information.
- Maintain data integrity checks.
- Monitor unusual changes in datasets.

### Stage 2: Prepare Your Data

During data preparation, organizations must pay particular attention to confidential and sensitive information.

Training datasets may contain personal information, financial records, government records, or other protected information.

**Recommended security practices:**

- **Anonymization:** Remove or transform personally identifiable information (PII) when appropriate to reduce privacy risks.
- **Data validation:** Check datasets for incorrect, inconsistent, or suspicious information.
- **Integrity checks:** Verify that data has not been modified without authorization.
- **Anomaly detection:** Identify unusual patterns that may indicate data manipulation or poisoning.
- **Encryption:** Protect data at rest and during transmission. Additional protections may be necessary when data is actively processed.
- **Logging and monitoring:** Record data access and processing activities to help identify suspicious behavior.

**Example:**

Before using CBMS data to develop an AI-assisted analytical application, an organization should assess whether personal information is present and apply appropriate privacy and security measures.

Removing direct identifiers alone may not guarantee anonymity, especially when records can be linked with other datasets.

### Stage 3: Train Your Model

The model and its training process must be protected against unauthorized access, modification, and theft.

An AI model contains learned parameters and may also incorporate proprietary information, specialized capabilities, or sensitive organizational knowledge.

**Security concern: Model Theft**

Model theft occurs when attackers obtain unauthorized copies of proprietary or sensitive AI models.

Stolen models may be:
- Replicated and used without authorization.
- Analyzed to discover vulnerabilities.
- Used for malicious purposes.
- Exploited to reproduce sensitive functionality.

**Recommended security practices:**
- Restrict access to model files and training environments.
- Protect model parameters and checkpoints.
- Secure training infrastructure and computing resources.
- Monitor model downloads and access activities.
- Protect model artifacts using encryption and appropriate access permissions.

### Stage 4: Deploy and Predict

Once a model has been trained, it must be protected within its operating environment.

This includes controlling who can interact with the model, what information it can access, and what actions it is allowed to perform.

**Recommended security practices:**
- Implement authentication and authorization.
- Restrict access to model endpoints and APIs.
- Apply appropriate input validation and filtering.
- Verify the source and integrity of pre-built or third-party models.
- Review dependencies and check for known vulnerabilities.
- Monitor incoming requests and generated outputs.

**Example:**

A government agency deploys an AI chatbot to answer questions about public services.

The agency should ensure that:
- Only authorized systems can access internal databases.
- Users cannot access confidential employee records.
- The chatbot does not disclose sensitive information.
- Suspicious or malicious requests are detected and handled appropriately.

### Stage 5: Manage Your Model

Security does not end after deployment. AI models and their operating environments require continuous monitoring and maintenance.

**Recommended security practices:**
- Regularly update software, libraries, and infrastructure.
- Apply security patches to address known vulnerabilities.
- Monitor model performance and outputs for unusual behavior.
- Detect possible signs of tampering or unauthorized modification.
- Review access permissions periodically.
- Monitor security logs and investigate suspicious activities.
- Update security controls as new threats emerge.

### Summary of Security Across the ML Lifecycle

| ML Lifecycle Stage | Security Focus | Example Threat or Risk |
|---|---|---|
| Gather data | Protect data access and integrity. | Data poisoning |
| Prepare data | Protect sensitive information and validate datasets. | Privacy breaches and manipulated data |
| Train model | Secure training data, parameters, and model artifacts. | Model theft |
| Deploy and predict | Control access to models and validate inputs. | Unauthorized access and adversarial attacks |
| Manage model | Continuously monitor, update, and maintain security. | Vulnerabilities, tampering, and misuse |

## 3. Adversarial Attacks

An **adversarial attack** occurs when an attacker deliberately manipulates inputs or interactions to cause an AI model to behave incorrectly or produce unintended results.

The attacker attempts to exploit weaknesses in the model or its surrounding application.

Think of it as someone attempting to bypass a security system using a fake identification card.

### Examples of Adversarial Attacks

**1. Manipulated Input Data**

An attacker introduces specially crafted information that causes an AI model to misclassify or misunderstand an input.

Example: An image recognition system is tricked into identifying a stop sign as a different traffic sign because of carefully designed alterations to the image.

**2. Prompt Injection**

Prompt injection occurs when malicious instructions are introduced through user input or external content to manipulate a generative AI application's behavior.

Example: A user attempts to make an AI assistant ignore its original instructions and reveal confidential information.

**3. Data Poisoning**

An attacker manipulates training data so that the model learns incorrect or harmful patterns.

**4. Model Theft**

An attacker attempts to obtain an unauthorized copy of a model or extract information about its behavior through repeated interactions.

### Input and Output Security

Organizations must protect both the information entering an AI model and the information it generates.

| Security Area | Purpose | Examples |
|---|---|---|
| Input security | Prevent malicious, manipulated, or unauthorized information from reaching the model. | Input validation, access controls, filtering, and prompt injection defenses |
| Output security | Prevent the model from exposing sensitive information or generating harmful content. | Output filtering, sensitive-data detection, content moderation, and human review |

**Input safeguards:**
- Validate and sanitize user inputs.
- Check external documents and retrieved content.
- Apply access controls to data sources.
- Detect suspicious or malicious instructions.
- Separate trusted system instructions from untrusted user-provided content.

**Output safeguards:**
- Check generated responses for sensitive information.
- Apply appropriate content moderation.
- Prevent unauthorized disclosure of confidential records.
- Validate important outputs before they are used in operational decisions.

> **Key takeaway:** Secure AI requires protection at both ends of the process. Organizations must filter and validate incoming information while monitoring generated outputs to prevent data leakage and harmful content.

## 4. Stay Informed About AI Security

AI security threats continue to evolve as models, applications, and attack techniques become more sophisticated.

Organizations must stay informed about emerging vulnerabilities, security research, and recommended practices.

The lesson introduces three important areas of support from Google:

### 4.1 Applying the Secure AI Framework (SAIF)

<text color="secondary" size="xs" weight="medium">GOOGLE SECURITY FRAMEWORK</text>

**SAIF (Secure AI Framework)** is Google's framework for establishing security practices for developing and deploying AI systems.

It provides a structured approach to managing AI and machine learning security risks.

SAIF aims to help organizations:
- Identify and understand potential AI security threats.
- Strengthen security defenses.
- Manage risks associated with AI systems.
- Integrate AI security into existing organizational security practices.
- Build AI applications with security considered from the beginning.

An important concept associated with SAIF is **secure by design**.

This means that security should be incorporated into the architecture, development, and deployment of AI systems rather than added only after an application has been built.

**Official reference:** [Google Secure AI Framework (SAIF)](https://safety.google/cybersecurity-advancements/saif/)

### 4.2 Google Cloud Security Tools

Google Cloud provides security capabilities that organizations can use to protect their applications, infrastructure, and data throughout the AI lifecycle.

Important tools and capabilities mentioned in the lesson include:

| Tool / Capability | Purpose |
|---|---|
| Secure-by-design infrastructure | Provides security protections across Google's infrastructure, hardware, and global network. |
| Encryption | Protects information at rest and in transit. |
| Identity and Access Management (IAM) | Controls who can access cloud resources and what actions they can perform. |
| Security Command Center | Provides centralized visibility into security risks, vulnerabilities, and security posture across Google Cloud environments. |
| Monitoring tools | Help observe workloads, identify unusual activities, and support operational security. |

#### Identity and Access Management (IAM)

IAM is particularly important because not every employee or application should have unrestricted access to organizational resources.

IAM allows administrators to assign permissions based on users' responsibilities.

**Example:**

In a government research project:
- A researcher may be allowed to view approved datasets.
- A data administrator may be allowed to modify records.
- An external participant may only access a public-facing application.

This follows the principle of **least privilege**, which means granting users and systems only the permissions necessary to perform their assigned tasks.

#### Security Command Center

Security Command Center provides a centralized view of security risks and findings across a Google Cloud environment.

It helps organizations identify potential vulnerabilities, misconfigurations, and threats that may affect their cloud resources.

### 4.3 Threat Research, Intelligence, and Expert Guidance

Security tools alone are not enough. Organizations also need to understand how attackers operate and how threats are evolving.

Google provides security research and expert guidance through groups such as:

**Google Threat Intelligence Group (GTIG)**

- Conducts research on emerging cyber threats and malicious activities.
- Shares threat intelligence to help organizations understand and respond to attacks.
- Helps identify and disrupt malicious operations.

**Mandiant**

- Provides cybersecurity threat intelligence and incident response expertise.
- Conducts security research and shares findings about attacker behavior.
- Offers consulting services to help organizations strengthen their security posture.
- Supports organizations in securing AI usage and applying AI to improve cyber defense.

These resources help organizations move beyond basic security controls toward proactive threat detection, validation, and operational readiness.

## 5. Practical Application: Securing a Government AI Assistant

Imagine a government agency develops an AI assistant that helps employees search internal documents, summarize reports, and answer questions about organizational policies.

The following security measures can be applied:

| Area | Potential Risk | Recommended Security Measure |
|---|---|---|
| Data collection | Unauthorized access to internal documents | Implement IAM and data access restrictions. |
| Data preparation | Exposure of personal information | Apply anonymization and data validation. |
| Model training | Unauthorized modification or theft | Secure model artifacts and training infrastructure. |
| Application deployment | Prompt injection and unauthorized access | Implement authentication, input validation, and security filtering. |
| AI responses | Disclosure of confidential information | Apply output filtering and sensitive-data detection. |
| Model management | Emerging vulnerabilities and suspicious activities | Monitor logs, update systems, and review permissions. |

For example, if an employee asks the assistant to summarize a confidential research report, the system should first verify whether that employee is authorized to access the document.

The AI assistant should not bypass document permissions simply because it can retrieve or summarize the content.

This demonstrates an important principle: **AI security must cover not only the model itself but also the data, users, applications, and infrastructure connected to it.**

## 6. Key Takeaways

- **Secure AI** protects AI systems from malicious attacks, unauthorized access, manipulation, and misuse.
- Security must be integrated throughout the machine learning lifecycle, from data collection to model management.
- **Data poisoning** involves manipulating training data to influence model behavior.
- **Model theft** occurs when attackers obtain unauthorized copies of proprietary or sensitive AI models.
- **Adversarial attacks** attempt to manipulate model inputs or interactions to produce unintended behavior.
- **Prompt injection** is a technique used to manipulate generative AI applications through malicious instructions.
- Input and output safeguards help prevent malicious inputs, sensitive-data leakage, and harmful generated content.
- **SAIF** provides a framework for integrating security into AI development and deployment.
- Google Cloud security capabilities such as IAM, encryption, and Security Command Center help organizations protect their cloud environments.
- Continuous monitoring, threat intelligence, software updates, and human oversight are essential for maintaining secure AI systems.

## 7. Quick Review Questions

**1. What does Secure AI mean?**

Protecting AI systems from intentional harm, malicious attacks, unauthorized access, and misuse throughout their lifecycle.

**2. What is data poisoning?**

A malicious attack in which an attacker introduces manipulated or incorrect information into an AI model's training dataset, potentially causing it to learn harmful or inaccurate patterns.

**3. What is model theft?**

The unauthorized acquisition or copying of a proprietary or sensitive AI model.

**4. What is an adversarial attack?**

An attack that deliberately manipulates inputs or interactions to trick an AI model into producing incorrect or unintended results.

**5. What is prompt injection?**

An attack that introduces malicious instructions through user input or external content to manipulate a generative AI application's behavior.

**6. Why is encryption important in AI security?**

It helps protect sensitive information from unauthorized access, particularly when data is stored or transmitted.

**7. What is IAM?**

Identity and Access Management. It controls who can access resources and what actions they are authorized to perform.

**8. What is Google's SAIF?**

The Secure AI Framework, a framework developed by Google to guide organizations in securing AI systems and managing AI-related security risks.

**9. What is the purpose of Security Command Center?**

It provides centralized visibility into security risks, vulnerabilities, and the security posture of Google Cloud environments.

**10. Why must AI security be continuously monitored?**

Because threats and vulnerabilities evolve over time. Continuous monitoring helps organizations detect suspicious activities, identify weaknesses, and maintain effective security controls.
