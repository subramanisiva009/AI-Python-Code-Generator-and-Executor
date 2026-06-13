# 🤖 AI Python Code Generator & Executor

This project uses Google's Gemini AI and LangChain to generate Python code from natural language instructions and execute the generated code automatically using PythonREPL.

## Overview

The application accepts a user instruction, sends it to Gemini AI, generates executable Python code, and then runs the code in a Python REPL environment. This demonstrates the integration of Large Language Models (LLMs) with automated code generation and execution workflows.

## Features

* Natural language to Python code generation
* Powered by Gemini 2.5 Flash
* Prompt engineering using LangChain
* Automatic Python code execution
* Simple and lightweight implementation
* Error handling during execution

## Technologies Used

* Python
* LangChain
* Google Gemini AI
* PythonREPL
* Python Dotenv

## Project Workflow

1. Load the Gemini API key from the environment file.
2. Initialize the Gemini language model.
3. Create a structured prompt template.
4. Send the user instruction to Gemini.
5. Generate executable Python code.
6. Execute the generated code using PythonREPL.
7. Display both the generated code and execution results.

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/ai-python-code-generator.git
cd ai-python-code-generator
```

Install the required dependencies:

```bash
pip install langchain langchain-google-genai langchain-experimental python-dotenv
```

## Environment Setup

Create a `.env` file in the project root directory:

```env
GEMINI_APIKEY=your_gemini_api_key
```

## Usage

Run the application:

```bash
python app.py
```

Example instruction:

```python
instruction = "Write a code to find even and odd numbers from an array"
```

Example Output:

```text
----- Generated Code -----
numbers = [1, 2, 3, 4, 5, 6]

even = [n for n in numbers if n % 2 == 0]
odd = [n for n in numbers if n % 2 != 0]

print("Even Numbers:", even)
print("Odd Numbers:", odd)

----- Execution Output -----
Even Numbers: [2, 4, 6]
Odd Numbers: [1, 3, 5]
```

## Future Enhancements

* Streamlit-based user interface
* Voice-to-code generation
* Multi-language code generation
* Secure sandboxed code execution
* Interactive chatbot support

## Author

Siva Prasad

## License

This project is licensed under the MIT License.
