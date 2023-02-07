# Sentence Formatter

## Introduction

This program is a simple web application that takes in a multi-line text input, processes it and outputs a text with the following conditions:
- Each sentence starts with a capital letter
- Each sentence ends with a full stop, except for sentences that end with a question mark or an exclamation mark
- Multiple full stops are merged into one

# Usage
- Copy and paste the text you want to format into the text area.
- The formatted text will appear in the output area.

# The text processing logic
- Split the input text into sentences based on line breaks (\r\n)
- Capitalize the first letter of each sentence
- Add a full stop to the end of each sentence, except for sentences that end - with a question mark or an exclamation mark
- Merge multiple full stops into one
- Join the sentences back into a single string

# Implementation
- The height and width of the program is height: 317px; width: 504px;
- The program uses HTML, CSS, and JavaScript to build the user interface and implement the text processing logic.
- The text is split into sentences using the following regular expression: /([.!?])\s+(?=[A-Z])/g.
- The first letter of each sentence is converted to uppercase using the .toUpperCase() method.
- A single period is added to the end of each sentence, unless the sentence already ends with a question mark or exclamation point.
- The sentences are joined together using .join(". ") to create the final output string.
