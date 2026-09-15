# Gemini Summarizer

## Project Overview

Gemini Summarizer is an AI-based text summarization project that uses the **Google Gemini API** to generate short and clear summaries from longer text.

The project demonstrates how generative AI can be used to simplify information and present the key points of a given text.

## Features

* AI-powered text summarization
* Uses the Google Gemini API
* Generates short and clear summaries
* Simple Python implementation
* Easy to run and modify

## Technologies Used

* Python
* Google Gemini API
* Google Generative AI SDK

## How It Works

1. Provide the input text.
2. Configure the Gemini API using an environment variable.
3. Initialize the Gemini model.
4. Send a summarization prompt to the model.
5. Generate the summary.
6. Display the original text and summarized text.

## Project Structure

```text
Gemini-Summarizer/
│
├── Gemini Summarizer code file
├── PRD file
├── README.md
└── requirements.txt
```

## Installation

Install the required dependency using:

```bash
pip install -r requirements.txt
```

## API Key Setup

For security, the Gemini API key should **not** be written directly in the source code.

Set the API key as an environment variable:

```text
GEMINI_API_KEY=your_api_key_here
```

The application reads the key using:

```python
import os
import google.generativeai as genai

genai.configure(api_key=os.getenv("GEMINI_API_KEY"))
```

## Example

### Input

```text
Machine learning helps computers learn from data and improve performance without explicit programming. It is widely used in recommendation systems and fraud detection.
```

### Output

The Gemini model generates a short and clear summary of the provided text.

## Project Documentation

The complete Project Requirements Document (PRD) is available in this repository.

## Purpose

This project demonstrates the use of generative AI for automatic text summarization and provides a simple example of integrating the Gemini API with Python.
