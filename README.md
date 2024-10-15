
# Ollama GUI Interface

This project provides a GUI interface for interacting with the `ollama` terminal command using the `Tkinter` library in Python. It allows users to select a model, input a prompt, and view the response with basic Markdown formatting in a scrollable text box. Responses from the terminal are displayed in real-time with a typing effect.

## Features
- **Model Selection:** Users can select different `ollama` models from a dropdown menu.
- **Prompt Input:** Users can enter a prompt and receive responses from the selected model.
- **Clean Output:** The program removes unwanted ANSI escape sequences and control characters.
- **Markdown Support:** Basic Markdown formatting such as bold, italic, inline code, and hyperlinks are supported in the chat history.
- **Typing Effect:** Responses are displayed character by character, simulating a typing effect.
- **Link Handling:** Hyperlinks in the response are clickable and will open in the default web browser.

## Installation

1. **Install Python 3.x**: Ensure you have Python 3.x installed on your system. You can download it from [here](https://www.python.org/downloads/).
2. **Install Tkinter**: Tkinter comes pre-installed with Python on most platforms. If not, you can install it:
   ```bash
   sudo apt-get install python3-tk
   ```
   or use `brew install python-tk` on macOS.

3. **Install Required Libraries**:
   Install `re`, `subprocess`, and `threading` (which are part of the Python standard library) as they do not require additional installation. If `ttk` is not installed, ensure that your Python version is up to date.

4. **Install the `ollama` command**: Make sure you have the `ollama` command available and configured in your system's PATH. You can verify by running:
   ```bash
   ollama --version
   ```

## Usage

1. **Run the script**:
   To start the GUI, simply run the Python script:
   ```bash
   python ollama_gui.py
   ```

2. **Select a Model**:
   Choose the model you'd like to use from the dropdown menu.

3. **Enter a Prompt**:
   Type your prompt in the input box and press the `Send` button or hit `Enter`.

4. **View the Response**:
   The response will be displayed in the chat history area with basic Markdown formatting.

## Markdown Support
- **Bold**: `**text**` or `__text__`
- **Italic**: `*text*` or `_text_`
- **Inline Code**: `` `code` ``
- **Hyperlinks**: `[text](url)`

## Error Handling
- If the `ollama` command is not found or an error occurs during execution, an error message will be displayed using a pop-up dialog.

## Example Usage

1. Select `llama3.2:1b` from the model dropdown.
2. Enter the prompt:
   ```
   Tell me a joke about meta.
   ```
3. The response will be displayed with a typing effect in the chat history.

## Contributions
Feel free to contribute to this project by adding new features, fixing bugs, or improving existing functionality. Fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License.

Enjoy using the Ollama GUI interface!
