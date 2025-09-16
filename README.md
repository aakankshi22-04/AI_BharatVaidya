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

### Prerequisites
- Install Python version 3.11 (pyenv recommended)
- Docker for running Milvus vector database

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/aakankshi22-04/AI_BharatVaidya.git
   cd AI_BharatVaidya
   ```

2. Install dependencies and setup virtual environment:
   ```bash
   ./install_dependencies.sh
   source .venv/bin/activate
   ```

3. Create `.env` file and populate it with API keys:
   ```bash
   echo "OPENAI_API_KEY=your_openai_api_key_here" > .env
   ```

### Running the Application

1. Start the Milvus Vector Database container:
   ```bash
   docker compose up
   ```

2. Start the application:
   ```bash
   ./run_app.sh
   ```

3. Open your browser and navigate to: `http://localhost:5000`

## 📁 Project Structure

The application follows a modular architecture to ensure flexibility and maintainability:

- **`app/services/llm_interaction.py`**: Abstraction layer for interacting with language models (LLMs) and embeddings
- **`app/services/chat_gpt_service.py`**: ChatGPT service logic for handling conversations
- **`app/routes/`**: Route definitions for handling web requests
- **`app/utils/util.py`**: Utility functions for various operations
- **`pdf_to_json/`**: GROBID integration for processing Ayurvedic texts
- **`tests/`**: Unit tests for the application

## 🚫 Ignored Files

The following files and directories are excluded from version control for performance and security reasons:

- **`vector_files/`**: Large FAISS index files (>20MB)
- **`pdf_to_json/input_pdfs/`**: Source PDF files (>150MB total)
- **`pdf_to_json/output_xmls/`**: Generated XML files
- **`products.db`**: SQLite database files
- **`.env`**: Environment variables and API keys

These files are generated during setup or contain sensitive information. Refer to the setup instructions for regenerating them.
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



