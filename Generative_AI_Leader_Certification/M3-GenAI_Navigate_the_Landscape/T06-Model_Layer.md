

# 🧠 The Model Layer

## 🎯 1. What is an AI Model?

At the heart of every AI and machine learning system lies the **model**. Think of it as the brain of the operation.

An AI model is a mathematical structure trained on data to learn patterns, relationships, and underlying representations. Through training, it develops the ability to process new inputs and perform tasks such as:

- ✍️ Generating content, including text, images, and code.
- 📊 Analyzing data and identifying patterns.
- 🏷️ Classifying information into categories.
- 🔍 Recognizing objects and detecting features.
- 🔮 Making predictions based on learned patterns.

### ⚙️ How Does an AI Model Work?

A simplified model development process involves:

1. **Input data:** The model receives training data, such as images, text, numerical records, or audio.
2. **Training:** The model processes the data and learns patterns by adjusting its internal parameters.
3. **Learning:** The model develops mathematical representations of relationships within the data.
4. **Inference:** The trained model receives new, previously unseen inputs and generates predictions or outputs.

**Example:** An image classification model is trained using thousands of images labeled as cats and dogs. After training, it can analyze a new image and predict whether it contains a cat or a dog.

💡 **Key takeaway:** The model layer provides the core intelligence of an AI system. It processes inputs and generates outputs based on patterns learned during training.

## ☁️ 2. Agent Platform: A Model Hub

Within Google Cloud's Agent Platform, organizations have different options for using AI models:

- **Use existing models:** Select pre-trained models and customize them for specific requirements.
- **Build custom models:** Develop and train models using machine learning frameworks or automated tools.

For many use cases, organizations do not need to build a model from scratch. Existing models can already perform a wide range of tasks and may only require customization or integration into an application.

### 🏪 2.1 Model Garden

**Model Garden** is a service within Google Cloud's ML platform that allows users to discover, customize, and deploy existing models from Google and its partners.

According to the course material, Model Garden provides access to more than 160 models, including:

- Google's own models.
- Third-party models.
- Open-source models.

Organizations can use these models directly when supported or customize them using their own data.

**Key capabilities:**

- 🔍 Discover available models for different use cases.
- 🎨 Customize models to meet specific requirements.
- 🚀 Deploy models into custom applications.
- ⚡ Use some pre-trained models without additional tuning.

### 🧩 2.2 Types of Models Available in Model Garden

#### A. First-Party Foundation Models

These are models developed by Google, including general-purpose foundation models and task-specific models.

| Model / Service | Primary Purpose |
|---|---|
| **Gemini Pro, Flash, and other Gemini models** | Multimodal understanding, reasoning, and content generation. |
| **Imagen** | Text-to-image generation. |
| **Veo** | Text-to-video and image-to-video generation. |
| **Chirp 2.0** | Speech-to-text capabilities. |

Google also provides pre-trained APIs that help developers build AI applications without training models from scratch.

Examples include:

| Google AI Service | Primary Purpose |
|---|---|
| Speech-to-Text | Converts spoken audio into written text. |
| Natural Language AI | Analyzes and processes text. |
| Translation | Translates text between languages. |
| Vision AI | Analyzes images and identifies visual information. |

#### B. Open Models

Model Garden also provides access to open models that organizations can use, customize, and deploy depending on their licensing and technical requirements.

Examples from the course material include:

| Model | Developer / Organization | Primary Purpose |
|---|---|---|
| **Gemma 2** | Google | Open model family for generative AI tasks. |
| **CodeGemma** | Google | Code generation and code-related tasks. |
| **PaliGemma** | Google | Vision-language tasks involving images and text. |
| **Llama 3.1** | Meta | Large language model for general-purpose AI tasks. |
| **Llama 3.2** | Meta | Model family supporting language and, in selected variants, vision tasks. |
| **Mistral models** | Mistral AI | Language generation and other AI applications. |
| **Jamba 1.5** | AI21 Labs | Language model for text processing and generation. |
| **Falcon, FLAN-T5, ViT, EfficientNet** | Technology Innovation Institute (TII) and other research contributors | Language processing and computer vision tasks. |

#### C. Third-Party Models

Model Garden also supports foundation models developed by external AI companies and partners.

**Example: Anthropic Claude**

Claude is a family of AI models developed by Anthropic. It can be used for tasks such as:

