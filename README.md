# Talk to Code

Talk to Code is a Python-based tool that allows you to have a conversation with any GitHub repository. By cloning the repository and processing its contents, it enables you to ask questions about the codebase and receive AI-generated explanations and insights using Google's Gemini model.

## Features

-   **Repo Cloning**: Automatically clones any public GitHub repository.
-   **Codebase Analysis**: Ingests the entire file structure and content for context.
-   **Interactive Chat**: Ask questions about the code in natural language.
-   **Markdown Output**: Saves detailed responses to `output.md` for easy reading.

## Prerequisites

-   Python 3.8 or higher
-   Git installed and accessible in your terminal
-   A Google Gemini API Key

## Installation

1.  Clone this repository:
    ```bash
    git clone https://github.com/aidankeighron/talk-to-code
    cd talk-to-code
    ```

2.  Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Configuration

1.  Create a `.env` file in the project root.
2.  Add your GitHub repository URL and Gemini API key:

    ```env
    GITHUB_REPO=https://github.com/username/repository
    GEMINI_API_KEY=your_api_key_here
    ```

    > You can get a free Gemini API key from [Google AI Studio](https://aistudio.google.com/app/apikey).

## Usage

1.  Run the main script:
    ```bash
    python main.py
    ```

2.  Wait for the repository to be cloned and processed.
3.  Enter your questions when prompted.
4.  Type `q` to exit the program.
5.  View the answers in the generated `output.md` file.
