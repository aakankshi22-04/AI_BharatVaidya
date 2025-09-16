# AI_BharatVaidya
BharatVaidya is an AI-powered Ayurvedic assistant that provides personalized health advice by combining ancient wisdom with AI, NLP and Vector Databases for ingredient transparency, helping users access trusted remedies and tailored wellness solutions.

## 🔑 Key Features

- Personalized health suggestions using symptoms, lifestyle, and body constitution (prakriti)
- Ingredient traceability with blockchain for verified Ayurvedic products
- Real-time recommendations using OpenAI embeddings and LangChain
- Multimodal user experience with text, audio guidance, and AR demonstrations
- Secure and scalable architecture with session management and database optimization


## 🛠 Technologies Used

- **Python, Flask** – Backend APIs and web services
- **OpenAI embeddings, LangChain** – NLP and semantic understanding
- **Milvus** – Vector database for efficient similarity search
- **SQLite** – Product database management
- **GROBID** – PDF to XML conversion for structured text extraction
- **Blockchain** – Ingredient traceability and compliance assurance
- **HTML, CSS, JavaScript** – Interactive and responsive frontend interface


## ⚙ How It Works

1. Ayurvedic texts like Charak Samhita are converted into structured XML using GROBID.
2. Text is split into chunks and transformed into embeddings using OpenAI models.
3. User inputs—symptoms, medical history, and lifestyle—are analyzed to match remedies.
4. Ingredient data is verified with blockchain to ensure authenticity and trustworthiness.
5. Personalized suggestions are provided through an intuitive chatbot interface with real-time feedback.



## 🚀 Setup Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/AI_Bharatvaidya.git

2. Navigate to the project folder:
     cd AI_Bharatvaidya

3. Install the required dependenices:
     pip install -r requirements.txt

4.Configure environment variables (.env) with API keys and database credentials.

5.Run the Flask server:
    python app.py
    
6.Open the web browser at http://localhost:5000 and start interacting with the chatbot.



