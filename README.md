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

4. Set your API key to api_keys.py and docker-compose.yml:

   ```shell
   api_keys.py :
     class ApiKey:
        OPEN_API_KEY = "YOUR_API_KEY_HERE"

   export OPENAI_API_KEY=YOUR_API_KEY_HERE

   docker_compose.yml :
       environment:
          OPENAI_API_KEY: "YOUR_API_KEY_HERE"
   ```

### Examples

You can use SynGPT in various ways. Here are some example use cases:

#### Reading a PDF document

```
  register : To register with new username, password and email.
  login : Login with the created username and password.
  upload : Upload the document from the local folder.
  process : Process the document.
  summary : Get the summary regarding the uploaded pdf.
  prompt : ask the questions regarding pdf to get the answers.
  Logout : Logged out of the system.
```

#### Uploading text

```
  register : To register with new username, password and email.
  login : Login with the created username and password.
  user_text : copy & paste the text.
  process : Process the document.
  summary : Get the summary regarding the uploaded pdf.
  prompt : ask the questions regarding text to get the answers.
  Logout : Logged out of the system.
```
Please replace the placeholder text (e.g., `YOUR_API_KEY_HERE`) and customize the examples and usage instructions to match the specific details of your project. Additionally, consider adding more sections or information as needed to make your README file comprehensive and user-friendly.
