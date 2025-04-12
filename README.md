# Project: Personalized Real Estate Agent – _HomeMatch_

🔗 [Udacity Generative AI Nanodegree](https://www.udacity.com/course/generative-ai--nd608)

Imagine you're a developer at **Future Homes Realty**, a forward-thinking real estate company. In an industry where personalization is essential for customer satisfaction, your task is to revolutionize how clients interact with property listings. The goal is to create a tailored experience for each buyer, making the property search process more engaging and aligned with individual preferences.

## 🧩 Components of "HomeMatch"

### 🧠 Understanding Buyer Preferences

- The real estate agent provides predefined questions and hardcoded answers from the buyer.
- Based on these inputs, the app identifies listings that match the buyer’s needs.

### 📦 Integrating with a Vector Database

- Embeddings of all property listings are stored in **LanceDB**.
- The buyer’s interview (preference input) is converted into a query embedding for semantic search.

### ✨ Personalized Listing Description Generation

- A **Language Model (LLM)** adjusts the property descriptions to match the buyer’s preferences.
- The model enhances the text without modifying any factual information.

### 🏡 Listing Presentation

- The personalized property descriptions are displayed as final output for the buyer.

## 🚀 How to Execute

1 - Clone the repositoy

```bash
git clone https://github.com/schadow98/udacity_personalized_real_estate_agent
cd udacity_personalized_real_estate_agent
```

2. **Open the Jupyter Notebook**

Open the [`notebook.ipynb`](./notebook.ipynb) file in your preferred Jupyter environment.

3. **(Optional) Set a proxy**

If you're behind a proxy, configure your environment accordingly to allow package downloads and external API access.

4. **Install the required dependencies**

Run the following command to install all necessary Python packages:

5. Create a .env file

Set up environment variables by creating a .env file based on the provided template: [.env-dist](./.env-dist) file

6. Run the notebook
   Execute all cells in [notebook](./notebook.ipynb) from top to bottom to initialize the application and test its full functionality.

## 🧪 Usage

1. **Initialize the application**

- Run all cells that define environment variables, import libraries, load models, and configure the vector database.
- This includes the setup of the embedding model, LanceDB connection, and all required utility functions.

2. **Enter buyer preferences**

- Scroll down to the **Usage** section in the notebook.
- Provide predefined questions and hardcoded answers to simulate buyer preferences.
- The application will:
  - Convert the input into an embedding
  - Perform a semantic search in the vector database
  - Retrieve the most relevant listings
  - Use an LLM to personalize each listing description based on the buyer's preferences

📌 The final personalized listings will be displayed directly in the notebook as output.
