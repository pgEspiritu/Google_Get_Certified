# 🛒 Use Case: Gemini in Action – Morrisons Product Finder

## 🏢 Overview

- **Morrisons** is one of the UK's largest supermarket chains.
  - Operates supermarkets and approximately 1,600 convenience stores.
  - Works with around 2,700 farmers and growers who supply its products.
- Morrisons partnered with **Google Cloud** to improve the in-store shopping experience using:
  - **BigQuery** – stores and manages product location data.
  - **Vertex AI (now Agent Platform)** – supports the development and deployment of AI-powered applications.
  - **Gemini** – interprets customer search queries and helps identify the requested products.

## 🔎 Product Finder: AI-Powered In-Store Search

- **Product Finder** is an AI-powered feature integrated into the Morrisons mobile app.
  - Helps customers quickly locate products inside physical stores.
  - Provides information about:
    - The product's aisle.
    - Its precise store location.
  - Allows customers to search using ordinary product names or descriptions.
  - Helps customers find products even when store shelves or product arrangements change.

- **Example:**
  - A customer searches for *tahini* using the app.
  - Gemini interprets the search query.
  - The system identifies the corresponding product and location IDs.
  - Product Finder displays where the item can be found in the store.

- **Customer impact:**
  - Makes in-store shopping faster and more convenient.
  - Reduces the difficulty of locating unfamiliar or hard-to-find products.
  - Provides a search experience similar to online shopping.
  - Recorded approximately **50,000 searches per day during Easter 2025**, with usage continuing to grow as customers returned to the feature.

## ⚙️ How the Technology Works

The solution combines Gemini, Vertex AI, and BigQuery to translate customer searches into useful product-location information.

1. **Customer submits a search query**
   - The customer enters a product name or description in the Morrisons app.
   - Example: "Tahini," "cranberry sauce," or "gravy."

2. **Gemini interprets the query**
   - Understands the customer's natural-language input.
   - Helps translate the search into the required product information.

3. **Vertex AI supports the AI application**
   - Provides the platform and capabilities used to integrate the AI model into the application.
   - Connects the AI-powered search process with the product information system.

4. **BigQuery provides product location data**
   - Contains information about where products are located in individual stores.
   - Helps the system identify the corresponding product ID and location ID.

5. **Product Finder displays the result**
   - Returns the product's aisle and location.
   - Helps customers find the item more easily.

## 🧩 Key Technologies and Their Roles

| Technology | Role in the Product Finder |
|---|---|
| 🧠 Gemini | Interprets customer search queries and translates natural-language input into the information needed by the system. |
| ⚙️ Vertex AI / Agent Platform | Supports the development and integration of the AI-powered application. |
| 🗄️ BigQuery | Stores and provides product and store-location data. |
| 📱 Morrisons App | Provides the customer-facing interface for searching and locating products. |

## 💡 Business Benefits and Impact

- **⏱️ Faster development**
  - Integrating Google's AI tools and cloud services reduced the amount of development work required.
  - A relatively small team could build the solution without spending months developing every capability from scratch.

- **💰 Reduced time and resources**
  - Pre-trained models reduced the need to build and train a model from the beginning.
  - Developers could focus more on application integration and customer experience.

- **😊 Improved customer experience**
  - Customers can quickly find products without having to ask store employees.
  - Particularly useful for unfamiliar products or items that are difficult to locate.

- **📈 Increased customer engagement**
  - Product Finder recorded approximately 50,000 daily searches during Easter 2025.
  - Continued usage indicates that customers find the feature useful.

- **🤝 Improved development collaboration**
  - The integration of Google Cloud services helped the team develop and bring proof-of-concept solutions into practical use more quickly.

## 🧪 Important Lesson: Using Pre-Trained Foundation Models

- One major advantage of using a **pre-trained model** is that organizations do not need to develop and train the entire model themselves.
- Instead, they can focus on testing how the model performs within their specific application and business environment.
- However, organizations must still:
  - Test the model's outputs and behavior.
  - Check its accuracy and reliability for the intended use case.
  - Validate its integration with existing systems and business data.
  - Monitor its performance in actual operating conditions.

> 💡 **Key Insight:** Pre-trained AI models allow organizations to focus more on solving business problems and improving user experiences rather than building every AI capability from scratch.

## 🖼️ Additional Application: Gemini for Product Imagery

- Gemini can also support businesses in generating customized product images at scale.
  - Helps create high-quality product imagery.
  - Supports customized and localized visual content.
  - Can reduce the time and resources required to produce product images.

- **Potential business applications:**
  - Creating product images for online catalogs.
  - Producing localized marketing materials.
  - Generating customized promotional visuals.
  - Supporting digital merchandising.

## 🎯 Key Takeaways

- Gemini can help businesses understand and process natural-language customer requests.
- Combining AI models with enterprise data makes AI applications more useful in real-world environments.
- BigQuery provides the product-location information, while Gemini interprets customer queries.
- Vertex AI supports the integration and deployment of AI-powered solutions.
- Pre-trained models can reduce development time and allow smaller teams to build practical AI applications.
- AI adoption can generate measurable business value through improved customer experience, operational efficiency, and customer engagement.

## 📝 Quick Review

**1. What is Morrisons Product Finder?**

- An AI-powered feature in the Morrisons mobile app that helps customers locate products inside physical stores.

**2. What is the role of Gemini?**

- It interprets customer search queries and helps translate them into the product information required by the system.

**3. What is the role of BigQuery?**

- It stores product and store-location data used to identify where items can be found.

**4. Why did Morrisons use pre-trained AI models?**

- To reduce development effort and allow its team to focus on integrating the technology and improving the customer experience.

**5. What is the main business value of the solution?**

- Faster and more convenient shopping, improved customer engagement, and more efficient application development.
