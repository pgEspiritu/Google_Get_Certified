# 📂 Understanding Data Types

## 📌 1. Introduction: Understanding Data Types

Data is central to many business processes and plays an important role in Machine Learning (ML) and Artificial Intelligence (AI).

Organizations use different types of data to:
- Understand customer behavior and preferences.
- Optimize business operations.
- Improve products and services.
- Support evidence-based decision-making.
- Develop AI and ML applications.

Larger datasets can often improve model performance, particularly for complex Generative AI models that produce diverse content. However, **having a large dataset does not automatically guarantee better results.**

Model performance also depends on:
- **Data volume:** The amount of available data.
- **Data organization:** How the information is arranged.
- **Data structure:** How the data is stored and represented.
- **Data quality:** Whether the information is accurate, complete, consistent, representative, and relevant.

Understanding an organization's data, including its quality, availability, and format, helps determine what AI applications can realistically be developed.

## 🗂️ 2. Data Forms: Structured and Unstructured Data

Data comes in different forms. Broadly, it can be categorized into two main types:

1. **Structured Data**
2. **Unstructured Data**

To understand the difference, consider a fictional company called **Cymbal Cleaning**, which sells eco-friendly cleaning supplies.

Its customer order records may contain the following information:

- Customer ID
- Customer name
- Purchase date
- Order cost
- Delivery address
- Product image
- Customer feedback (1–5 star rating)
- Written customer feedback
- Email content

Although these details belong to the same business process, they do not all have the same data structure.

## 📊 3. Structured Data

**Structured data** is information organized according to a predefined format or structure, typically arranged in rows and columns.

It is relatively easy to search, filter, sort, and analyze because each data field follows an established format.

A familiar example is the contact list on a mobile phone, where names, phone numbers, and addresses are organized into identifiable fields.

### Characteristics

- Organized into rows and columns.
- Follows a predefined structure or schema.
- Uses clearly defined fields and data types.
- Easy to search, filter, sort, and query.
- Commonly stored in relational databases.

### Examples

- Customer records
- Online shopping transactions
- Bank statements
- Employee databases
- Inventory records
- Statistical datasets

### Example: Cymbal Cleaning Customer Database

The following information can be stored as structured data:

| Customer ID | Customer Name | Purchase Date | Order Cost | Feedback Rating |
|---|---|---|---:|---:|
| C001 | Maria Santos | 2026-10-15 | ₱1,250 | 5 |
| C002 | Juan Reyes | 2026-10-16 | ₱850 | 4 |
| C003 | Ana Cruz | 2026-10-17 | ₱1,500 | 5 |
| C004 | Pedro Garcia | 2026-10-18 | ₱950 | 3 |

Each column represents a specific field, while each row represents an individual customer transaction.

### Where Is Structured Data Stored?

Structured data is commonly stored in a **relational database**, which organizes information into tables with defined relationships.

Examples of database management systems include:
- MySQL
- PostgreSQL
- Microsoft SQL Server
- Oracle Database
- SQLite

Structured data can also be stored in spreadsheets such as Microsoft Excel and Google Sheets.

## 🖼️ 4. Unstructured Data

**Unstructured data** is information that does not follow a predefined tabular structure or fixed schema.

Unlike structured data, it cannot be easily organized into conventional rows and columns without additional processing.

It is often more complex because it can contain different types of content, such as text, images, audio, and video.

### Characteristics

- Does not follow a fixed tabular structure.
- Can contain different forms of information.
- Requires specialized tools or techniques for analysis.
- May require preprocessing before it can be used in ML models.
- Commonly stored as documents, media files, or other digital content.

### Examples

- PDF documents
- Emails and social media posts
- Photographs and digital artwork
- Medical images and scans
- Speech recordings
- Music files
- Videos and smartphone recordings

### Example: Cymbal Cleaning Customer Records

The following information can be considered unstructured data:

