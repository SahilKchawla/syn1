# SynGPT

SynGPT is a Python-based project that leverages the power of OpenAI's GPT-3.5 model to read and understand PDF documents or uploaded text. It allows users to ask questions related to the content of these documents and receive informative responses.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Getting API Key](#getting-api-key)
  - [Examples](#examples)

## Getting Started

Follow these instructions to get SynGPT up and running on your local machine.

### Prerequisites

Before you begin, make sure you have the following installed:

- Python 3.6 or higher
- pip package manager

### Installation

1. Clone the SynGPT repository:

   ```shell
   git clone https://github.com/bhanujoshi24/SynGPT.git
   ```

2. Navigate to the project directory:

   ```shell
   cd SynGPT
   ```

3. Install the required Python dependencies:

   ```shell
   pip install -r requirements.txt
   ```

## Usage

### Getting API Key

To use SynGPT, you'll need an API key from OpenAI. Follow these steps to get your API key:

1. Visit the [OpenAI Developer](https://beta.openai.com/signup/) platform and sign up for an account.

2. Once you're logged in, create a new API key.

3. Copy your API key.

4. Set your API key as an environment variable on your local machine:

   ```shell
   export OPENAI_API_KEY=YOUR_API_KEY_HERE
   ```

### Examples

You can use SynGPT in various ways. Here are some example use cases:

#### Reading a PDF document

```python
from synGPT import SynGPT

# Initialize the SynGPT instance
syn_gpt = SynGPT()

# Read a PDF document
document_path = "path/to/your/document.pdf"
syn_gpt.read_pdf(document_path)

# Ask a question related to the document
question = "What is the main topic of the document?"
response = syn_gpt.ask_question(question)

# Print the response
print(response)
```

#### Uploading text

```python
from synGPT import SynGPT

# Initialize the SynGPT instance
syn_gpt = SynGPT()

# Upload text
text = "This is some sample text that you can upload to SynGPT."
syn_gpt.upload_text(text)

# Ask a question related to the text
question = "What is the main idea in the uploaded text?"
response = syn_gpt.ask_question(question)

# Print the response
print(response)
```
Please replace the placeholder text (e.g., `YOUR_API_KEY_HERE`) and customize the examples and usage instructions to match the specific details of your project. Additionally, consider adding more sections or information as needed to make your README file comprehensive and user-friendly.
