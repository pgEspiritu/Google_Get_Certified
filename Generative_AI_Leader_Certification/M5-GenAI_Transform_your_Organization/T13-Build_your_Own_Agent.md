
# 🛠️ Build Your Own Agent

## 1. Creating Agent Instructions

When building a Customer Experience (CX) agent using **CX Agent Studio**, you define how the agent should behave through system instructions.

### What to Include in Agent Instructions
- **Goal:** Define the agent's primary purpose.
  - Example: Customer support, answering questions, or generating content.
- **Behavior:** Specify how the agent should interact with users.
- **Rules and Constraints:** Establish what the agent should and should not do.
- **Tools and Knowledge:** Connect external tools, such as data stores, to provide additional information.

### Agent Development Workflow
1. Define the agent's goal.
2. Write its system instructions.
3. Specify its behavior and constraints.
4. Connect relevant tools and data stores.
5. Test the agent through conversations.
6. Refine the instructions based on the results.

## 2. 🏭 Practical Activity: Build a Cymbal Manufacturing Chatbot

### Business Scenario
**Cymbal Manufacturing** is a manufacturer of high-quality machinery, primarily producing storage containers.

The company wants an AI-powered website chatbot that can:
- Answer common customer inquiries.
- Provide product information.
- Offer basic troubleshooting assistance.
- Direct customers to the appropriate contact channel when necessary.

### Tools Used
- **Google AI Studio:** Used to build and experiment with the chatbot.
- **Gemini 2.5 Flash:** The model selected for the activity.
- **System Instructions:** Define the chatbot's persona, knowledge, behavior, and limitations.

> **Important:** CX Agent Studio is generally recommended for building production-oriented customer service agents. Google AI Studio is used in this activity because it is more accessible for experimentation and does not require setting up a Google Cloud project.

## 3. 🧠 What Are System Instructions?

System instructions provide the model with context, persona, goals, and constraints **before the user submits a prompt**.

They guide the agent's behavior throughout the conversation.

### Benefits of System Instructions

| Benefit | Description |
|---|---|
| **Consistency** | Maintains a consistent tone, personality, and communication style. |
| **Accuracy** | Grounds responses in specified knowledge and reduces the risk of hallucinations. |
| **Relevance** | Keeps responses focused on the intended business or subject area. |
| **Safety** | Establishes boundaries to prevent inappropriate or unhelpful responses. |

### Important Note
- System instructions help guide model behavior, but they do not guarantee that every response will be correct or safe.
- Production-ready enterprise agents require additional tools and techniques, including stronger security controls and adversarial defenses.
- Google Cloud's CX Agent Studio is recommended for more advanced enterprise conversational agents.

## 4. 🚀 Step-by-Step: Building the Chatbot in Google AI Studio

### STEP 1: Set Up Google AI Studio

