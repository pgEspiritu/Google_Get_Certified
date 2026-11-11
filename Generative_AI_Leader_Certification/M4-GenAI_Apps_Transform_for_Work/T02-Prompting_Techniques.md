
# 🎯 Prompting Techniques

## 1. 📌 Introduction

- **Prompting** is the process of providing instructions or inputs to a generative AI (Gen AI) model to guide its responses and outputs.
- Developing effective prompting skills is essential for getting accurate, relevant, and useful results from generative AI applications.
- **Importance of prompting:**
  - 🎯 Improve the quality and relevance of AI-generated outputs.
  - ⚙️ Tailor AI responses to specific tasks and requirements.
  - 💡 Guide the model toward the desired results.
  - 🚀 Maximize the capabilities of generative AI tools.
- **Key principle:** Effective prompting requires practice and experimentation with different techniques.

## 2. 🧠 Using Examples in Your Prompts

One way to improve prompting is to provide examples that demonstrate how the AI should perform a task.

### 2.1. Zero-Shot Prompting

- **Definition:** Asking a foundation model to perform a task without providing any prior examples.
- The model relies on its existing knowledge and understanding of the instructions.
- **Characteristics:**
  - No examples are provided.
  - Relies entirely on the prompt and the model's existing knowledge.
  - Useful for straightforward tasks.
- **Example:**
  - An online clothing store customer asks about its return policy.
  - The AI generates a response based on its general knowledge, even without being given examples of how to respond.
- **Key idea:** Give an instruction without demonstrating an example.

### 2.2. One-Shot Prompting

- **Definition:** Providing the foundation model with one example to demonstrate how a task should be performed.
- The model uses the example as a guide when handling similar tasks.
- **Characteristics:**
  - Provides exactly one example.
  - Demonstrates the expected format, pattern, or response.
  - Helps the model understand the desired output.
- **Example:**
  - An online clothing store provides one example of a customer inquiry about shipping times and its corresponding category.
  - The AI uses this example to classify similar customer inquiries.
- **Key idea:** Give one example to guide the model's response.

### 2.3. Few-Shot Prompting

- **Definition:** Providing the foundation model with multiple examples to help it understand and perform a task.
- The examples demonstrate different situations and expected outputs.
- **Characteristics:**
  - Provides multiple examples.
  - Helps establish patterns and expected responses.
  - Improves consistency in handling similar situations.
  - Useful for tasks requiring specific formats, classifications, or response styles.
- **Example:**
  - An online clothing store provides several examples of customer inquiries and appropriate responses.
  - The AI learns from the demonstrated patterns and applies them to similar inquiries.
  - Possible outputs include:
    - Providing a discount code when a customer reports a delayed delivery.
    - Giving detailed instructions when a customer wants to return a damaged item.
- **Key idea:** Give multiple examples to demonstrate different scenarios and expected outputs.

## 3. 📊 Comparison of Prompting Techniques

| Prompting Technique | Number of Examples | Description |
|---|---:|---|
| Zero-Shot | 0 | Performs a task using instructions alone. |
| One-Shot | 1 | Uses one example as a guide. |
| Few-Shot | 2 or more | Uses multiple examples to establish patterns and expected outputs. |

## 4. 🛍️ Practical Application: Online Clothing Store

Consider an online clothing store that uses generative AI to improve customer service.

- **Zero-Shot Prompting:**
  - The AI receives a customer question about the return policy without any sample responses.
  - It generates an answer based on its existing knowledge and the provided instructions.
- **One-Shot Prompting:**
  - The AI receives one sample customer inquiry about shipping times, together with its corresponding classification.
  - It uses the example to classify similar customer inquiries.
- **Few-Shot Prompting:**
  - The AI receives multiple customer inquiries and their corresponding responses.
  - It uses the examples to handle different customer situations, such as delayed deliveries and damaged products.

## 5. 🎯 Key Takeaways

- Prompting is an essential skill for effectively using generative AI.
- Providing examples helps guide AI models toward the desired output.
- The three prompting techniques differ primarily in the number of examples provided:
  - **Zero-Shot:** No examples.
  - **One-Shot:** One example.
  - **Few-Shot:** Multiple examples.
- Choose the prompting technique based on the complexity of the task and the level of guidance required.
- 💡 **Remember:** The more clearly you communicate your instructions and demonstrate the expected output, the easier it is to guide generative AI toward useful and consistent results.
