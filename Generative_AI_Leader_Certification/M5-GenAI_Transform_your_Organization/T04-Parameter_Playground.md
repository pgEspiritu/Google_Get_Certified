
# 🎛️ Parameter Playground

## 📖 Introduction

This lesson provides a hands-on activity using **Google AI Studio** to understand how sampling parameters affect Gemini's generated responses.

- Experiment with different model settings.
- Observe how parameter changes influence the model's output.
- Develop an understanding of how to configure AI models to achieve desired results.

## 🧪 Hands-On Activity: Experimenting with Gemini

### 1. 🚀 Access Google AI Studio

1. Log in using your Google account.
2. Open [Google AI Studio](https://aistudio.google.com/).
3. Accept the terms and conditions if prompted.
4. Select **Playground**.

### 2. ✍️ Craft a Creative Prompt

**Scenario:** You are preparing an important presentation and need to convince an audience to invest in your team's new product or service.

Steps:

1. Locate the prompt input area and the **Run** button.
2. Enter a prompt describing a fictional product or service.
3. Include relevant details such as:
   - Product features.
   - Target audience.
   - Intended benefits.
   - Desired outcome.

**Sample prompt:**

```text
Write a pitch for a new app offering fast and affordable on-campus food delivery for university students.
```

4. Select **Run** to generate the initial pitch.

### 3. 🌡️ Experiment with Temperature

1. Open the **Run settings** panel.
2. Locate the **Temperature** setting.
3. Adjust the slider or enter a different value.
4. Reuse the same prompt and select **Run** again.
5. Compare the generated responses.

| Temperature | Expected Output |
|---|---|
| Lower | More formal, focused, and factual pitch |
| Higher | More creative, passionate, and enthusiastic pitch |

### 4. 🎯 Experiment with More Sampling Parameters

1. Open **Run settings**.
2. Select **Advanced settings**.
3. Experiment with the following parameters:

**A. Output Length**
- Change the maximum output length.
- Run the same prompt again.
- Observe how the response becomes shorter or more detailed.

**B. Top-p**
- Adjust the Top-p value.
- Run the same prompt again.
- Compare the generated responses.

| Top-p | Expected Output |
|---|---|
| Lower | More focused and concise pitch |
| Higher | Greater variety and potentially more elaborate pitch |

### 5. 🔍 Observe and Analyze

Pay attention to how each parameter affects the tone, style, and persuasiveness of the generated pitch.

**Guide Questions:**

- Does the pitch sound confident and authoritative?
- Is the response concise and direct or detailed and elaborate?
- Does it evoke the desired emotions in the audience?
- Does changing the temperature affect creativity and enthusiasm?
- Does changing Top-p affect the variety of the generated content?
- Does output length affect the completeness of the pitch?

## 🔑 Key Takeaways

- Google AI Studio Playground provides a practical environment for experimenting with Gemini models.
- Using the same prompt while changing one parameter at a time makes it easier to observe each parameter's effect.
- **Temperature** influences creativity and randomness.
- **Top-p** influences the range of probable tokens considered.
- **Output Length** controls the maximum size of the generated response.
- The best settings depend on the intended task and desired output.

💡 **Best Practice:** Change one parameter at a time while keeping the prompt consistent. This makes it easier to identify which setting caused a difference in the model's response.