| Data | Example |
|---|---|
| Written Feedback | "The cleaning product works well, but delivery took too long." |
| Product Image | Photograph of a cleaning product uploaded by a customer. |
| Email Content | A customer's email asking about product ingredients or delivery status. |

These data types do not naturally fit into a predefined table with fixed fields and values.

However, AI techniques can help extract useful information from them.

For example:
- **Natural Language Processing (NLP):** Analyze written feedback and email content.
- **Computer Vision:** Identify products or objects in uploaded photographs.
- **Speech Recognition:** Convert audio recordings into text.
- **Generative AI:** Summarize customer feedback or draft email responses.

## ⚖️ 5. Structured vs. Unstructured Data

| Feature | Structured Data | Unstructured Data |
|---|---|---|
| Organization | Predefined structure | No fixed structure |
| Format | Rows and columns | Text, images, audio, video, and documents |
| Storage | Relational databases and spreadsheets | File systems, document repositories, media storage, and other platforms |
| Searching | Generally easier using queries and filters | Often requires specialized search and processing techniques |
| Analysis | Conventional querying and statistical tools | May require NLP, computer vision, or other AI techniques |
| Example | Customer ID, purchase date, and order cost | Customer emails, product images, and videos |

## 🏛️ 6. Practical Application in Government and Statistical Work

Government agencies handle both structured and unstructured data.

Understanding the difference helps determine which tools and techniques are appropriate for processing and analyzing government information.

| Government Data | Classification | Example Application |
|---|---|---|
| Population records | Structured | Population analysis and demographic profiling. |
| Household survey responses with predefined fields | Structured | Statistical tabulation and poverty analysis. |
| Government financial records | Structured | Budget monitoring and expenditure analysis. |
| Research reports in PDF format | Unstructured | Document summarization and information extraction. |
| Citizen feedback and complaints | Unstructured | Sentiment analysis and classification of concerns. |
| Photographs of infrastructure projects | Unstructured | Image analysis and project documentation. |
| Recorded interviews | Unstructured | Speech-to-text transcription and qualitative analysis. |

**Example: CBMS and Local Government Planning**

A local government may use structured CBMS data, such as household characteristics, education, employment, and access to basic services, to generate statistical indicators and identify development priorities.

Meanwhile, unstructured information, such as community feedback, research reports, and supporting photographs, may provide additional context for interpreting local conditions.

Combining different data types can help organizations develop more comprehensive analyses and support evidence-based planning.

## 🔑 7. Key Takeaways

1. **Data is not limited to numbers.** It can include text, images, audio, video, dates, and other forms of information.
2. **Structured data follows a predefined format.** It is commonly organized into rows and columns and stored in relational databases.
3. **Unstructured data does not follow a fixed tabular structure.** Examples include emails, PDF documents, photographs, audio, and videos.
4. **Both data types are useful for AI.** Different AI techniques can process different forms of information.
5. **Data volume is not the only consideration.** Data quality, organization, structure, and relevance also affect model performance.
6. **Understanding organizational data is important.** It helps determine which AI applications are feasible and what preparation is needed.

## 📝 Quick Review

**1. What are the two broad categories of data?**

Structured data and unstructured data.

**2. What is structured data?**

Data organized according to a predefined structure, typically in rows and columns.

**3. What is unstructured data?**

Data that does not follow a predefined tabular structure, such as documents, emails, images, audio, and videos.

**4. Where is structured data commonly stored?**

Relational databases and spreadsheets.

**5. Is customer feedback structured or unstructured?**

It depends on its format:
- A numerical rating from 1 to 5 is structured data.
- A written customer comment is unstructured data.

**6. What AI technologies can help process unstructured data?**

- Natural Language Processing for text.
- Computer Vision for images.
- Speech Recognition for audio.
- Generative AI for tasks such as summarization and content generation.

**7. Does having a larger dataset automatically guarantee better AI performance?**

No. Data quality, relevance, organization, and structure are also important.

**8. Why should organizations understand their data before implementing AI?**

Because understanding the data's type, quality, availability, and format helps determine whether it can support the intended AI application and what preparation is required.
