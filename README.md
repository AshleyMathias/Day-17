# Day-17
Quiz Program 🧠
This project is a simple console-based quiz game that uses object-oriented programming principles. The game reads questions and their answers from a data file, processes them into a question bank, and allows the user to answer them interactively.

Features 🌟
Dynamic Question Bank: Fetches questions and answers from a data file.
Interactive Quiz: Asks questions one at a time and validates user responses.
Score Tracking: Keeps track of correct answers and displays the final score.
Prerequisites 📋
Python 3.x installed on your system.
Ensure the following modules/files are included:
question_model.py
data.py
quiz_brain.py
How to Run the Program 🚀
Clone or download this repository.
Ensure the following files are in the directory:
question_model.py: Handles the Question class.
data.py: Contains the question_data (a list of dictionaries with question text and answers).
quiz_brain.py: Implements the quiz logic.
Open the main script file in your preferred Python IDE or text editor.
Run the program using:
bash
Copy
Edit
python main.py
Program Flow 🔄
Initialize Questions:

The program reads questions from data.py.
Each question is converted into a Question object and added to a question bank.
Start Quiz:

The Quizbrain object initializes the game and displays questions one by one.
User inputs their answer for each question.
Validate Answers:

The program checks the user's input against the correct answer.
Keeps track of the user's score.
End Game:

Displays the user's final score and ends the quiz.
Modules Overview 🛠️
1. Question Module
Represents a single question.
Attributes:
text: The text of the question.
answer: The correct answer to the question.
2. data Module
Contains question_data, a list of dictionaries.
Each dictionary has:
text: Question text.
answer: Correct answer ("True" or "False").
3. Quizbrain Module
Manages the quiz flow.
Attributes:
question_number: Tracks the current question number.
score: Tracks the user's score.
Methods:
still_has_question(): Checks if there are remaining questions.
next_question(): Displays the next question and gets user input.
