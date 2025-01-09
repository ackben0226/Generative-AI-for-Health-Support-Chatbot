# __🩺 Health Support Chatbot - README 📖__

## __🌟 Overview__
</br> This project is a Health Support Chatbot designed to assist users with health-related queries using customer data and advanced AI models. The chatbot provides tailored responses by leveraging structured data and OpenAI-powered language capabilities.

## __✨ Features__
- 💬 ___Interactive Chat Interface:___ User-friendly chatbot powered by Streamlit.
- 🔍 ___Customer Insights Retrieval:___ Fetches and utilizes detailed customer information (e.g., demographics, health goals, satisfaction scores).
- 🤖 ___AI-Powered Responses:___ Context-aware answers generated using OpenAI's language models.
- ⚡ ___Fast Data Search:___ Implements FAISS for quick similarity-based retrieval.
- 📚 ___Dynamic Summaries:___ Combines data insights with user queries for meaningful, personalized answers.
  
## __🚀 Installation and Setup__
### __✅ Prerequisites__
1. 🐍 Python 3.7 or higher
2. 🖥️ Streamlit installed
3. 🔑 OpenAI API Key
4. 📦 Required Python libraries
   
## __🛠️ Dependencies__
Install the required libraries using pip:

bash

Copy code
pip install streamlit langchain openai python-dotenv faiss pandas

## __🔐 Environment Variables__
Set up a .env file with your OpenAI API key:

plaintext
Copy code
OPENAI_API_KEY=your_openai_api_key_here

## __🏃 Usage__
Step 1️⃣: Prepare the Customer Data
Ensure the CSV file (Cleaning_GenerativeAI_Health_Customer_Insights.csv) is available and formatted correctly.

🔑 Required Columns:
CustomerID, Age, Gender, Region, HealthGoal, PreferredInteractionChannel, SatisfactionScore, MonthlySpending, AIInsight, FeedbackComments, StressLevel.
Step 2️⃣: Run the Application
Run the chatbot with:

bash
Copy code
streamlit run app.py
Step 3️⃣: Chat with the Assistant
🖊️ Enter your health-related query in the input field.
🧠 The chatbot retrieves relevant customer data and provides a refined response.
🛠️ Project Workflow
1️⃣ Data Processing
📄 Reads and cleans customer data from the CSV file.
📝 Converts rows into descriptive text summaries.
✂️ Splits text into manageable chunks using RecursiveCharacterTextSplitter.
2️⃣ Vectorstore Setup
📊 Embeddings are generated using OpenAI and stored in FAISS for fast similarity-based searches.
3️⃣ Query Handling
🔍 Matches user queries with relevant customer data.
🧩 Combines retrieved data and user questions to create context-enriched prompts.
4️⃣ AI Response Generation
🛠️ Formats a prompt with ChatPromptTemplate.
💡 Generates a detailed, user-specific response using OpenAI's language model.
🎛️ Customization
🔄 Modify Customer Data
Update the CSV file with additional insights or fields to enhance responses.

🎨 Adjust LLM Behavior
🔥 Modify the temperature parameter for more or less creative responses.
🖋️ Customize the ChatPromptTemplate to adjust tone or style.
🧩 Extend Functionality
🎤 Add voice input for greater accessibility.
🌐 Integrate external APIs for real-time health recommendations.
⚠️ Limitations
📋 Requires well-structured and complete input data for best results.
🛠️ Depends on OpenAI API, so an active key is essential.
🤔 May generate less accurate responses if data quality is poor.
🖊️ Author
[Your Name]

📜 License
[Specify your license, e.g., MIT License]

Enjoy building your health assistant! 🌟






