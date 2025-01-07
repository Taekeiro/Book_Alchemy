# Book Alchemy 📚

Book Alchemy is a Flask-based web application for managing a personal book collection. Users can add authors, add books, view book details, and delete books easily using a web interface.

## Features

- **Add Authors:** Add authors with name, birth date, and date of death.
- **Add Books:** Add books with title, ISBN, publication year, and link to an author.
- **View Books:** Browse and search through the list of books with their authors and cover images.
- **Delete Books:** Remove books from the collection with a confirmation prompt.

## Project Structure

```plaintext
📦Book Alchemy
├── 📄 app.py              # Main Flask application
├── 📄 data_models.py      # SQLAlchemy models for Author and Book
├── 📄 library.sqlite      # SQLite database file
├── 📂 static
│   ├── 📄 styles.css      # Styling for the web pages
│   └── 📄 script.js       # Client-side form validation and interactive features
├── 📂 templates
│   ├── 📄 home.html       # Homepage displaying books
│   ├── 📄 add_author.html # Form for adding an author
│   ├── 📄 add_book.html   # Form for adding a book
│   ├── 📄 book_detail.html # Detailed view of a single book
├── 📄 background.jpeg     # Background image used in the web app
└── 📄 README.md           # Project documentation (this file)
```

## Technologies Used

- **Python (Flask)**: Backend server and database management.
- **HTML/CSS/JavaScript**: Frontend rendering and form validation.
- **SQLite**: Database for storing book and author information.
- **SQLAlchemy**: ORM for database interactions.

## Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Taekeiro/Book_Alchemy
   cd Book_Alchemy
   ```
2. **Create a virtual environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Initialize the database:**
   ```python
   python
   >>> from app import db
   >>> db.create_all()
   >>> exit()
   ```
5. **Run the application:**
   ```bash
   python app.py
   ```
6. **Access the web app:**
   Open `http://localhost:5000` in your web browser.

## Usage

- Visit the homepage to browse available books.
- Use the **Add Author** and **Add Book** buttons to add new entries.
- Click on a book to view its details.
- Delete a book using the delete button (confirmation required).

## Contributing

Contributions are welcome! Please fork the repository and create a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License.

---

**Happy Reading! 📖**

