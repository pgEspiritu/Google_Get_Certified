# 🧠 Types of Machine Learning

## 1. Machine Learning Approaches and Data Requirements

Machine learning (ML) uses different learning approaches depending on the type of data available and how the model is expected to learn.

There are three primary machine learning approaches:

1. **Supervised Learning** – Learns from labeled data.
2. **Unsupervised Learning** – Discovers patterns in unlabeled data.
3. **Reinforcement Learning** – Learns through interaction, feedback, and rewards.

Each approach has different data requirements and is suited to different problems.

| Learning Approach | Data Requirement | How It Learns | Main Purpose |
|---|---|---|---|
| Supervised Learning | Labeled data | Learns from examples with known answers | Predict outcomes or classify data |
| Unsupervised Learning | Unlabeled data | Identifies patterns and relationships | Discover groups, structures, and anomalies |
| Reinforcement Learning | Interaction and feedback | Learns through trial and error using rewards or penalties | Find actions that maximize rewards |

## 2. Labeled vs. Unlabeled Data

Before understanding the three learning approaches, it is important to distinguish between labeled and unlabeled data.

### 🏷️ Labeled Data

**Labeled data** contains tags or annotations that identify the meaning, category, or correct answer associated with each data item.

Labels may be assigned manually by people or generated through automated systems.

**Examples:**
- An image dataset where each picture is labeled as `cat` or `dog`.
- Customer reviews labeled as `positive`, `negative`, or `neutral`.
- A dataset of houses where each record includes the actual selling price.
- A collection of emails labeled as `spam` or `not spam`.

Labels provide the model with known answers that it can use to learn relationships between inputs and expected outputs.

### 📂 Unlabeled Data

**Unlabeled data** is information that does not have predefined tags or categories identifying the correct answer.

The data is available, but the model must discover patterns, similarities, or structures without being given explicit labels.

**Examples:**
- A collection of photos without object names or categories.
- Audio recordings without transcripts or classifications.
- Website traffic logs without predefined user segments.
- Customer purchase records without assigned customer groups.

Unlabeled data is useful for discovering patterns that may not have been identified beforehand.

### Quick Comparison

| Aspect | Labeled Data | Unlabeled Data |
|---|---|---|
| Tags or annotations | Available | Not provided |
| Known answers | Available during training | Not provided |
| Learning approach commonly associated with it | Supervised learning | Unsupervised learning |
| Example | Customer reviews labeled positive or negative | Customer reviews without sentiment labels |

**Important:** Labeled data is not necessarily better than unlabeled data. The appropriate data depends on the problem and the learning approach being used.

## 3. Supervised Machine Learning

**Supervised learning** trains a model using labeled data. Each input is paired with its corresponding correct output, allowing the model to learn the relationship between them.

The model identifies patterns in the training data and uses what it has learned to predict outputs for new, unseen inputs.

### How It Works

1. **Collect labeled data** – Gather examples with known answers.
2. **Train the model** – Let the algorithm learn relationships between input features and their corresponding outputs.
3. **Evaluate the model** – Test its predictions using data it has not seen during training.
4. **Make predictions** – Use the trained model to predict outcomes for new data.

### Example: Predicting House Prices

Suppose a real estate company wants to predict the selling price of houses.

The training dataset contains:

| House Size (sqm) | Bedrooms | Location | Actual Selling Price |
|---:|---:|---|---:|
| 80 | 2 | Quezon City | ₱3,500,000 |
| 100 | 3 | Quezon City | ₱4,500,000 |
| 120 | 3 | Makati | ₱7,000,000 |
| 150 | 4 | Pasig | ₱8,000,000 |

The model learns how house characteristics relate to their actual selling prices.

After training, it can estimate the selling price of another house using its size, number of bedrooms, and location.

### Common Supervised Learning Tasks

- **Classification** – Predicts a category or class.
  - Example: Classifying an email as spam or not spam.
  - Example: Identifying whether a customer review is positive, negative, or neutral.
- **Regression** – Predicts a numerical value.
  - Example: Predicting house prices.
  - Example: Forecasting monthly electricity consumption.

**Key idea:** Supervised learning learns from examples where the correct answers are already known.

## 4. Unsupervised Machine Learning

**Unsupervised learning** uses unlabeled data to identify patterns, relationships, similarities, or natural groupings.

Unlike supervised learning, the model is not given predefined answers. Instead, it explores the data to discover its underlying structure.

It is particularly useful for exploratory data analysis because it can reveal patterns that may not be immediately obvious.

### How It Works

