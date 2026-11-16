
# ☁️ Google's Agent Tooling

## 📖 Introduction

Google Cloud provides a wide range of services and APIs that can be integrated into generative AI agents.

Agents can use:
- **Custom-built tools** developed for specific requirements.
- **Third-party solutions** that provide external integrations.
- **Google Cloud tools and services** that provide storage, databases, computing, and AI capabilities.

💡 Many Google Cloud tools can also be integrated into agents whose core logic is developed outside Google Cloud.

## 1. 🛠️ Key Google Cloud Tools for Agents

### 1. Cloud Storage

- Highly scalable and durable object storage service.
- Allows agents to store and retrieve data needed to perform tasks.
- Useful for storing documents, files, images, and other data.

### 2. 🗄️ Databases

Google Cloud offers different database solutions that agents can use to store and retrieve information.

| Database Service | Description |
|---|---|
| **Cloud SQL** | Managed relational database service |
| **Cloud Spanner** | Globally scalable relational database service |
| **Firestore** | NoSQL document database |

**Agent use cases:**
- Store and retrieve information.
- Manage user data.
- Track agent progress.
- Maintain application records.

### 3. ⚙️ Cloud Run Functions

- Provides serverless functions that act as specialized tools for agents.
- Can execute specific tasks when triggered by an agent.
- Automatically scales based on demand.

**Possible functions:**
- Connect to databases.
- Call external APIs.
- Perform complex calculations.
- Handle other specialized operations.

### 4. 🐳 Cloud Run

- A serverless platform for deploying and running stateless containers.
- Suitable for more complex agent tools requiring containerized environments.
- Useful when custom tools need:
  - Specific software dependencies.
  - Custom runtime environments.
  - Greater control over execution.

### 5. 🤖 Agent Platform

- Allows agents to use other agents as tools.
- Developers can create models or agents through Agent Platform.
- These agents can then be called by other agents to perform specialized tasks.

**Concept:** One agent can delegate a specific task to another agent, enabling collaboration between specialized agents.

## 2. 🧠 Pre-built AI APIs

Google Cloud provides pre-built AI APIs that agents can use to perform specialized tasks without building every capability from scratch.

### 1. 🎙️ Speech-to-Text API

- Converts spoken audio into text.
- Useful for:
  - Meeting transcription.
  - Customer service call transcription.
  - Video transcription.

### 2. 🔊 Text-to-Speech API

- Converts written text into natural-sounding speech.
- Useful for:
  - Voice user interfaces.
  - Voice-enabled applications and devices.
  - Personalized audio communication.

### 3. 🌐 Translation API

- Translates text, documents, websites, and supported audio and video content.
- Supports more than 135 languages, as stated in the course material.

### 4. 📄 Document Translation API

- Translates formatted documents.
- Preserves the original document layout during translation.

### 5. 📑 Document AI API

- Extracts information from different document formats.
- Automates document processing and data capture.
- Supports documents such as:
  - Invoices.
  - Contracts.
  - Medical records.
- Can also summarize large documents using generative AI.

### 6. 🖼️ Cloud Vision API

- Uses machine learning to understand image content.
- Capabilities include:
  - Object detection.
  - Face detection.
  - Landmark detection.
  - Optical Character Recognition (OCR) to extract text from images.

**Use cases:**
- Image tagging.
- Content moderation.
- Visual search.

### 7. 🎬 Cloud Video Intelligence API

- Analyzes video content and extracts meaningful information.
- Can identify:
  - Objects.
  - Actions.
  - Events.
  - Spoken words through transcription.

**Use cases:**
- Content recommendation.
- Video search.
- Media analysis.

### 8. 📝 Natural Language API

- Uses machine learning to analyze unstructured text.
- Extracts useful insights from written content.

**Capabilities:**
- Sentiment analysis.
- Content classification.
- Entity extraction, including:
  - People.
  - Places.
  - Events.
- Supports text analysis in multiple languages.

## 3. 🌐 Other Google Cloud APIs

Google Cloud provides an extensive **API Library** containing APIs connected to various Google products and services.

Examples include:
- Google Maps.
- Google Workspace.
- YouTube.
- Google Photos.
- Other Google services.

🔗 **API Library:** https://console.cloud.google.com/apis/library

## 4. 📍 Agent Tooling Example: Meeting Location Planner

### Scenario

A user uploads a document, such as:
- A meeting invitation.
- A list of potential conference venues.
- A document containing attendee addresses.

The user asks the agent to recommend the most convenient meeting location for all attendees.

The agent combines **Document AI, Google Maps API, and custom logic** to analyze the information and recommend a suitable location.

### 🔄 Workflow

#### 1. 📄 Document Processing – Document AI API

- The agent processes the uploaded document using Document AI.
- Extracts relevant information, particularly addresses mentioned in the document.

**Output:** A list of extracted addresses.

#### 2. 🌍 Geocoding – Google Maps Geocoding API

- The agent sends the extracted addresses to the Google Maps Geocoding API.
- Converts addresses into geographic coordinates:
  - Latitude.
  - Longitude.
- These coordinates can be used to calculate distances and travel times.

**Output:** Geographic coordinates for each address.

#### 3. 🧮 Location Analysis – Custom Logic

- The agent uses custom logic implemented through a Cloud Function.
- Analyzes the geocoded addresses.
- Determines a suggested meeting location based on the location data.

**Output:** A recommended meeting location for the attendees.

### 📌 Workflow Summary

```text
👤 User Uploads Meeting Document
              ↓
📄 Document AI API
   Extract Addresses
              ↓
🌍 Google Maps Geocoding API
   Convert Addresses into Coordinates
              ↓
🧮 Cloud Function
   Analyze Locations and Distances
              ↓
📍 Recommend Convenient Meeting Location
              ↓
💬 Agent Presents Recommendation
```

## 🔑 Key Takeaways

- Google Cloud offers a wide range of tools for building capable AI agents.
- Important infrastructure and computing services include:
  - **Cloud Storage:** Stores and retrieves files and data.
  - **Databases:** Manage and retrieve structured or unstructured information.
  - **Cloud Run Functions:** Execute specialized serverless operations.
  - **Cloud Run:** Runs custom containerized tools.
  - **Agent Platform:** Enables agents to use other agents as tools.
- Pre-built AI APIs provide specialized capabilities:
  - **Speech-to-Text:** Speech-to-text conversion.
  - **Text-to-Speech:** Text-to-audio conversion.
  - **Translation:** Language translation.
  - **Document Translation:** Translates documents while preserving layout.
  - **Document AI:** Extracts and processes document information.
  - **Cloud Vision:** Analyzes images and extracts text.
  - **Cloud Video Intelligence:** Analyzes video content.
  - **Natural Language:** Analyzes and extracts insights from text.
- Google Cloud APIs can be combined to build complete agent workflows.
- The Meeting Location Planner demonstrates how an agent can combine document processing, geocoding, and custom logic to solve a real-world problem.

💡 **Remember:** Google Cloud provides the infrastructure, databases, functions, and AI APIs that allow agents to access information, process data, and perform real-world tasks.