1. Open [Google AI Studio](https://aistudio.google.com/).
2. On the Home screen, select **Chat with models**.
3. Open the **Run settings** menu on the right.
4. Click the current model name.
5. Select **Gemini 2.5 Flash**.

### STEP 2: Generate System Instructions

Instead of manually writing the chatbot's instructions, use generative AI to create them.

This approach uses an initial AI prompt to generate a more detailed system prompt.

#### Procedure
1. In the left panel, select **Enable saving** under Playground.
2. If prompted, select **Allow access** and complete the Google Drive authentication process.
3. Open **Run settings**.
4. Select **System instructions**.
5. In the Title field, enter:

   `Agent instruction writer`

6. Paste the following prompt into the System Instructions input box:

#### System Prompt: Agent Instruction Writer

```text
You are an expert at building virtual agent assistants.
For the provided company, role, and other information,
provide a system prompt that a developer can use.

You always fulfill the user's request to the best of
your ability.

Create a distinct goal and set of instructions for
this system prompt.
```

7. The instructions automatically save.
8. Close the System Instructions panel.

### STEP 3: Generate System Instructions for the Chatbot

Now use the instruction writer to generate a specific system prompt for the Cymbal Manufacturing chatbot.

#### Procedure
1. Enter the following prompt in the chat input box:

#### Prompt: Generate the Cymbal Manufacturing Chatbot Instructions

```text
Your task: Build a system prompt for a virtual agent
optimized for an LLM that would be appropriate to
assist an end user with the following job:

End user's company: Cymbal Manufacturing

Use case to be developed:
Cymbal Manufacturing builds storage containers
primarily. However, Cymbal is also capable of doing
custom machining based on request.

If the user needs custom machining done, they should
call the company directly.

You may answer any question which seems reasonable
within the scope of container manufacturing, but do
not take too many guesses.

Our containers are typically blue or green, but they
can occasionally be red.

Make sure to always keep a respectful tone and admit
when you don't know the answer to a user's question.

Cymbal's phone number is (333) 333-3333.
```

2. Select **Run**.
3. Review the generated system instructions.
4. Select **Copy to clipboard**.

**Output:** A generated system prompt containing the chatbot's goal, persona, knowledge, behavior, and limitations.

### STEP 4: Create the Cymbal Manufacturing Chatbot

1. At the top of Google AI Studio, select **New chat (+)**.
2. Open **Run settings**.
3. Select **System instructions**.
4. Open the dropdown and select **Create new instruction**.
5. Enter the instruction title:

   `Cymbal Manufacturing chatbot`

6. Paste the generated system instructions from Step 3.
7. Allow the instructions to save automatically.
8. Close the System Instructions panel.

**Result:** You now have a chatbot configured specifically for Cymbal Manufacturing.

### STEP 5: Test the Conversational Agent

Interact with the chatbot by entering different prompts and selecting **Run**.

#### Suggested Test Prompts

| Test | Example Prompt | Expected Behavior |
|---|---|---|
| Greeting | "Hello!" | Responds politely and introduces its assistance. |
| Product Information | "What colors are your storage containers available in?" | Explains that containers are typically blue or green, and occasionally red. |
| Custom Manufacturing | "Can you perform custom machining?" | Explains the service and directs the customer to call the company. |
| Out-of-Scope Question | "What's the weather today?" | Recognizes that the question is outside its knowledge scope rather than guessing. |

**Company Contact:** `(333) 333-3333`

### Testing Checklist

- [ ] Does the chatbot maintain a respectful tone?
- [ ] Does it provide relevant product information?
- [ ] Does it correctly describe available container colors?
- [ ] Does it direct custom machining requests to the company phone number?
- [ ] Does it admit when it does not know an answer?
- [ ] Does it avoid making unsupported assumptions?
- [ ] Does it stay within its intended business scope?

> **Note:** This activity demonstrates a basic conversational agent. It does not represent the full capabilities of a production-ready agent built using CX Agent Studio or other advanced conversational AI platforms.

## 5. ✨ Metaprompting

### What Is Metaprompting?
- **Metaprompting** is a prompting technique in which AI is instructed to create, modify, or interpret other prompts.
- Instead of directly writing the final prompt, you use an initial prompt to guide AI in generating a more detailed and structured prompt.

### How Metaprompting Was Used in This Activity

The Cymbal Manufacturing chatbot activity demonstrates two levels of prompting:

1. **First prompt:** Instructs AI to act as an expert virtual agent instruction writer.
2. **Second prompt:** Provides company information and requirements so AI can generate the chatbot's system instructions.
3. **Final system instructions:** The generated prompt is applied to the actual chatbot.

### Metaprompting Workflow

```text
Developer provides initial instructions
              |
              v
AI acts as a prompt engineer
              |
              v
Developer provides company details
and chatbot requirements
              |
              v
AI generates a detailed system prompt
              |
              v
Generated prompt becomes
the chatbot's system instructions
              |
              v
Chatbot is tested and refined
```

### Benefits of Metaprompting
- **Dynamic:** Allows prompts to be generated based on different requirements.
- **Flexible:** Makes it easier to adapt instructions to different business use cases.
- **Efficient:** Reduces the effort required to manually write complex system prompts.
- **Reusable:** The same prompt-generation approach can be applied to different companies and agents.
- **Adaptable:** Helps improve and modify prompts as requirements change.

## 6. 🔑 Key Takeaways

- **Agent instructions** define an agent's goal, persona, behavior, rules, and limitations.
- **System instructions** guide the model before and throughout user interactions.
- **Google AI Studio** provides an accessible environment for experimenting with conversational AI.
- **CX Agent Studio** is generally recommended for building more advanced customer experience agents.
- **Testing** is essential to verify whether the agent follows its instructions and handles different scenarios appropriately.
- **Metaprompting** uses AI to generate or improve other prompts.
- Agents can be enhanced by connecting external tools and data stores to access additional knowledge and perform tasks.

### 🧠 Quick Comparison: Prompting vs. Metaprompting

| Technique | Purpose | Example |
|---|---|---|
| **Prompting** | Instructs AI to perform a task. | "Answer customer questions about storage containers." |
| **Metaprompting** | Instructs AI to create or improve another prompt. | "Generate system instructions for a manufacturing customer service chatbot." |

**Remember:** System instructions define how an agent behaves, tools and data stores extend what it can do, and metaprompting helps create the instructions that guide the agent.
