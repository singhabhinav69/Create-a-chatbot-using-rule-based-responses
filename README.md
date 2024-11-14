# Create-a-chatbot-using-rule-based-responses
# Rule-Based Chatbot

A simple, rule-based chatbot that responds to user input based on predefined rules and keywords. The chatbot uses pattern matching to provide responses and simulate conversation in a controlled environment.

## Features
- Rule-based conversation: The chatbot responds to specific keywords or patterns in user input.
- Customizable responses: Easily modify or extend the chatbot’s behavior by editing the response rules.
- No AI/ML: This is a simple rule-based implementation without advanced AI or machine learning models.

## Getting Started

### Prerequisites
- Python 3.x installed
- A basic understanding of Python

### Installation
1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/rule-based-chatbot.git
   cd rule-based-chatbot
   
2. Install dependencies:

   While this project doesn't require external libraries, you can use a virtual environment for better management:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. (Optional) Install any required dependencies:

   ```bash
   pip install -r requirements.txt
   ```
4. Run the chatbot:

   ```bash
   python chatbot.py
   ```
   
### Usage
To start a conversation with the chatbot, simply type messages into the terminal. The chatbot will respond according to the rules defined in the `responses` dictionary.

#### Example Interaction:
Welcome to the Rule-Based Chatbot! Type 'exit' to end the conversation.
User: Hello
Chatbot: Hi there! How can I help you today?

User: How are you?
Chatbot: I'm just a program, but I'm doing great! How about you?

User: Tell me a joke
Chatbot: Why don't skeletons fight each other? They don't have the guts!

User: exit
Chatbot: Goodbye! Have a nice day!

### Customizing Responses

The chatbot's behavior is defined by a set of rules and responses in the `responses` dictionary in `chatbot.py`. To add new rules or modify existing responses, follow these steps:

1. Open `chatbot.py`.
2. Look for the `responses` dictionary, where key-value pairs define possible user inputs and corresponding chatbot responses.
3. Add, remove, or modify entries as needed.

Example:
python
responses = {
    "hello": "Hi there! How can I help you today?",
    "how are you": "I'm just a program, but I'm doing great! How about you?",
    "bye": "Goodbye! Have a nice day!",
    "joke": "Why don't skeletons fight each other? They don't have the guts!",
}

To add a new response for a custom user input, simply add another key-value pair.

### Code Overview- **`chatbot.py`**: Contains the logic for the chatbot, including the rule-based response mechanism and user input handling.
- **`responses` dictionary**: A simple dictionary to map user inputs to chatbot responses.
- **`main()` function**: Runs the main loop, accepts user input, and displays appropriate responses.
- **Pattern Matching**: The chatbot matches keywords from the user input to predefined responses.


### How it Works
1. **Input Handling**: The program takes user input and compares it against predefined patterns using a case-insensitive regex search.
2. **Matching Responses**: If a match is found in the `responses` dictionary, the chatbot returns the corresponding response.
3. **Exit Condition**: The chatbot continues to interact until the user types "exit".

### Contributing
Feel free to fork the repository and submit pull requests for new features or improvements. Please ensure to follow the code style and include tests for new features where applicable.

### License
This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
