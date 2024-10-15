# Ollama GUI Interface

This project provides a simple graphical interface (GUI) for interacting with the `ollama` command-line tool. The interface is built using Python's `tkinter` library and allows users to enter prompts and receive responses from a specified Ollama model. The GUI displays the conversation history, including the user prompts and the responses from Ollama, with a typing effect for added realism.

## Features

- **User-friendly interface:** Easily interact with the `ollama` command through a simple GUI.
- **Chat history:** Displays the conversation between the user and Ollama, keeping track of prompts and responses.
- **Typing effect:** The response from Ollama is displayed character by character to simulate a real-time conversation.
- **Multithreading:** Handles Ollama responses in a separate thread to prevent the interface from freezing during processing.
- **Error handling:** Includes basic error handling for missing or invalid commands.

## Prerequisites

Before using the Ollama GUI, ensure that the following are installed on your system:

- **Python 3.6+**: This script is written in Python, so you'll need Python installed to run it.
- **tkinter**: The GUI is built using `tkinter`, which is part of the Python standard library, but on some Linux systems, you may need to install it separately.
- **Ollama**: Ensure that the `ollama` command-line tool is installed and available in your system's PATH. You can download and install it from [Ollama's official website](https://ollama.com).

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/ollama-gui-interface.git
   cd ollama-gui-interface
   ```

2. **Install required Python modules:**

   This project uses Python's standard library, so no additional external dependencies are needed.

3. **Run the GUI:**

   Simply execute the following command to start the GUI:

   ```bash
   python ollama_gui.py
   ```

## Usage

1. **Model Selection:**
   - Enter the model name in the "Model Name" field. This is the model you want to use with `ollama`.
   
2. **Prompt Input:**
   - Enter your prompt in the "Prompt" field and press the `Send` button (or press `Enter` on your keyboard).

3. **View Responses:**
   - The conversation between you and the Ollama model will appear in the chat history. You will see both your prompts and the model's responses.

### Example Interaction

1. Enter a model name, e.g., `gpt-3`.
2. Type your prompt, e.g., `What is the capital of France?`, and press `Send`.
3. Ollama's response will be displayed in the chat history, with a typing effect.

## Project Structure

```
ollama_gui_interface/
│
├── ollama_gui.py     # The main Python script containing the code for the GUI interface.
└── README.md         # This README file.
```

## Error Handling

- **Missing Ollama Command:** If the `ollama` command is not found in your system's PATH, an error message will be displayed.
- **Ollama Errors:** If the `ollama` command encounters an error (e.g., invalid model name), the error will be shown in the interface.

## Future Enhancements

- **Support for Multiple Models:** Add support for switching between models more seamlessly.
- **Improved Error Handling:** Provide more specific error messages for common issues.
- **Customizable Typing Speed:** Allow users to adjust the typing effect speed.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Any feedback or suggestions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
