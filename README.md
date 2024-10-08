Here's a shorter version of the README file:

---

# RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot built with Django, Pinecone, and OpenAI's GPT. This bot retrieves
information from uploaded PDFs and generates responses based on the content.

## Features

- **User Authentication**: JWT-based login and registration.
- **Chatbot Management**: Create and manage chatbots with unique names.
- **PDF Upload**: Upload PDFs, process them into vector embeddings, and store in Pinecone.
- **Query Chatbot**: Retrieve information and get responses using OpenAI's GPT-3.5.

## Tech Stack

- **Backend**: Django, Django REST Framework
- **Vector Store**: Pinecone
- **LLM**: OpenAI GPT-3.5
- **Database**: SQlite

## Setup

1. Clone the repo and navigate to the directory:

    ```bash
    git clone https://github.com/your-username/rag-chatbot.git
    cd rag-chatbot
    ```

2. Set up a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate
    ```

3. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Configure environment variables in `.env`:

    ```plaintext
    OPENAI_API_KEY=your-openai-api-key
    PINECONE_API_KEY=your-pinecone-api-key
    ```

5. Run migrations and start the server:

    ```bash
    python manage.py migrate
    python manage.py runserver
    ```

## Usage

- **Register/Login**: Create and authenticate users.
- **Create Chatbot**: Use the `/api/chatbots/` endpoint.
- **Upload PDF**: Upload via `/api/upload-pdf/`.
- **Query Chatbot**: Interact via `/api/chat/`.

## License

MIT License

---

This version is concise while still covering the key points.