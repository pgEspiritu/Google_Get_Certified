
# ⚓ Grounding

## 1. 📌 Introduction

- **Grounding** refers to the ability of an AI model to connect its generated outputs to specific, verifiable sources of information.
- It provides additional context and reference materials that help AI models generate more accurate, relevant, and reliable responses.
- Grounding can be implemented without programming by:
  - Attaching documents and resources to a custom Gem.
  - Uploading reference files in Gemini prompts.
  - Providing relevant information directly within prompts.
- **Purpose of Grounding:**
  - 🎯 Improve the accuracy and relevance of AI-generated responses.
  - 📚 Connect AI outputs to trusted reference materials.
  - 🔎 Provide context specific to a task or organization.
  - 🛡️ Improve the reliability and trustworthiness of AI systems.
  - ⚙️ Reduce the likelihood of AI hallucinations.

## 2. 📚 Practical Application of Grounding

- **Scenario:** An employee wants to use Gemini to edit documents according to their organization's writing guidelines.
- **Process:**
  1. Provide Gemini with the document that needs editing.
  2. Upload the organization's writing guidelines or style guide.
  3. Instruct Gemini to review and revise the document based on the provided references.
  4. Gemini uses the additional information as context when generating the revised document.
- **Example prompt:**

  ```text
  Review and edit the following document based on the attached
  organizational writing guidelines.

  Ensure that the revised document follows the prescribed writing
  style, tone, formatting, and terminology.

  Highlight any sections that do not comply with the guidelines.
  ```

- **Expected benefits:**
  - Produces content aligned with organizational standards.
  - Reduces inconsistencies in writing and formatting.
  - Provides more contextually relevant recommendations.
  - Improves the accuracy and usefulness of AI-generated content.

## 3. 🧠 RAG: Retrieval-Augmented Generation

- **Retrieval-Augmented Generation (RAG)** is a grounding technique that enhances generative AI by retrieving relevant information from external knowledge sources before generating a response.
- Instead of relying exclusively on the model's existing knowledge, RAG provides additional information retrieved from relevant databases, documents, or other sources.
- **Main purpose:**
  - Provide relevant external knowledge to the AI model.
  - Improve the accuracy and relevance of generated responses.
  - Help address limitations associated with outdated or incomplete model knowledge.
  - Reduce the likelihood of hallucinations.

### 3.1. ⚙️ How RAG Works

RAG involves two major processes:

- **1. 🔎 Retrieving Relevant Information**
  - The system searches for information relevant to the user's prompt.
  - Information can be retrieved from:
    - Databases.
    - Document collections.
    - Organizational knowledge bases.
    - External websites and the internet.
  - Retrieval can use technologies such as:
    - **Semantic Search:** Finds information based on meaning and context rather than relying only on exact keyword matches.
    - **Vector Databases:** Store and retrieve information using numerical representations called vectors or embeddings.
  - The retrieved information is provided to the AI model as additional context.

- **2. ✍️ Generating Output**
  - The AI model receives the original user prompt together with the retrieved information.
  - It uses the additional context to generate a response.
  - Possible outputs include:
    - Answers to questions.
    - Summaries of documents.
    - Reports and analyses.
    - Other AI-generated content.

### 3.2. 🤖 Model Only (Without RAG)

- The user submits a prompt directly to the AI model.
- The model generates a response primarily using its existing learned knowledge and the information included in the prompt.
- No external retrieval system is used to obtain additional knowledge.
- **Limitations:**
  - Responses may rely on outdated information.
  - The model may lack access to specific organizational documents or recent developments.
  - There is a greater risk of generating inaccurate information or hallucinations.

**Process:**

1. User submits a prompt.
2. AI model processes the prompt.
3. Model generates an output using its existing knowledge.

### 3.3. 🔗 Model with RAG

- The user submits a prompt to the AI application.
- The system sends a query to an external retrieval system, such as a search engine or vector database.
- The retrieval system identifies relevant information from available knowledge sources.
- The retrieved information is added to the prompt as additional context.
- The AI model generates an output using both the original prompt and the retrieved information.
- **Benefits:**
  - Access to relevant external and potentially updated information.
  - More contextually accurate responses.
  - Reduced likelihood of hallucinations.
  - Better alignment with specific knowledge bases and reference documents.

**Process:**

1. User submits a prompt.
2. Retrieval system searches for relevant information.
3. Relevant information is retrieved from external sources.
4. Retrieved information is incorporated into the model's context.
5. AI model generates an output using the provided information.

## 4. 📊 Comparison: Model Without RAG vs. Model With RAG

| Aspect | Model Without RAG | Model With RAG |
|---|---|---|
| Knowledge Source | Existing learned knowledge and prompt context | Existing learned knowledge plus retrieved external information |
| Information Retrieval | No external retrieval | Uses search engines, databases, or document repositories |
| Context | Limited to available model knowledge and user input | Enriched with relevant retrieved information |
| Information Freshness | May be outdated | Can access updated information from connected sources |
| Accuracy | May be less reliable for specialized or current information | Can improve accuracy through relevant references |
| Hallucination Risk | Higher likelihood | Reduced likelihood, but not eliminated |
| Best Use Case | General knowledge and creative tasks | Document-based question answering and knowledge-intensive tasks |

## 5. 🎯 Key Takeaways

- **Grounding** connects AI-generated outputs to specific and verifiable information sources.
- Users can improve grounding by providing relevant documents, reference materials, and organizational guidelines directly in Gemini or custom Gems.
- **RAG (Retrieval-Augmented Generation)** is a technique that retrieves relevant external information before generating an AI response.
- RAG has two main stages:
  - 🔎 **Retrieval:** Find relevant information from external knowledge sources.
  - ✍️ **Generation:** Use the retrieved information to produce a response.
- Semantic search and vector databases are technologies that can support the retrieval process.
- Grounding and RAG help improve response relevance and reduce the likelihood of hallucinations.
- 💡 **Remember:** Grounding provides AI with reliable reference information, while RAG adds an automated retrieval process that allows the model to use relevant external knowledge when generating responses.
- ⚠️ **Important:** Grounding and RAG do not guarantee factual accuracy. Retrieved information may be incomplete, outdated, or incorrect, so important outputs should still be verified against their original sources.

## 6. 🔗 Additional Learning Resources

- [What Is Semantic Search? – Google Cloud](https://cloud.google.com/discover/what-is-semantic-search?hl=en)
- [What Is a Vector Database? – Google Cloud](https://cloud.google.com/discover/what-is-a-vector-database?hl=en)
