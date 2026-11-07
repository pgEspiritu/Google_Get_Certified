

# 📱 AI on the Edge

## 🎯 1. What is Edge Computing?

**Edge computing** is an approach where data processing and AI computations happen on devices or servers located **closer to the data source or point of need**, rather than relying entirely on centralized cloud infrastructure.

Cloud computing is powerful, but it is not always the best option for every AI application.

For example, a self-driving car needs to make split-second decisions when detecting pedestrians, vehicles, or obstacles. Sending data to a remote cloud server and waiting for a response could introduce delays that affect safety.

This is where edge computing becomes useful.

### 🧩 Examples of Edge Computing

- 🚗 **Self-driving vehicles:** Process sensor data locally to detect obstacles and make immediate driving decisions.
- 🚁 **Drones:** Analyze camera and sensor information locally to navigate and avoid obstacles.
- 📱 **Smartphones:** Run AI features directly on the device without constantly sending information to the cloud.
- 🏭 **Industrial automation:** Process sensor readings locally to detect equipment abnormalities and trigger responses.
- 📹 **Smart surveillance cameras:** Analyze video feeds locally to identify objects or unusual activities.

💡 **Key definition:** Edge computing runs AI on devices or servers closer to the data source or point of need.

## ⚡ 2. Why Go Local or Edge?

Running AI models locally provides several advantages, particularly when applications require immediate responses or have limited internet connectivity.

### 🔒 2.1 Privacy

- Sensitive data can be processed directly on the device.
- Reduces the need to transmit raw personal or confidential information to remote servers.
- Provides greater control over how and where data is processed.

**Example:** A smartphone processes voice commands locally instead of continuously sending audio recordings to a cloud server.

*Note: Local processing can improve privacy, but it does not automatically guarantee data security. Devices still need appropriate access controls, encryption, and protection.*

### 🚀 2.2 Speed and Low Latency

- Processes data close to where it is generated.
- Reduces communication delays associated with sending information to remote cloud servers.
- Supports real-time applications that require immediate responses.

**Example:** A drone detects an obstacle and adjusts its flight path using locally processed sensor data without waiting for a cloud response.

### 🌐 2.3 Offline Access

- Allows supported AI functions to operate without an internet connection.
- Reduces dependence on continuous cloud connectivity.
- Enables applications to function in remote areas or locations with unstable internet access.

**Example:** A smartphone can perform certain text-processing or summarization tasks locally even when it has no internet connection.

### 📋 Benefits of Edge Computing

| Benefit | Explanation |
|---|---|
| 🔒 Privacy | Sensitive information can be processed locally. |
| 🚀 Speed | Reduces communication delays and supports real-time processing. |
| 🌐 Offline Access | Allows supported AI functions to work without continuous internet access. |
| 📡 Reduced Network Dependency | Lessens reliance on sending data to remote cloud infrastructure. |
| ⚙️ Local Control | Provides greater control over local processing and device operations. |

## 🛠️ 3. Google Tools for Edge AI

Running AI models on mobile devices and other edge hardware requires models and software optimized for limited computing resources.

Google provides tools that help developers deploy and run AI models locally.

### 3.1 Lite Runtime (LiteRT)

**Lite Runtime (LiteRT)** is Google's high-performance runtime for deploying machine learning models on edge devices, including mobile phones and embedded systems.

It helps models operate efficiently on devices with limited computing resources.

**Key purposes:**

- 📱 Run ML models directly on mobile devices.
- ⚡ Optimize model execution for on-device performance.
- 🖥️ Support deployment across different edge hardware.
- 🔄 Help developers convert and run compatible models locally.

**Example:** A developer builds an image classification application that identifies objects using a smartphone camera. LiteRT can help run the trained model directly on the phone.

💡 **Remember:** LiteRT helps machine learning models run efficiently on edge devices.

## 🤖 4. Gemini Nano

**Gemini Nano** is Google's compact and efficient AI model designed to run directly on supported devices, such as smartphones and other edge environments.

It belongs to Google's broader Gemini model family.

