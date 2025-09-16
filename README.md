# Assignment Y - Conversation Summarization and User Info Extraction

## Overview

This Jupyter notebook (`Assignment y.ipynb`) implements a conversation summarization system and user information extraction tool using the Groq API. It demonstrates advanced techniques for managing long-form conversations in AI applications, including automatic summarization, history truncation, and structured data extraction with validation.

The project showcases practical implementations for handling conversational AI contexts, such as chatbots, virtual assistants, and research applications requiring condensed dialogue management.

## Features

- **Conversation History Management**: Store and track user-assistant interactions with role-based messaging.
- **Automatic Summarization**: Leverage Groq's language models to generate concise summaries of conversation threads.
- **Truncation Strategies**:
  - Truncate by number of conversation turns.
  - Truncate by total character length to manage memory and context.
- **Periodic Summarization**: Automatically summarize conversations at regular intervals to maintain context without excessive history.
- **User Information Extraction**: Extract structured personal details (name, email, phone, location, age) from chat texts using JSON schema.
- **Data Validation**: Validate extracted information against predefined JSON schemas for accuracy and consistency.

## Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab
- Internet connection for API calls
- Groq API key (obtain from [Groq Console](https://console.groq.com/))

## Installation

1. **Clone or Download** the notebook file to your local machine.

2. **Install Required Packages**:
   ```bash
   pip install openai jsonschema
   ```

3. **Set Up API Key**:
   - Obtain your Groq API key from the Groq Console.
   - In the notebook, replace the placeholder API key with your actual key:
     ```python
     os.environ["OPENAI_API_KEY"] = "your_groq_api_key_here"
     ```
   - **Security Note**: Avoid hardcoding API keys in production code. Use environment variables instead.

## Usage

1. **Launch Jupyter**:
   ```bash
   jupyter notebook
   ```

2. **Open the Notebook**:
   - Navigate to `Assignment y.ipynb` and open it.

3. **Run the Cells**:
   - Execute cells sequentially to see demonstrations.
   - The notebook includes interactive examples for:
     - Conversation flow with summarization.
     - Truncation demonstrations.
     - User information extraction from sample chats.

4. **Customization**:
   - Modify summarization intervals, truncation parameters, or JSON schemas as needed.
   - Adapt the code for integration into larger AI systems.

## Examples

### Conversation Summarization
The notebook demonstrates summarization in various contexts:
- Technical project discussions
- AI research scenarios
- Academic assignments

### User Info Extraction
Sample chats are processed to extract structured data:
```json
{
  "name": "Priya Patel",
  "email": "priya.patel@techfirm.com",
  "phone": "8765432109",
  "location": "Pune",
  "age": 27
}
```

### Truncation Methods
- Keep only the last N conversation turns.
- Limit total conversation length to a specified character count.

## Dependencies

- `openai`: For Groq API integration
- `jsonschema`: For JSON schema validation
- `os`: For environment variable management
- `json`: For JSON handling

## Notes

- The notebook uses the `moonshotai/kimi-k2-instruct-0905` model via Groq for both summarization and extraction tasks.
- API calls may incur costs based on your Groq plan.
- Ensure compliance with data privacy regulations when handling personal information.

## Contributing

This is an assignment project. For educational purposes, feel free to modify and extend the code.

## License

This project is for educational use. No specific license is applied.
