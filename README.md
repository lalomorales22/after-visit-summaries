# Nurse After-Visit Summary Assistant

## Description
The Nurse After-Visit Summary Assistant is a Streamlit-based application designed to help nurses create comprehensive and accurate after-visit summaries. It uses AI models from both OpenAI and Ollama to provide intelligent assistance, answer questions, and offer suggestions based on medical best practices.

## Features
- AI-powered assistance for creating after-visit summaries
- Support for multiple AI models (OpenAI GPT models and Ollama models)
- Customizable categories for summary content
- Ability to add new custom categories on-the-fly
- Dark/Light theme toggle
- Conversation saving and loading functionality
- Token usage tracking

## Requirements
- Python 3.7+
- Streamlit
- OpenAI Python library
- Ollama Python library
- python-dotenv (for environment variable management)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/nurse-after-visit-summary-assistant.git
   cd nurse-after-visit-summary-assistant
   ```

2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

4. Set up your OpenAI API key:
   - Create a `.env` file in the project root
   - Add your OpenAI API key to the `.env` file:
     ```
     OPENAI_API_KEY=your_api_key_here
     ```

5. Ensure Ollama is installed and running on your system (if you plan to use Ollama models)

## Usage

1. Run the Streamlit app:
   ```
   streamlit run app.py
   ```

2. Open your web browser and go to the URL provided by Streamlit (usually http://localhost:8501)

3. Use the sidebar to:
   - Select an AI model
   - Choose existing categories or add new ones
   - Customize the AI instructions
   - Toggle between light and dark themes
   - Save or load conversations

4. Enter your queries or information in the chat input at the bottom of the page

5. The AI assistant will provide responses to help you create your after-visit summary

## Customization

- To add new default categories, edit the `SUMMARY_CATEGORIES` list in the `app.py` file
- To modify the AI's behavior, adjust the `custom_instructions` text in the `app.py` file

## Contributing

Contributions to improve the Nurse After-Visit Summary Assistant are welcome. Please feel free to submit pull requests or open issues to discuss potential changes or enhancements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This application is designed as an assistant tool and should not replace professional medical judgment. Always refer to your healthcare facility's policies and guidelines when creating official medical documentation.
