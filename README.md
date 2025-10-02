📚 MongoDB Bookstore Project

This project demonstrates how to build and interact with a MongoDB database using Node.js and the MongoDB Driver.
It includes two main scripts:

insert_books.js → Seeds the database with sample book data.

queries.js → Performs queries, updates, deletions, aggregations, and indexing on the data.


🚀 Features

Database Seeding (insert_books.js)

Connects to MongoDB

Drops existing books collection (if it exists)

Inserts a set of sample books

Logs inserted documents

Queries & Operations (queries.js)

CRUD Operations

Find books by genre

Find books published after a year

Find books by a specific author

Update book price

Delete a book

Advanced Queries

Find in-stock books published after 2010

Projection (only title, author, price)

Sorting (ascending & descending by price)

Pagination (page 2, 5 books per page)

Aggregation Pipelines

Average price by genre

Author with the most books

Group books by decade

Indexes

Create index on title

Create compound index on author + published_year

Query performance analysis with explain()


📂 Project Structure
📦 mongodb-bookstore
 ┣ 📜 insert_books.js   # Script to seed MongoDB with sample data
 ┣ 📜 queries.js        # Script to run queries & aggregations
 ┣ 📜 README.md         # Project documentation


🛠️ Prerequisites

Install Node.js

Install MongoDB Community Edition
 or use MongoDB Atlas

Start your local MongoDB server (default: mongodb://localhost:27017)


📥 Installation
# Clone the repository
git clone <your-repo-url>

# Navigate to the project
cd mongodb-bookstore

# Install dependencies
npm install mongodb

▶️ Usage
1. Seed the Database

Run the insert_books.js script to populate the plp_bookstore database:

node insert_books.js


✅ This will insert sample books into the books collection.

2. Run Queries

Execute the queries.js script to test different MongoDB operations:

node queries.js


✅ You’ll see console output for each task: CRUD, advanced queries, aggregation, and indexes.

📊 Example Console Output
Connected to MongoDB server
12 books were successfully inserted into the database

 Fiction Books: [ ... ]
 Books published after 1950: [ ... ]
 Updated Hobbit price: Success
 Deleted Moby Dick: Success
 Average price by genre: [ ... ]
 Author with the most books: [ ... ]
 Books grouped by decade: [ ... ]
 Index created on 'title'
 Compound index created on 'author' and 'published_year'
