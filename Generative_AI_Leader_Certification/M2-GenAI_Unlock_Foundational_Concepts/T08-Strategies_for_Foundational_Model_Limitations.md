# Google Strategies for Foundation Model Limitations

## 1. Introduction: Why Grounding Is Important

Generative AI is transforming many areas of work, including marketing, software development, research, and data analysis. However, despite its ability to generate creative and useful content, it can sometimes produce information that is inaccurate, misleading, or completely fabricated. This behavior is known as **AI hallucination**.

### What is Grounding?

**Grounding** is the process of connecting a generative AI model's responses to specific, reliable sources of information. It provides additional context and evidence so that the model can generate more accurate, relevant, and organization-specific answers.

Think of grounding as a reality check for AI. Instead of relying only on patterns learned during training, the model can use relevant information from external or organizational sources.

In an enterprise environment, grounding can connect AI applications to:

- Internal documents and reports
- Company policies and procedures
- Customer and operational data
- Databases and knowledge repositories
- Source code and technical documentation

**Example:**

An employee asks an AI assistant:

> What were our organization's total expenses for the third quarter?

Without grounding, the model might generate a plausible but incorrect answer because it does not have access to the organization's actual financial records.

With grounding, the AI can retrieve relevant financial reports or database records and use them to formulate an answer based on the available information.

### Why Is Grounding Important?

Grounding helps organizations:

1. **Improve accuracy:** Connect generated responses to relevant information and reliable sources.
2. **Provide relevant answers:** Give the model organization-specific context rather than generic responses.
3. **Reduce hallucinations:** Help prevent unsupported or fabricated information.
4. **Improve trustworthiness:** Make it easier to verify where an answer came from.
5. **Support enterprise applications:** Enable AI assistants to work with organizational knowledge and information.

> **Key takeaway:** Grounding connects AI-generated responses to relevant information. It does not guarantee that every answer will be correct, so source verification and human review remain important.

### Grounding, Fine-Tuning, and RAG

This lesson introduces two important strategies for improving how foundation models work with specialized information:

- **Fine-tuning:** Further training an existing model on a specialized dataset to adapt its behavior or improve its performance on particular tasks.
- **Retrieval-Augmented Generation (RAG):** Retrieving relevant information from external sources and providing it to the model as context when generating a response.

These approaches will be discussed in more detail in the succeeding lessons.

## 2. Foundation Model Limitations

Foundation models are powerful because they are trained on large and diverse datasets. However, they still have limitations that can affect their accuracy, reliability, fairness, and usefulness.

Understanding these limitations is essential when selecting, implementing, and managing generative AI solutions.

### 2.1 Data Dependency

The performance of foundation models depends heavily on the quality, quantity, and diversity of their training data.

If the training dataset contains inaccurate, incomplete, outdated, or biased information, these problems can influence the model's outputs.

**Example:**

Imagine asking a student to write an essay about a book they have never read. The student may produce an answer based on limited information or incorrect assumptions.

Similarly, an AI model cannot reliably learn information that is missing or poorly represented in its training data.

**Key considerations:**
- Models require substantial amounts of training data.
- Incomplete datasets can result in limited knowledge.
- Incorrect information can influence generated responses.
- Poor-quality data can reduce model performance.

### 2.2 Knowledge Cutoff

A **knowledge cutoff** refers to the point in time up to which information was included in a model's training data.

A model with an older knowledge cutoff may not know about recent events, discoveries, policy changes, or developments that occurred afterward.

Foundation models do not automatically update their knowledge whenever new information becomes available.

**Example:**

If an AI model was trained using information available only up to 2022, it may not know about:
- Government policies introduced in 2023 or later.
- Recent scientific discoveries.
- New technologies released after its training period.
- Recent economic or statistical developments.

**How to address this limitation:**

Organizations can connect AI applications to updated external information sources through approaches such as RAG, web search, or database integration.

> **Important:** A model's knowledge cutoff is not necessarily the same as the date of its latest update or deployment. Some AI applications can access current information through external tools even when their underlying model has a fixed training cutoff.

### 2.3 Bias

**Bias** occurs when a model produces systematically skewed or unbalanced outputs.

Large language models learn from extensive datasets that may contain historical, social, cultural, or other forms of bias. Because models learn patterns from their training data, they can reproduce or even amplify these existing biases.

**Example:**

Suppose a model is trained using employment datasets in which certain demographic groups are underrepresented in leadership positions.

The model may learn patterns that associate leadership roles with the groups that appear more frequently in those positions. As a result, its generated recommendations may unintentionally reinforce existing stereotypes.

**Key considerations:**
- Bias can originate from unrepresentative training data.
- Historical inequalities may be reflected in generated outputs.
- Models can reproduce stereotypes and discriminatory patterns.
- Bias can affect recommendations, classifications, and decision-support applications.

**How to address this limitation:**
- Use diverse and representative datasets.
- Evaluate model outputs across different demographic groups.
- Conduct regular bias assessments.
- Apply responsible AI practices and human oversight.

### 2.4 Fairness

**Fairness** refers to the challenge of ensuring that AI systems treat individuals and groups equitably.

Even when a dataset is balanced, determining whether an AI model is fair is not straightforward. Fairness can have different interpretations depending on the application, affected groups, and desired outcomes.

For example, an AI system used for evaluating job applicants may be assessed based on whether:
- Different demographic groups have comparable opportunities.
- The model applies consistent evaluation criteria.
- Its recommendations do not unfairly disadvantage particular groups.

Fairness assessments and benchmarks can help identify certain forms of bias, but they cannot capture every possible fairness concern.

