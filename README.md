# **Web Scraping and Question-Answering from Web Content**

This repository demonstrates a simple approach to scrape text from a webpage and use a pre-trained question-answering model to extract relevant information from the scraped content.

## **Features**

Scrapes text content from a specified URL.
Cleans the scraped text to remove extra whitespace.
Uses the transformers library's pre-trained question-answering model to answer questions based on the content of the webpage.

## **Requirements**

**requests:** For fetching the webpage content.
**BeautifulSoup from bs4:** For parsing the HTML and extracting text.
**re:** For cleaning up the scraped text.
**pipeline from transformers:** For using the pre-trained question-answering model.

## **Scraping Function:**

The scrape_website function takes a URL, sends a GET request to the website, and extracts the text from all paragraph (<p>) tags.
The extracted text is cleaned by removing unnecessary spaces and joining the text into a single string.

## **Question-Answering:**

A pre-trained question-answering model is loaded using the pipeline function from Hugging Face's transformers.
The qa_model is used to answer the question "What services does the website offer?" based on the content extracted from the webpage.
