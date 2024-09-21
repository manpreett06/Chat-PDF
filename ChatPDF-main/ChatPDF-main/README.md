# ChatPDF

## Introduction
------------
The ChatPDF App is a Python tool designed for conversing with multiple PDF documents. Through this application, users can engage in dialogue using natural language to inquire about the content of the PDFs. The app generates relevant responses based on the documents' information, leveraging a language model for accurate answers. It's important to note that the app will only respond to queries that pertain to the loaded PDFs.

## How It Works
------------
![PDF-LangChain](https://github.com/aviraj2501/ChatPDF/assets/148218162/90bdcfa4-dce1-4ccb-a78e-eebd0e6a590f)

The application follows these steps to provide responses to your questions:

1. PDF Loading: The app reads multiple PDF documents and extracts their text content.

2. Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

3. Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

## Dependencies and Installation
----------------------------
To install the ChatPDF App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from OpenAI and add it to the `.env` file in the project directory.
```commandline
OPENAI_API_KEY=your_secret_api_key
HUGGINGFACEHUB_API_TOKEN=your_secret_api_key
```

## Usage
-----
To use the MultiPDF Chat App, follow these steps:

1. Ensure that you have installed the required dependencies and added the OpenAI API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.


