# OCR → LLM Pipeline Take-Home Assignment

## Objective
You’ll build a pipeline that:
1. Extracts text from a medical-legal document using OCR.
2. Cleans the text to improve readability and accuracy.
3. Uses an LLM to answer questions about the document.

This assignment is designed to mimic real-world challenges in our OCR → LLM pipeline and should take **3-4 hours** to complete.

---

## Steps
1. **OCR Extraction**: Use an OCR library (e.g., `pytesseract` or `easyocr`) to extract text from `sample_document.pdf`.
2. **Text Cleaning**: Write a script to clean the OCR output (e.g., remove noise, fix line breaks, handle special characters).
3. **LLM Integration**: Use OpenAI’s GPT-4 API to answer questions from `sample_questions.txt` based on the cleaned text.
4. **Pipeline Script**: Combine the above steps into a single script (`pipeline.py`) that takes a PDF and questions as input and outputs answers.

---

## Deliverables
- A working pipeline script (`pipeline.py`).
- Cleaned OCR output saved to a file (`cleaned_text.txt`).
- Answers to the questions saved to a file (`answers.txt`).
- A brief write-up (1-2 paragraphs) explaining:
  - Your approach to text cleaning.
  - Any assumptions or trade-offs you made.
  - How you’d improve the pipeline given more time.

---

## Getting Started
1. Clone this repo:
   ```bash
   git clone <repo-url>
   cd ocr-llm-pipeline
  ```

2. Install the requirements
  ```bash
  pip install -r requirements.txt
  ```

3. Add your OpenAI API key to a .env file (a temporary API key will be provided to you):
   OPENAI_API_KEY=your-api-key-here

4. python src/pipeline.py

---

## Files
data/sample_document.pdf: A sample medical-legal document with noise (e.g., handwritten notes, smudges).

data/sample_questions.txt: Predefined questions about the document.

src/ocr.py: Starter code for OCR extraction.

src/text_cleaner.py: Starter code for text cleaning.

src/llm_qa.py: Starter code for LLM question-answering.

src/pipeline.py: Main pipeline script (to be completed).

---
## Evaluation Criteria

Code Quality: Is the code clean, modular, and well-documented?

Text Cleaning: Did you handle noise effectively? Did you explain your approach?

LLM Integration: Are the answers accurate and relevant?

Critical Thinking: Did you identify meaningful improvements or trade-offs?
---
## Bonus Challenge (Optional)
If you finish early, consider:

Performance Optimization: How would you handle a 10,000-page document?

Error Handling: How would you deal with OCR failures or ambiguous LLM outputs?
---
## Submission
Fork this repo and push your changes.

Share the link to your fork with us.

Good luck! We’re excited to see what you build.
