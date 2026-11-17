
# 🔎 Retrieval-Augmented Generation (RAG) and Tooling

## 1. Pre-RAG History

Before Retrieval-Augmented Generation (RAG):
- LLMs relied primarily on information learned during their training.
- They could use tools to retrieve external information but had limited ability to process and integrate that information into their knowledge.
- Retrieved data was generally used only to answer the immediate query.
- Their responses could become outdated or lack information not included in their training data.

**RAG addresses these limitations** by allowing LLMs to retrieve relevant external information and incorporate it into their responses.

## 2. How RAG Works with Tools

### 🔍 What Is RAG?
- **Retrieval-Augmented Generation (RAG)** enhances LLMs by grounding their responses in external knowledge sources.
- It allows models to access and process information beyond their original training data.
- This helps produce more:
  - Accurate responses
  - Relevant answers
  - Up-to-date information
  - Contextually appropriate outputs
- RAG can also support source citations, improving transparency and trustworthiness.

### 🧰 Retrieval Tools and Knowledge Sources

An LLM can use different tools to retrieve information:

| Tool / Knowledge Source | Description | Example |
|---|---|---|
| **Data stores** | Internal databases and repositories containing structured or unstructured information. | Customer databases, company documents |
| **Vector databases** | Store embeddings (numerical representations of information) to find semantically similar content. | Searching documents based on meaning rather than exact keywords |
| **Search engines** | Retrieve relevant information from websites and online sources through APIs or extensions. | Google Search, online news |
| **Knowledge graphs** | Store information about entities and their relationships. | Connecting people, organizations, locations, and events |

### 🧠 Understanding Vector Databases
- **Embeddings** are numerical representations of text or other information.
- They capture semantic meaning, allowing systems to identify related content even when exact keywords differ.
- Basic retrieval process:
  1. Convert the user's query into an embedding.
  2. Search the vector database for semantically similar embeddings.
  3. Retrieve matching documents or passages.
  4. Provide the retrieved information to the LLM as context.

### ⚙️ The RAG Process

RAG follows three main stages, with optional iteration:

#### 1. Retrieval
- The user submits a question or request.
- The LLM uses retrieval tools to search external knowledge sources.
- Relevant documents, passages, or information are retrieved.

#### 2. Augmentation
- The retrieved information is added to the original user prompt.
- The augmented prompt contains:
  - The user's original question.
  - Relevant external information retrieved by the tools.

#### 3. Generation
- The LLM processes the augmented prompt.
- It generates an answer grounded in the retrieved information.
- It can cite the sources used to support its response.

#### 4. Iteration (Optional)
- If the retrieved information is insufficient, the LLM can:
  - Refine its search query.
  - Use different retrieval tools.
  - Search additional data sources.
  - Ask the user clarifying questions.
- The process repeats until sufficient information is gathered or the task reaches its stopping point.

### 🔄 RAG Workflow

```text
User submits a query
        |
        v
   RETRIEVAL
        |
        v
Search external knowledge sources
(Data stores, vector databases,
search engines, knowledge graphs)
        |
        v
Retrieve relevant information
        |
        v
  AUGMENTATION
        |
        v
Combine original query
with retrieved information
        |
        v
   GENERATION
        |
        v
LLM generates a grounded response
        |
        v
Are the results sufficient?
        |
   +----+----+
   |         |
  Yes        No
   |         |
   v         v
Respond   Refine query or
with      retrieve more data
sources       |
              +----> Repeat
```

## 3. 🌍 Example: Answering a Question About a Recent Event

**User query:**

"What were the main developments at the recent climate conference in Dubai?"

| Stage | What Happens |
|---|---|
| **1. User Query** | The user asks about the latest developments at the climate conference. |
| **2. Retrieval** | The LLM searches a vector database of climate-related news articles and uses a search engine to find recent reports and official conference documents. |
| **3. Augmentation** | The retrieved summaries of discussions, agreements, and announcements are combined with the user's original question. |
| **4. Generation** | The LLM summarizes the main developments and cites the news articles and official documents used. |
| **5. Iteration (Optional)** | If the results are incomplete, the LLM refines its search terms or queries additional sources. |

**Result:** The LLM produces a more comprehensive and current answer than one based solely on its original training data.

## 4. 🗄️ Data Stores

### What Are Data Stores?
- Data stores are structured and unstructured knowledge repositories that AI applications and agents can access.
- They are important components of RAG because they provide external information for retrieval and response generation.
- They allow agents to use organizational data, documents, and online information.

### Types of Data Stores

| Data Store Type | Description | Examples |
|---|---|---|
| **Websites** | Allow agents to access and process information directly from web pages. | Public websites, online articles, current events |
| **Structured Data** | Information organized into defined formats, such as tables or JSON. | Product catalogs, customer databases, internal knowledge bases |
| **Unstructured Data** | Information stored in files without a rigid tabular structure. | HTML, PDF, DOCX documents |

### Data Stores in Google Agent Platform
- Agents can connect to different data sources through AI Applications.
- For structured data:
  - The platform can automatically understand the data structure.
  - Developers can also define the structure themselves.
- For unstructured data:
  - Agents can retrieve and use information from documents in different file formats.
- These capabilities allow agents to use organizational knowledge when responding to user queries.

## 5. 🔑 Key Takeaways

- **RAG** enhances LLMs by retrieving external information and incorporating it into generated responses.
- **Retrieval** finds relevant information from external knowledge sources.
- **Augmentation** combines retrieved information with the original user prompt.
- **Generation** produces a response grounded in the retrieved context.
- **Iteration** allows the agent to improve retrieval when initial results are insufficient.
- **Vector databases** use embeddings to find semantically similar information.
- **Knowledge graphs** represent entities and their relationships.
- **Data stores** provide the structured and unstructured knowledge that agents need.

### 🧠 RAG vs. Traditional LLM

| Traditional LLM | LLM with RAG |
|---|---|
| Primarily relies on training data. | Can retrieve external information. |
| May lack recent or organization-specific information. | Can access updated and organization-specific data sources. |
| Generates responses based on its existing knowledge and prompt. | Generates responses using the original prompt and retrieved context. |
| May not provide verifiable sources. | Can cite retrieved sources when source information is available. |

**Remember:** RAG does not automatically retrain or permanently teach the model. It retrieves relevant external information and supplies it as context for generating a response.