Unlike larger models that typically rely on cloud-based computing resources, Gemini Nano is designed for on-device AI processing.

Think of it as a smaller AI model that brings selected generative AI capabilities directly to a device.

### 4.1 Benefits of Gemini Nano

#### 🔒 Privacy

- Processes supported AI tasks directly on the device.
- Reduces the need to send certain information to remote servers.
- Helps keep sensitive information on the user's device.

#### 🚀 Speed

- Reduces the need for round-trip communication with cloud servers.
- Supports faster responses for supported on-device tasks.
- Useful for applications requiring low latency.

#### 🌐 Offline Access

- Supports certain AI capabilities without requiring an active internet connection.
- Allows supported features to work even when connectivity is unavailable.
- Reduces dependence on continuous cloud access.

### 4.2 Gemini Nano in Google Products

The course highlights examples of Gemini Nano integration into Google's products and services.

#### 📱 A. Pixel Phones

Gemini Nano powers selected on-device AI features, including:

- **Call Notes:** Helps summarize phone conversations.
- **Pixel Recorder:** Provides summaries of voice recordings.

These features demonstrate how generative AI can be integrated directly into smartphone experiences.

#### 📲 B. Android

Gemini Nano is available to Android developers through Google's **AI Edge SDK**, enabling developers to build AI-powered experiences into their applications.

Examples of potential applications include:

- Text summarization.
- Smart writing assistance.
- Text classification.
- Context-aware features.
- On-device content processing.

> ⚠️ **Note:** Feature availability depends on the supported device, model version, operating system, and application implementation. Not every Gemini Nano capability works on every Android device.

## ☁️ 5. Using Agent Platform to Build and Deploy Edge AI Models

Even when the final goal is to run an AI model on an edge device, cloud-based platforms can still play an important role in its development.

Google's ML platform, referred to as Agent Platform in the course, provides tools for building, training, evaluating, and refining models before deploying them to edge environments.

### 5.1 Model Development and Preparation

Agent Platform can support activities such as:

- 📊 **Data preparation:** Clean, organize, and transform training datasets.
- 🏋️ **Model training:** Train models using cloud computing resources.
- 🎨 **Model tuning:** Adjust model configurations and parameters.
- 📈 **Model evaluation:** Assess model performance using appropriate metrics.
- 🤝 **Collaboration:** Allow development teams to work together.
- ⚙️ **MLOps:** Manage model versions, workflows, and performance.

### 5.2 Deploying Models to Edge Devices

Once a model is ready, the deployment process involves several steps.

#### 🔄 A. Convert Models

Convert compatible models into **LiteRT** format or another supported format optimized for edge deployment.

The purpose is to make models suitable for execution on devices with limited computing resources.

#### 📦 B. Package and Deploy

- Package models and their required dependencies.
- Use containers where appropriate for supported edge deployment environments.
- Deploy models to compatible edge hardware.
- Configure the environment needed to run the model.

#### 📡 C. Manage and Monitor

- Manage deployed edge models.
- Track their performance.
- Gather information about model behavior.
- Identify potential issues.
- Use collected insights to improve or update models.

💡 **Key takeaway:** Cloud platforms can be used to develop and prepare AI models, while the final model execution can happen locally on edge devices.

## ⚖️ 6. Edge AI vs. Cloud AI

Edge AI and cloud AI differ mainly in where data processing and model inference take place.

| Aspect | ☁️ Cloud AI | 📱 Edge AI |
|---|---|---|
| Processing Location | Remote cloud servers or data centers. | Devices or servers close to the data source. |
| Internet Dependency | Usually requires network connectivity to access cloud services. | Can support offline operation for locally deployed models. |
| Latency | May experience network communication delays. | Often provides lower latency for local processing. |
| Computing Resources | Can access powerful cloud computing resources. | Limited by the device's available hardware. |
| Privacy | Data may need to be transmitted to cloud services. | Data can be processed locally, reducing transmission. |
| Scalability | Can scale using cloud infrastructure. | Depends on the number and capabilities of deployed devices. |
| Best Use Cases | Large-scale analysis, centralized processing, and resource-intensive workloads. | Real-time processing, offline operation, and local decision-making. |

