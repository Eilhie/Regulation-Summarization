# Regulation Summarization with BART Pretrained Model

This project demonstrates how to summarize regulatory documents using the **BART pretrained model** and **web scraping techniques** to gather the necessary data. The project is implemented as a Jupyter Notebook (`.ipynb`) file, allowing for an interactive and modular approach to text summarization.

---

## Project Overview

### Objective
The objective of this project is to:
1. Scrape regulatory documents from a specific website.
2. Preprocess the scraped data for summarization.
3. Use the BART pretrained model to generate concise summaries of the regulations.
4. Provide an automated workflow for obtaining and summarizing regulatory updates.

### Key Features
- **Web Scraping**: Extract regulation text and metadata from online sources.
- **Text Preprocessing**: Clean and prepare data for model input.
- **Summarization**: Generate concise summaries using a fine-tuned BART model.
- **Modular Workflow**: Each step (scraping, preprocessing, summarization) is independent and can be reused or adapted.

---

## Installation

### Prerequisites
Ensure you have the following installed:
- Python >= 3.8
- Jupyter Notebook
---

## Usage

### Step 1: Web Scraping
1. Identify the target website containing the regulatory documents.
2. Use `selenium` to extract relevant data.
3. Save the scraped data.

### Step 2: Text Preprocessing
1. Clean the text by removing unwanted characters, stopwords, and HTML tags.
2. Tokenize the text and prepare it for the model input.

### Step 3: Summarization
1. Load the BART pretrained model using the `transformers` library:
   ```python
   from transformers import BartForConditionalGeneration, BartTokenizer

   model = BartForConditionalGeneration.from_pretrained('facebook/bart-large-cnn')
   tokenizer = BartTokenizer.from_pretrained('facebook/bart-large-cnn')
   ```
2. Pass the preprocessed text to the model for summarization

### Step 4: Displaying Summary 
1. Display the summarized results.
---

## Future Improvements
- Fine-tune the BART model with domain-specific data for better summarization.
- Integrate additional preprocessing steps for more robust text cleaning.
- Automate the entire workflow with periodic updates.

---

## License
This project is licensed under the MIT License.

---

## Acknowledgments
- [Hugging Face Transformers Library](https://huggingface.co/transformers/)
- [Selenium Documentation](https://www.selenium.dev/documentation/)
- [Beautiful Soup Documentation](https://www.crummy.com/software/BeautifulSoup/)

---

## Contact

For any questions or feedback:
- Email: b.sachio88@gmail.com
- LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/marvinsachio)
