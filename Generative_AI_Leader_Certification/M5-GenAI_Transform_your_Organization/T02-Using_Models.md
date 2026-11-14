
# 🧠 Using Models

## 📖 Introduction

- Generative AI agents are powered by **generative AI models**, which serve as the brains of the operation.
- Even after models are trained and ready, their outputs can still be improved through adjustments to parameters and settings.
- This lesson focuses on how to effectively use generative AI models within agents.

## 🎛️ Sampling Parameters and Settings

Sampling parameters are adjustable settings that influence how an AI model generates responses.

Think of them as **knobs and dials** that help customize the model's output based on the task or desired result.

### 1. 🔢 Token Count

- Tokens are the basic building blocks of text processed by an AI model.
- A token can represent:
  - A complete word.
  - Part of a word.
  - A space or punctuation mark.
- Models have limits on the number of tokens they can process.
- A higher token count can support longer conversations but requires more processing power.

**Rule of thumb:**
- 1 token ≈ 4 English characters.
- 100 tokens ≈ 60–80 words.

### 2. 🌡️ Temperature

- Controls the **creativity and randomness** of the model's word choices.
- Influences the diversity and unpredictability of generated responses.

| Temperature | Effect |
|---|---|
| Low | More focused, predictable, and repeatable responses |
| High | More creative, diverse, and unpredictable responses |

**Use cases:**
- Low temperature: Factual answers, structured responses, and summaries.
- High temperature: Brainstorming, creative writing, and open-ended tasks.

### 3. 🎯 Top-p (Nucleus Sampling)

- Controls the cumulative probability of the most likely tokens considered during text generation.
- Influences how focused or diverse the model's responses can be.

| Top-p | Effect |
|---|---|
| Low | Considers a narrower range of the most probable tokens |
| High | Allows a broader range of possible tokens, increasing diversity |

- Lower top-p generally produces more focused and predictable responses.
- Higher top-p allows more varied and diverse responses.

### 4. 🛡️ Safety Settings

- Control the filtering of potentially harmful or inappropriate content.
- Filtering levels can be adjusted based on the application's requirements and preferences.

### 5. 📏 Output Length

- Determines the maximum length of the generated response.
- Can be controlled through a specified number of words, characters, or tokens, depending on the model or platform.
- The model may also generate content until it reaches a natural stopping point.

## ⚙️ Practical Parameter Adjustments

Different tasks require different model settings.

| Desired Output | Suggested Settings |
|---|---|
| Concise and factual answer | Lower temperature, shorter output length |
| Creative and open-ended response | Higher temperature and top-p |
| Focused and predictable response | Lower temperature and top-p |
| Longer conversation or detailed response | Higher token allowance and output length |

💡 **Tip:** Experiment with sampling parameters to find the settings that best match the task. Temperature and top-p both influence randomness, but they control it in different ways.

## 🔌 How to Access Sampling Parameters and Settings

The process depends on:
- Where the AI model comes from.
- Which platform or application is used to access it.
- How the model is integrated into the agent.

### Accessing Models Through APIs

- **API** stands for Application Programming Interface.
- It allows different software systems to communicate and exchange information.
- An API acts as a messenger between applications.

**Example:**
- A weather application sends a request to a weather service through an API.
- The service returns weather information to the application.

**In Generative AI:**
1. An application sends a prompt to an AI model through an API.
2. The API passes the prompt and any configured parameters to the model.
3. The model generates a response.
4. The API returns the response to the application.

- APIs often allow developers to customize model behavior by supplying sampling parameters and settings alongside the prompt.

## 🔑 Key Takeaways

- Generative AI models power the intelligence of AI agents.
- Sampling parameters help control how models generate responses.
- The five important settings discussed are:
  1. 🔢 Token Count – Controls the amount of text the model can process.
  2. 🌡️ Temperature – Controls randomness and creativity.
  3. 🎯 Top-p – Controls the range of probable tokens considered.
  4. 🛡️ Safety Settings – Filter potentially harmful or inappropriate content.
  5. 📏 Output Length – Limits the size of generated responses.
- APIs allow applications to communicate with AI models and pass customization settings.