### 🔀 6.1 Hybrid AI: Combining Edge and Cloud

Organizations do not always have to choose between edge and cloud computing. A **hybrid approach** combines both.

- Edge devices handle tasks requiring immediate responses.
- Cloud infrastructure handles resource-intensive processing, large-scale analysis, and centralized management.
- Selected information can be sent to the cloud for further analysis.

**Example: Industrial Monitoring System**

1. 🏭 Sensors collect temperature and vibration readings from industrial machines.
2. 📱 An edge device processes the readings and detects abnormal conditions.
3. 🚨 The system immediately triggers a local warning when an anomaly is detected.
4. ☁️ Selected sensor data is sent to the cloud for historical analysis.
5. 📊 A cloud-based model analyzes long-term trends and helps improve predictive maintenance.

This approach combines the low latency of edge processing with the computing power and scalability of cloud infrastructure.

## 🏛️ 7. Example: Applying Edge AI in Government

Imagine a local government unit wants to deploy an AI-powered monitoring system for flood-prone communities.

The system uses cameras and environmental sensors to monitor water levels and detect possible flooding.

| Requirement | Edge / Cloud Capability |
|---|---|
| 📹 Analyze camera feeds | On-device or edge-based computer vision model |
| 🌊 Detect sudden water-level changes | Local sensor processing and anomaly detection |
| 🚨 Trigger immediate warnings | Edge-based inference and local alerts |
| 📊 Analyze historical flood patterns | Cloud-based data processing and analytics |
| 🧠 Improve prediction models | Cloud-based model training and evaluation |
| 📡 Monitor deployed devices | Centralized cloud monitoring and management |

**Why use a hybrid approach?**

- Edge processing enables faster warnings even when internet connectivity is unstable.
- Cloud processing supports large-scale analysis of historical environmental data.
- Local processing can reduce the transmission of continuous video feeds.
- Centralized monitoring helps manage multiple deployed devices.

## 💡 8. Key Takeaways

- Edge computing processes data closer to its source rather than relying entirely on remote cloud infrastructure.
- Edge AI is useful for applications requiring low latency, privacy, and offline functionality.
- LiteRT helps developers run machine learning models efficiently on edge devices.
- Gemini Nano is a compact Gemini model designed for on-device AI applications.
- Gemini Nano supports selected AI features on compatible Pixel phones and Android devices.
- Agent Platform can support model development, training, evaluation, and preparation before edge deployment.
- Models can be converted, packaged, deployed, and monitored for edge environments.
- Hybrid AI combines edge processing with cloud-based computing and analytics.

## 📝 9. Quick Review Questions

**1. What is edge computing?**

Processing data on devices or servers closer to the data source or point of need.

**2. Why is edge computing useful for self-driving cars and drones?**

It enables faster, low-latency processing so devices can respond immediately to their surroundings.

**3. What are three major benefits of edge AI?**

- 🔒 Privacy.
- 🚀 Speed and low latency.
- 🌐 Offline access.

**4. What is LiteRT?**

Google's high-performance runtime for running machine learning models on edge devices.

**5. What is Gemini Nano?**

A compact and efficient Gemini model designed to run directly on supported devices.

**6. What is the difference between Gemini Nano and cloud-based Gemini models?**

Gemini Nano is designed for on-device execution, while cloud-based Gemini models use remote computing infrastructure.

**7. Why use Agent Platform when deploying AI models to edge devices?**

It provides tools for model development, training, tuning, evaluation, and management before deployment.

**8. What are the three major steps in preparing models for edge deployment?**

1. 🔄 Convert models.
2. 📦 Package and deploy.
3. 📡 Manage and monitor.

**9. What is hybrid AI?**

An approach that combines edge processing for local, latency-sensitive tasks with cloud computing for resource-intensive processing and large-scale analysis.

**10. When is edge AI more appropriate than cloud AI?**

When an application requires immediate responses, local data processing, reduced network dependency, or offline functionality.