- Understanding and generating text.
- Summarizing documents.
- Answering questions.
- Analyzing information.
- Assisting with coding.

💡 **Key takeaway:** Model Garden provides a central place to explore different AI models instead of requiring organizations to develop everything from scratch.

> ⚠️ **Note:** The model names, availability, specifications, and number of models in Model Garden may change over time. The examples above reflect the course material and should not be treated as a current catalog.

## 🏗️ 3. Build Models with Agent Platform

Organizations can also create and train their own models using Agent Platform.

The course presents two approaches:

### 3.1 Custom Model Training

Developers can build and train models using machine learning frameworks such as:

- **PyTorch:** An open-source framework for developing and training deep learning models.
- **TensorFlow:** A framework for building and deploying machine learning and deep learning models.
- **scikit-learn:** A Python library for traditional machine learning algorithms, including classification, regression, and clustering.
- **XGBoost:** A machine learning library that implements gradient-boosted decision trees.

**Advantages:**

- Greater control over model architecture and training.
- Flexibility in selecting algorithms and frameworks.
- Ability to customize models for specialized requirements.
- Support for complex and large-scale ML workloads.

**Example:** A data science team develops a regression model using scikit-learn to predict local government revenue based on historical financial data.

### 3.2 AutoML (Automated Machine Learning)

**AutoML** automates parts of the machine learning development process, allowing users to build and train models with less manual coding and technical effort.

Instead of manually selecting and configuring every model component, AutoML helps automate activities such as:

- Model selection.
- Training configuration.
- Hyperparameter tuning.
- Model evaluation.

The course identifies the following types of data and supported objectives:

| Data Type | Supported Objectives |
|---|---|
| 🖼️ Image Data | Classification and object detection. |
| 🎥 Video Data | Action recognition, classification, and object tracking. |
| 📊 Tabular Data | Classification, regression, and forecasting. |

**Examples:**

- **Image classification:** Determine whether an image shows a damaged or undamaged road.
- **Object detection:** Identify and locate vehicles, people, or other objects in an image.
- **Action recognition:** Identify activities or movements in a video.
- **Tabular classification:** Predict whether a household belongs to a particular category.
- **Regression:** Predict household expenditure based on socioeconomic characteristics.
- **Forecasting:** Estimate future service demand based on historical records.

### ⚖️ Custom Training vs. AutoML

| Aspect | Custom Model Training | AutoML |
|---|---|---|
| Technical knowledge | Requires more ML expertise. | Requires less specialized ML knowledge. |
| Coding | Usually involves programming. | Automates many development steps. |
| Model control | Greater control over algorithms and architecture. | More limited control over some model configurations. |
| Flexibility | Suitable for specialized requirements. | Suitable for supported tasks and data types. |
| Development effort | Generally requires more time and effort. | Can reduce development time and manual work. |
| Best suited for | Experienced data scientists and ML engineers. | Teams seeking to build models with less manual configuration. |

💡 **Key takeaway:** Custom training provides greater flexibility and control, while AutoML simplifies model development by automating parts of the process.

## 🔄 4. Standard Workflow for Creating Models in Agent Platform

The course presents five major steps for creating and managing machine learning models.

### 📥 Step 1: Gather Your Data

Determine the data required for training and testing based on the desired outcome.

Activities include:

- Define the problem the model needs to solve.
- Identify the required data sources.
- Collect relevant datasets.
- Determine the target variable or expected output.
- Separate data for training and testing.

**Example:** To predict household electricity consumption, gather historical electricity usage, household size, appliance information, and other relevant variables.

### 🧹 Step 2: Prepare Your Data

Ensure that the collected data is properly formatted, organized, and labeled.

Activities include:

- Remove duplicate records.
- Handle missing values.
- Correct inconsistent formats.
- Identify and address invalid values.
- Label data when required.
- Transform data into the format expected by the model.
- Check data quality and consistency.

**Example:** Before training a model using household records, standardize categorical values, handle missing income information, and verify that numerical fields contain valid values.

### 🏋️ Step 3: Train

Use the prepared data to build and train the model.

Activities include:

- Select an appropriate model or algorithm.
- Configure training parameters.
- Set hyperparameters.
- Run the training process.
- Evaluate the model using appropriate metrics.

**Example:** Train a regression model using historical household electricity consumption to predict future consumption.

