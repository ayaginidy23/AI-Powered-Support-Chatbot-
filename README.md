# AI-Powered  Support Chatbot

This project introduces an AI-powered **Technical Support Chatbot** designed to enhance the support experience for students at educational institutions. The chatbot leverages **LLaMA 3** (Meta AI) to provide accurate, dynamic responses in both **English** and **Arabic**. By automating the process of answering technical support queries, it reduces the reliance on human staff, improves operational efficiency, and enhances student satisfaction.

(https://github.com/ayaginidy23/AI-Powered-Support-Chatbot-/blob/5f9ccdb59b00844e1fb16309837d6e621f2b0e60/Chatbot.png)



## Table of Contents

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Project Objectives](#project-objectives)
4. [System Design](#system-design)
5. [Key Features](#key-features)
6. [Technologies Used](#technologies-used)
7. [Installation](#installation)
8. [Usage](#usage)
9. [Challenges](#challenges)
10. [Evaluation](#evaluation)
11. [Future Work](#future-work)
12. [Conclusion](#conclusion)
13. [Contributing](#contributing)
14. [Team Members](#team-members)

## Introduction

In modern educational institutions, students often struggle to get quick and accurate technical support. Traditional systems that depend on human staff or static FAQs often fail to provide timely assistance, especially during off-hours. Our **AI-Based Technical Support Chatbot** aims to solve this issue by providing a fast, multilingual, and AI-powered solution that allows students to get instant responses to their queries. The system uses **LLaMA 3** (Meta AI), a state-of-the-art language model, to process and respond to inquiries in both **English** and **Arabic**, improving accessibility and efficiency.

## Problem Statement

Educational institutions face several challenges in managing technical support, including:

* **High Volume of Queries**: Repetitive and frequent questions overwhelm human support staff.
* **Delayed Responses**: Traditional support teams cannot offer 24/7 service, leading to delays.
* **Limited Scalability**: Scaling human-based systems is costly and resource-intensive.
* **Inadequate Solutions**: Existing chatbots are typically limited to predefined questions and cannot handle complex queries.

These challenges lead to delayed support, high operational costs, and increased frustration among students.

## Project Objectives

The primary objectives of the **AI-Based Technical Support Chatbot** are:

* To develop an AI-driven chatbot capable of understanding and processing technical queries in **English** and **Arabic**.
* To automate the retrieval of answers from a structured FAQ knowledge base.
* To implement fallback mechanisms for email redirection when the chatbot cannot handle a query.
* To reduce response time and improve student satisfaction.
* To minimize reliance on human support, thus reducing operational costs.

## System Design

### 1. Frontend (HTML/CSS + JavaScript)

A clean, intuitive web interface where students can enter queries and receive instant answers.

### 2. Backend (Flask API)

Handles business logic, manages queries, and processes responses from the FAQ database and **LLaMA 3**.

### 3. Document Processing Engine

* Extracts text from `.docx` FAQ documents.
* Splits content into manageable chunks to optimize retrieval performance.

### 4. Embedding and Retrieval (FAISS)

* Uses **Sentence Transformers** to convert FAQ text chunks into vector embeddings.
* Stores embeddings in a **FAISS** FlatL2 index for fast similarity-based search.

### 5. LLaMA Model Integration

* Integrates **LLaMA 3-8B** via the **Groq API** to interpret user queries and generate relevant responses.

### 6. Language Detection (langdetect)

* Automatically detects the language of the input and adjusts processing accordingly.

### 7. Fallback Mechanism

* If the chatbot cannot answer a query, it redirects the user to email support.

## Key Features

* **AI-Powered Instant Responses**: Processes dynamic queries efficiently.
* **Multilingual Support**: Supports both **English** and **Arabic** for a wider user base.
* **Vector-Based Retrieval**: Quickly identifies the most relevant FAQ responses.
* **Fallback Support**: Redirects unresolved queries to email support.
* **Simple User Interface**: Designed for students with varying technical backgrounds.

## Technologies Used

* **LLaMA 3**: NLP model for generating dynamic responses.
* **Flask**: Backend framework to handle API requests and responses.
* **FAISS**: Vector-based search for fast document retrieval.
* **Sentence Transformers**: For converting text into embeddings.
* **langdetect**: For automatic language detection.
* **HTML/CSS/JavaScript**: For creating the user interface.

## Installation

To run the AI-based chatbot locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/ayaginidy23/AI-Powered-Support-Chatbot.git
   cd AI-Technical-Support-Chatbot
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up the environment variables for **LLaMA 3** and **FAISS** integration.

4. Start the Flask application:

   ```bash
   python app.py
   ```

5. Open your browser and access the chatbot interface at `http://127.0.0.1:5000`.

## Usage

1. Visit the chatbot interface in your web browser.
2. Type a technical query in either **English** or **Arabic**.
3. The chatbot will respond with the most relevant answer from the FAQ knowledge base.
4. If the chatbot cannot provide an answer, it will redirect you to email support.

## Challenges

* **Multilingual Processing**: Ensuring that both **English** and **Arabic** queries are understood and processed accurately.
* **Efficient Document Chunking**: Balancing the chunk size to ensure optimal retrieval performance.
* **Fallback Handling**: Designing a smooth transition from the chatbot to email support when necessary.
* **Query Ambiguity**: Handling unclear or vague queries required advanced preprocessing and robust interpretation.

## Evaluation

The system has been evaluated based on the following metrics:

* **Accuracy**: Correctness of the chatbot's responses.
* **Response Time**: Minimal delay between the query and response.
* **User Satisfaction**: Feedback gathered from pilot testing among students.

### Expected Outcomes

* A **70% reduction** in human workload for repetitive queries.
* 24/7 availability of support for students.
* Faster and more accurate responses to technical queries.
* Support for both **English** and **Arabic**.

## Future Work

* Improve the chatbot's ability to handle more complex queries.
* Enhance the multilingual capabilities to support more languages.
* Integrate with other institutional systems for even more automated support.
* Optimize the system for mobile platforms.

## Conclusion

The **AI-Based Technical Support Chatbot** provides an efficient, scalable, and multilingual solution for technical support in educational institutions. By using **LLaMA 3**, the system offers accurate, context-aware responses without relying on proprietary models like **GPT**. It ensures that students can get the support they need quickly and at any time, reducing the workload for human support staff and improving overall student satisfaction.

## Contributing

We welcome contributions to improve the chatbot. Please fork the repository, create a new branch, and submit a pull request with your improvements.


## Team Members

* **Aya Tamer Ginidy** 
* **Amr Khaled Gaber**
* **Mohamed Talat Elslmawy** 
* **Ahmed Mohamed Dawood** 
* **George Nashaat Mosaed** 
