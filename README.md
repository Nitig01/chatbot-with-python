
## Simple Chatbot Documentation

### Overview
This application is a simple chatbot built using Python's tkinter library for the GUI and basic string matching for responses. The chatbot can respond to specific user inputs with predefined responses.

### Features
- *Interactive GUI*: A simple interface where users can type and submit their queries.
- *Predefined Responses*: The chatbot responds to specific inputs such as "hi", "how are you", "who are you", "how old are you", "what time is it", and "bye".
- *Timestamp*: The chatbot can provide the current time in response to the query "what time is it".

### Requirements
- Python 3.x
- tkinter (usually included with Python installations)

### Components

#### GUI Elements
- *Root Window*: The main application window.
- *Output Frame*: A frame to hold the chat display.
- *Output Label*: A label indicating the chat display section.
- *Output Field*: A Text widget displaying the conversation.
- *Input Frame*: A frame to hold the input section.
- *Input Label*: A label indicating the user input section.
- *Input Field*: An Entry widget where users type their queries.
- *Submit Button*: A button to submit the user input.

#### Tags
- *'blue'*: Used to color the chatbot's responses.
- *'red'*: Used to color the user's input.

### Functions

#### on_submit(event=None)
Handles user input submission. It performs the following actions:
1. Retrieves the user input from the input field.
2. Displays the user input in the output field.
3. Checks the user input against predefined responses and displays the appropriate response.
4. Clears the input field.

### Usage
1. *Run the Program*: Execute the script to launch the chatbot window.
2. *Type a Query*: Enter a query in the input field.
3. *Submit the Query*: Press the "Submit" button or hit the Enter key.
4. *View the Response*: The chatbot's response will appear in the output field.

### Example Interactions

- *User*: hi
  - *Chatbot*: Hello, how can I help you?

- *User*: how are you
  - *Chatbot*: I am Okay. How about you?

- *User*: who are you
  - *Chatbot*: I am simple chatbot

- *User*: how old are you
  - *Chatbot*: My creator just brought me to life in front of you. I am not much older than 10 minutes.

- *User*: what time is it
  - *Chatbot*: (current time)

- *User*: bye
  - *Chatbot*: Goodbye, have a nice day!

### Customization
To add more responses or change existing ones, modify the on_submit function. For example, to add a response for "hello", include:
python
elif user_input == 'hello':
    output_field.insert('end', 'Hi there!\n', 'blue')


### Limitations
- The chatbot uses basic string matching and does not understand variations of the predefined queries.
- It does not support advanced natural language processing (NLP) or machine learning features.

### Conclusion
This simple chatbot provides a foundation for creating interactive applications using tkinter. It demonstrates basic GUI elements and handling user input to produce predefined responses.

---

