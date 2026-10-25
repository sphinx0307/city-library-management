# City Library Management System

A Python-based, menu-driven library management system developed as part of an IIT assignment. The implementation uses object-oriented programming and Python's standard library.

## Features

- Add books with a book ID, title, author, genre, and copy count.
- Register library members.
- Issue multiple copies of a book, subject to availability and a per-member limit of five borrowed copies.
- Return borrowed copies with quantity validation.
- Search books by title or author.
- List available books by genre.
- List members with active loans.
- Display a library summary and most popular genre.
- Maintain an in-memory borrow/return transaction log with timestamps.

## Tech stack

- Python 3
- Python standard library (`datetime`)

No third-party Python packages are required.

## Run the project

The notebook contains an interactive command-line program. Run the code cell in a Jupyter environment that supports `input()`, or copy the code into a `.py` file and run it in a terminal:

```bash
python city_library_management.py
```

The application prompts for menu choices and the details required for each operation.

## Important limitations

- Books, members, and transaction logs are stored in memory and are lost when the program exits.
- Input conversion is not wrapped in error handling, so non-numeric values entered for numeric fields can raise an exception.
- This is an educational assignment, not a production library system.

## Repository contents

- `city_library_management.ipynb` — original Part A implementation, separated from the unrelated Retail Transactions Insights assignment.
- `requirements.txt` — no third-party dependencies are required.
- `.gitignore` — ignores common Python, Jupyter, and local-environment files.

## Future improvements

- Add automated tests for successful and invalid operations.
- Validate user input and handle malformed values.
- Persist records using a database or file storage.
- Add book/member update and deletion workflows.
- Track due dates and overdue returns.