1. **Collect unlabeled data** – Gather records without predefined categories or target values.
2. **Analyze patterns** – The algorithm examines similarities, differences, and relationships.
3. **Identify structures** – The model discovers natural groupings or unusual observations.
4. **Interpret the results** – People examine the findings and determine their practical meaning.

### Example: Customer Segmentation

Suppose a company wants to understand its customers' purchasing behavior.

It has transaction records containing:
- Customer purchase history
- Frequency of purchases
- Total amount spent
- Product preferences

The dataset does not contain predefined customer categories.

An unsupervised learning algorithm can identify groups of customers with similar purchasing patterns.

For example, it might discover:

- **Group A:** Customers who frequently purchase low-cost products.
- **Group B:** Customers who make occasional but high-value purchases.
- **Group C:** Customers who regularly purchase products from a particular category.

The company can use these findings to improve marketing strategies and product recommendations.

### Common Unsupervised Learning Tasks

- **Clustering** – Groups similar data points together.
  - Example: Grouping customers based on purchasing behavior.
- **Anomaly Detection** – Identifies observations that differ significantly from normal patterns.
  - Example: Flagging unusual financial transactions.
- **Dimensionality Reduction** – Reduces the number of variables while retaining important information.
  - Example: Simplifying a dataset with many features for analysis or visualization.

**Key idea:** Unsupervised learning discovers patterns without being given predefined answers or categories.

## 5. Reinforcement Learning

**Reinforcement learning (RL)** is a machine learning approach in which an agent learns by interacting with an environment and receiving feedback based on its actions.

Instead of learning from labeled examples, the agent uses trial and error to determine which actions produce the best results.

It aims to maximize cumulative rewards over time while avoiding actions that lead to penalties or undesirable outcomes.

### How It Works

The main components of reinforcement learning are:

- **Agent** – The learner or decision-maker.
- **Environment** – The surroundings or system with which the agent interacts.
- **Action** – A decision or movement made by the agent.
- **Reward** – Feedback indicating whether an action was beneficial.
- **State** – The current situation or condition of the environment.

### Example: Robot Navigating a Maze

Imagine a robot learning how to navigate a maze.

1. The robot starts without knowing the maze's layout.
2. It takes an action, such as moving forward or turning left.
3. The environment provides feedback.
4. It receives a positive reward when it moves closer to the goal or finds the exit.
5. It receives a penalty when it hits a wall or makes an unsuccessful move.
6. Over repeated interactions, it learns which actions lead to better outcomes.

This process allows the robot to improve its decisions over time.

### Common Applications

- **Robotics** – Training robots to perform tasks in manufacturing environments.
- **Autonomous vehicles** – Developing decision-making strategies for navigating complex traffic situations.
- **Gaming** – Training an agent to select actions that maximize its chances of winning.
- **Recommendation systems** – Adapting recommendations based on user interactions and feedback.

**Key idea:** Reinforcement learning learns through interaction, using rewards and penalties to improve decision-making.

## 6. Comparing the Three Machine Learning Approaches

| Feature | Supervised Learning | Unsupervised Learning | Reinforcement Learning |
|---|---|---|---|
| Learning method | Learns from labeled examples | Discovers patterns in unlabeled data | Learns through interaction and feedback |
| Data requirement | Inputs with known outputs | Data without predefined labels | Environment, states, actions, and rewards |
| Feedback | Correct answers during training | No predefined correct answers | Rewards or penalties from actions |
| Main objective | Predict or classify | Discover patterns or groupings | Maximize cumulative rewards |
| Example | House price prediction | Customer segmentation | Robot navigation |

### Easy Way to Remember

- 🏷️ **Supervised:** Learn with an answer key.
- 🔍 **Unsupervised:** Find patterns without an answer key.
- 🎮 **Reinforcement:** Learn through trial and error with rewards and penalties.

## 7. Examples of Machine Learning Approaches on Google Cloud

Google Cloud provides tools and services that support different machine learning use cases. The appropriate service depends on the problem, data, and model requirements.

> **Note:** The course uses the term Agent Platform. Google Cloud product names and capabilities may evolve, so verify the current service documentation when implementing these examples.

### A. Predictive Maintenance with Agent Platform (Supervised Learning)

**Objective:** Predict when industrial equipment is likely to fail so that maintenance can be performed before a breakdown occurs.

**How it works:**

1. Collect sensor data from machines, such as:
   - Temperature
   - Pressure
   - Vibration
2. Use historical sensor readings paired with known equipment outcomes, such as normal operation or recorded failures.
3. Train a supervised learning model to recognize patterns associated with equipment failure.
4. Use the trained model to estimate the likelihood of future failures.
5. Schedule maintenance based on the model's predictions.

