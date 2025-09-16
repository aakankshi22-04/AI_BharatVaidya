


<<<<<<< HEAD
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
=======
# Setup
- Install Python version 3.11 (pyenv recommended)
- Run the `install_dependencies.sh` script to install requirements and setup a virtual environment (`.venv`)
- Activate the virtual environment `source .venv/bin/activate`
- Create `.env` file and populate it with API keys:
    - `OPENAI_API_KEY`

# Running Locally
Standup the Milvus Vector Database container by running:
```shell
docker compose up
```

Then run the `run_app.sh` script to start a local instance of the application:
```shell
./run_app.sh
```

Once the application starts, open your browser and navigate to:
```
http://localhost:5000
```

# Application Architecture

The application follows a modular architecture to ensure flexibility and maintainability. Here's an overview of the main components:

- **`app/services/llm_interaction.py`**: This module provides an abstraction layer for interacting with language models (LLMs) and embeddings. It allows the application to dynamically switch between different LLMs based on configuration, without modifying the codebase.

- **`app/utils/util.py`**: This module contains utility functions for car diagnostics, such as generating diagnostic context using the selected LLM and embeddings.

- **`app/routes/`**: This directory contains the route definitions for the application, including routes for handling ChatGPT interactions and form submissions.

- **`app/__init__.py`**: This module initializes the Flask application and sets up the necessary configurations, such as loading environment variables and registering blueprints.
>>>>>>> 2470582 (Initial commit with full project structure)