### 📊 Step 4: Manage Your Model

Review model metrics to evaluate performance and monitor changes over time.

Activities include:

- Review evaluation metrics.
- Compare different model versions.
- Track model performance.
- Monitor data drift and performance degradation.
- Determine whether model updates or retraining are necessary.

**Example:** Monitor a household electricity consumption model to determine whether its prediction errors increase as consumption patterns change.

### 🚀 Step 5: Deploy and Predict

Make the trained model available for actual use.

Activities include:

- Deploy the trained model to an appropriate environment.
- Configure access and serving endpoints.
- Connect the model to applications or systems.
- Send new inputs to the deployed model.
- Generate predictions or outputs.

**Example:** Integrate the trained electricity consumption model into a dashboard where users can submit household information and receive estimated consumption.

### 🔁 Model Development Workflow Summary

| Step | Activity | Main Objective |
|---|---|---|
| 1. Gather Data | Collect relevant data. | Obtain the information needed to train and test the model. |
| 2. Prepare Data | Clean, format, and label data. | Ensure data is suitable for model training. |
| 3. Train | Configure and train the model. | Allow the model to learn patterns from the data. |
| 4. Manage | Evaluate and monitor the model. | Assess performance and identify issues. |
| 5. Deploy and Predict | Make the model available for use. | Generate predictions using new data. |

## 🏛️ 5. Example: Applying the Model Layer in a Government Agency

Imagine PSRTI wants to develop a machine learning model that predicts the demand for local government services.

The model layer provides the intelligence needed to analyze historical data and generate predictions.

| Requirement | Model Layer Capability |
|---|---|
| Use an existing language or predictive model | Model Garden |
| Develop a specialized prediction model | Custom model training |
| Build a model with less manual configuration | AutoML |
| Predict future service demand | Regression or forecasting model |
| Classify barangays based on service demand | Classification model |
| Identify objects in infrastructure images | Object detection model |
| Evaluate prediction accuracy | Model evaluation metrics |
| Generate predictions using new data | Model deployment and inference |

**Important distinction between the layers:**

- 🖥️ **Infrastructure:** Provides computing resources, storage, and networking.
- 🧠 **Model:** Provides the trained mathematical system that processes inputs and generates outputs.
- 🧩 **Platform:** Provides the tools and services to develop, train, deploy, and manage models.
- 🎯 **Agents:** Use models and tools to pursue goals and perform tasks.
- 📱 **Applications:** Provide the user-facing interface for interacting with AI capabilities.

## 💡 6. Key Takeaways

- The model layer is the core intelligence of an AI system.
- AI models are mathematical structures trained on data to learn patterns and relationships.
- Model Garden allows organizations to discover, customize, and deploy existing models.
- Model Garden includes first-party Google models, open models, and third-party models.
- Organizations can use pre-trained models or develop their own.
- Custom model training provides greater control and flexibility.
- AutoML simplifies model development by automating parts of the training process.
- The five major model development steps are gathering data, preparing data, training, managing, and deploying.
- A trained model can generate predictions or outputs when given new inputs. This process is called **inference**.

## 📝 7. Quick Review Questions

**1. What is an AI model?**

A mathematical structure trained on data to learn patterns and relationships and generate predictions or outputs.

**2. What is Model Garden?**

A service that allows users to discover, customize, and deploy existing AI models from Google and its partners.

**3. What are the three model categories available through Model Garden?**

- First-party Google models.
- Open models.
- Third-party models.

**4. What is the difference between custom model training and AutoML?**

Custom training provides greater control over model development, while AutoML automates parts of the process and requires less manual effort.

**5. Which framework is commonly used for traditional machine learning in Python?**

scikit-learn.

**6. Which framework is commonly used for deep learning?**

PyTorch and TensorFlow.

**7. What is the purpose of AutoML?**

To simplify model development by automating activities such as model selection, training configuration, and hyperparameter tuning.

**8. What are the five steps in the model development workflow?**

1. 📥 Gather your data.
2. 🧹 Prepare your data.
3. 🏋️ Train.
4. 📊 Manage your model.
5. 🚀 Deploy and predict.

**9. What is inference?**

The process of using a trained model to generate predictions or outputs from new input data.

**10. Does an organization always need to build an AI model from scratch?**

No. It can use existing pre-trained models from services such as Model Garden and customize them when necessary.