**Benefits:**
- Reduces unexpected equipment downtime.
- Supports preventive maintenance.
- Helps optimize maintenance schedules.
- Can reduce operational costs.

**Why supervised learning?**

The model learns from historical examples where equipment conditions are paired with known outcomes, such as whether a machine failed.

### B. Anomaly Detection with BigQuery ML (Unsupervised Learning)

**Objective:** Identify unusual transactions that may indicate fraudulent or suspicious activity.

**How it works:**

1. Collect historical transaction data, including:
   - Transaction amount
   - Transaction location
   - Transaction time
   - Transaction frequency
2. Analyze normal transaction patterns using an unsupervised learning approach.
3. Identify transactions that significantly deviate from those patterns.
4. Flag unusual transactions for further investigation.

**Benefits:**
- Helps identify suspicious activities.
- Supports fraud monitoring.
- Reduces the need to manually examine every transaction.
- Helps organizations detect unusual patterns.

**Why unsupervised learning?**

The model can identify unusual transactions without requiring every transaction to be labeled as fraudulent or legitimate in advance.

### C. Product Recommendations with Agent Platform (Reinforcement Learning)

**Objective:** Improve product recommendations by learning from user interactions and feedback.

**How it works:**

1. Collect information about user interactions, such as:
   - Browsing history
   - Previous purchases
   - Product clicks
   - Recommendation responses
2. Present product recommendations to users.
3. Observe how users respond to the recommendations.
4. Use feedback, such as clicks or purchases, as signals for evaluating recommendation strategies.
5. Adjust future recommendations to improve the desired outcome, such as engagement or sales.

**Benefits:**
- Improves personalization.
- Adapts recommendations based on user behavior.
- Can increase customer engagement.
- Helps optimize recommendation strategies over time.

**Why reinforcement learning?**

The recommendation strategy can learn from user interactions and feedback, adjusting its actions to maximize a defined reward.

**Important distinction:** Not every recommendation system uses reinforcement learning. Many use supervised learning, collaborative filtering, or other approaches. Reinforcement learning is particularly relevant when recommendations are continuously adjusted based on feedback and longer-term outcomes.

## 8. Applying the Three Approaches in Government and Statistical Work

These learning approaches can also support government operations, research, and statistical analysis.

| Government Use Case | Possible ML Approach | Example |
|---|---|---|
| Predicting service demand | Supervised learning | Predicting the number of citizens expected to request a particular service |
| Identifying barangay profiles | Unsupervised learning | Grouping barangays with similar socioeconomic characteristics |
| Detecting unusual transactions | Unsupervised learning | Identifying irregularities in financial or procurement records |
| Classifying citizen feedback | Supervised learning | Categorizing feedback as positive, negative, or neutral using labeled examples |
| Optimizing resource allocation | Reinforcement learning | Evaluating allocation strategies based on defined outcomes and feedback |

**Practical consideration:** Government applications require appropriate data governance, privacy protection, data quality controls, and human oversight. Model predictions should support—not automatically replace—professional judgment and official decision-making.

## 9. Key Takeaways

1. Machine learning has three primary learning approaches: supervised, unsupervised, and reinforcement learning.
2. Supervised learning requires labeled data, where inputs are paired with known outputs.
3. Unsupervised learning uses unlabeled data to discover patterns, groups, and unusual observations.
4. Reinforcement learning learns through interaction with an environment and feedback in the form of rewards or penalties.
5. The choice of learning approach depends on the problem, available data, and desired outcome.
6. Google Cloud services can support different machine learning applications, including predictive maintenance, anomaly detection, and personalized recommendations.

## 10. Quick Review Questions

**1. Which machine learning approach uses labeled data to predict outcomes?**

Answer: Supervised learning.

**2. What is the main difference between labeled and unlabeled data?**

Answer: Labeled data has predefined tags or known answers, while unlabeled data does not.

**3. A company wants to group customers based on their purchasing behavior without predefined customer categories. Which approach should it use?**

Answer: Unsupervised learning.

**4. What machine learning approach allows a robot to learn by receiving rewards and penalties?**

Answer: Reinforcement learning.

**5. A model is trained using historical machine sensor readings paired with known equipment failures. Which approach is appropriate?**

Answer: Supervised learning.

**6. A financial institution wants to identify unusual transactions by analyzing normal transaction patterns. Which approach is appropriate?**

Answer: Unsupervised learning.

**7. What are the main components of reinforcement learning?**

Answer: Agent, environment, state, action, and reward.

**8. Can all recommendation systems be considered reinforcement learning systems?**

Answer: No. Recommendation systems can use several approaches, including supervised learning and collaborative filtering. Reinforcement learning is one option when the system learns and adjusts recommendations through ongoing interaction and feedback.
