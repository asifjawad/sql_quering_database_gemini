# SQL Query using Gemini

This project demonstrates how to retrieve SQL queries using Google’s Gemini model. It allows users to input questions in English, and the model generates corresponding SQL queries. The queries are then executed on an SQLite database named student.db.

## Installation
Make sure you have Python installed.

- Clone this repository.
- Install the required packages using pip install -r requirements.txt.
- Set up your Google API key by creating a `.env` file with the following content:
`GOOGLE_API_KEY=your_api_key_here`
- Run the Streamlit app using `streamlit run APP.py`.

## Usage
- Enter your English question in the input field.
- Click the “Ask the question” button.
- The Gemini model will generate an SQL query based on your question.
- The query will be executed on the student.db database.
- The response will be displayed below.

## Example Questions
How many entries of records are present?
- SQL query: `SELECT COUNT(*) FROM STUDENT`;
Tell me all the students studying in Data Science class?
- SQL query: `SELECT * FROM STUDENT WHERE CLASS="Data Science"`;

Note: Ensure that the SQL code does not have triple backticks (```) at the beginning or end, and the word “sql” should not appear in the output.