**Key considerations:**
- Fairness has multiple definitions and measurement approaches.
- Balanced datasets do not automatically guarantee fair outcomes.
- Evaluation benchmarks may cover only specific types of bias.
- Fairness must be considered in the context of the actual application.

> **Key takeaway:** Bias concerns patterns in data and model outputs, while fairness concerns whether the resulting treatment and outcomes are equitable. Addressing one does not automatically resolve the other.

### 2.5 Hallucinations

**Hallucination** occurs when a generative AI model produces information that is inaccurate, fabricated, misleading, or unsupported by reliable evidence.

A response may sound confident and convincing even when the information is incorrect.

This happens because foundation models generate outputs by learning and predicting patterns rather than automatically verifying every statement against real-world facts.

**Examples:**
- Inventing academic references or research publications.
- Providing incorrect statistics or financial figures.
- Citing government policies that do not exist.
- Generating code containing incorrect functions or logic.
- Giving outdated information as if it were current.

**Why are hallucinations concerning?**

They can create serious problems in applications where accuracy is critical, such as:
- Government policy research and statistical reporting.
- Healthcare and medical information.
- Financial analysis and reporting.
- Legal research and regulatory compliance.
- Public information and decision support.

**How to address this limitation:**
- Ground responses using reliable and relevant sources.
- Use RAG to retrieve supporting information.
- Ask the model to identify its sources.
- Verify important claims against authoritative references.
- Require human review for high-impact decisions.

> **Important:** Grounding can reduce hallucinations, but it does not eliminate them. A model may still misunderstand retrieved information or generate unsupported conclusions.

### 2.6 Edge Cases

**Edge cases** are rare, unusual, or atypical situations that fall outside the common patterns encountered during model training.

Foundation models may perform well under normal conditions but struggle when presented with unfamiliar situations or unusual combinations of information.

**Examples:**
- A government chatbot receiving an unusual combination of questions about multiple policies.
- An image recognition model encountering an object under unusual lighting conditions.
- A data analysis assistant processing an unfamiliar date format or an unexpected data structure.
- A language model interpreting a highly specialized technical term or uncommon local expression.

**Why are edge cases challenging?**

Models learn patterns from their training data. When they encounter situations that differ significantly from those patterns, they may produce errors, misunderstand the input, or generate unexpected responses.

**How to address this limitation:**
- Test models using diverse and unusual scenarios.
- Include representative edge cases in evaluation datasets.
- Monitor performance after deployment.
- Provide fallback mechanisms when the model cannot confidently answer.
- Maintain human intervention for exceptional or high-risk cases.

## 3. Summary: Foundation Model Limitations

| Limitation | Description | Possible impact |
|---|---|---|
| Data dependency | Model performance depends on the quality and completeness of training data. | Inaccurate or incomplete outputs |
| Knowledge cutoff | The model may not know information introduced after its training period. | Outdated answers |
| Bias | The model may reproduce or amplify biases in its training data. | Skewed or discriminatory outputs |
| Fairness | Ensuring equitable treatment and outcomes is difficult to define and measure. | Unfair decisions or recommendations |
| Hallucinations | The model may generate fabricated or unsupported information. | Misleading or incorrect responses |
| Edge cases | The model may struggle with rare or unusual situations. | Unexpected errors and unreliable outputs |

## 4. Practical Application: Government and Statistical Work

These limitations are particularly important when using generative AI in government agencies and statistical institutions.

| Application | Potential limitation | Recommended consideration |
|---|---|---|
| Statistical report generation | Hallucinated figures or incorrect interpretations | Verify figures against official statistical datasets. |
| Policy research | Knowledge cutoff and outdated references | Use updated government publications and authoritative sources. |
| CBMS data analysis | Data dependency and incomplete records | Validate data quality, completeness, and representativeness. |
| Public service chatbot | Incorrect policy information | Ground responses in updated official policies and guidelines. |
| Program prioritization | Bias and fairness concerns | Review criteria and assess potential impacts on different communities. |
| Document processing | Edge cases involving unusual formats or terminology | Test different document structures and provide human review. |

## 5. Key Takeaways

- Foundation models have limitations despite their advanced capabilities.
- The quality and diversity of training data significantly influence model performance.
- Knowledge cutoffs can cause models to provide outdated information.
- Bias and fairness are related but distinct challenges in responsible AI.
- Hallucinations can produce convincing but inaccurate information.
- Edge cases expose weaknesses that may not appear during ordinary use.
- Grounding, fine-tuning, RAG, evaluation, and human oversight are important strategies for addressing these limitations.

## 6. Quick Review Questions

**1. What is grounding in generative AI?**

Grounding connects AI-generated responses to specific, relevant information sources to improve accuracy and relevance.

**2. What is a knowledge cutoff?**

It is the point in time up to which information was included in a model's training data.

**3. Why can foundation models produce biased outputs?**

Because their training data may contain historical, social, or demographic biases that the model can learn and reproduce.

**4. Does a balanced dataset guarantee fairness?**

No. Fairness has multiple definitions and depends on the context, application, and outcomes being evaluated.

**5. What is an AI hallucination?**

It occurs when a model generates inaccurate, fabricated, or unsupported information that may sound convincing.

**6. What are edge cases?**

They are rare or unusual situations that may fall outside the common patterns encountered during model training.

**7. What are two strategies for grounding generative AI models?**

Fine-tuning and Retrieval-Augmented Generation (RAG). However, they work differently: fine-tuning adapts the model through additional training, while RAG supplies relevant external information during response generation.
