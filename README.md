﻿
# 📄 PDF Summarizer with Multiple LLMs

This project is a web-based **PDF Summarizer** application that processes PDF files and generates concise summaries using multiple **Language Learning Models (LLMs)**. It allows users to upload PDF files and receive summaries from two distinct models, providing diverse perspectives and understanding.



## 🚀 Features

- **PDF Summarization**: Upload any PDF file and get real-time summaries from two different LLMs.
- **Multiple LLM Support**: Get summaries from **Hugging Face** and **Google Generative AI (Gemini)** models.
- **Socket.IO Integration**: Real-time updates and efficient handling of PDF uploads and summary generation.
- **Error Handling**: Robust error handling for PDF processing and LLM failures.
- **Beautiful UI**: Modern and responsive UI for seamless user interaction.

## 🛠️ Tech Stack

- **Backend**: 
  - **Node.js**: Server-side JavaScript runtime.
  - **Express.js**: Web framework for building APIs.
  - **Socket.IO**: Real-time communication between the client and server.
  - **multer**: Middleware for handling file uploads.
  - **pdf-parse**: Library for extracting text from PDF files.

- **Frontend**: 
  - **React.js**: JavaScript library for building user interfaces.
  - **Socket.IO-Client**: Real-time communication with the server.

- **Language Models (LLMs)**:
  - **Hugging Face**: Using the `facebook/bart-large-cnn` model for summarization.
  - **Google Generative AI (Gemini)**: Using **Gemini 1.5 Flash** model for text summarization.


## 📑 Usage

1. **Clone the Repository**:
   ```bash
   git clone [https://github.com/nasiriubat/gpt-pdf-summary.git](https://github.com/tarunvinodhkumar/PDF-Summarizer-using-GPT-model.git]
   cd pdf-summarizer
   ```

2. **Install Dependencies**:
   ```bash
   npm install:all
   ```

3. **Set Environment Variables**:
   Create a `.env` file in the /backend directory with the following API keys:
   ```
   GEMINI_API_KEY=your_gemini_api_key
   HUGGINGFACE_API_KEY=your_huggingface_api_key
   ```

4. **Run the Application**:
   ```bash
   npm start
   ```

5. **Run Tests**:
   Run the test cases to ensure everything is working properly:
   ```bash
   cd backend
   npm test
   ```

6. **Upload a PDF**: Open the browser and navigate to `http://localhost:5173` to upload your PDF and receive summarized outputs.

## 📦 LLM Models Used

- **Hugging Face**: `facebook/bart-large-cnn` is a state-of-the-art model for summarizing large pieces of text.
- **Gemini 1.5 Flash**: A cutting-edge model from **Google Generative AI** designed for fast and efficient content generation, providing high-quality summaries.

## ⚙️ Project Structure

```bash
.
├── backend
│   ├── app.js        # Express server & Socket.IO setup
│   ├── gemini.js     # Google Generative AI summarization logic
│   ├── hface.js      # Hugging Face summarization logic
│   ├── .env      # environment variable
│   └── test
│       └── app.test.js # Test cases for the app
├── frontend
│   └── src
│       └── App.js    # React app for uploading PDFs
└── README.md         # Project documentation
```
