# Reading List App

A simple Laravel application for keeping track of books I want to read, am currently reading, or have finished. Users can add, edit, delete, and filter books by status.

## Requirements

- PHP
- Composer
- Laravel
- SQLite

## Installation

1. Clone the repository.
2. Install dependencies:

   ```bash
   composer install
   ```

3. Create the environment file if needed:

   ```bash
   cp .env.example .env
   ```

   On Windows PowerShell, use `Copy-Item .env.example .env` instead if the file does not exist.

4. Generate the application key:

   ```bash
   php artisan key:generate
   ```

5. Configure SQLite in `.env`:

   ```text
   DB_CONNECTION=sqlite
   ```

6. Create `database/database.sqlite` if it does not exist.
7. Run database migrations:

   ```bash
   php artisan migrate
   ```

8. Start the application:

   ```bash
   php artisan serve
   ```

9. Open http://127.0.0.1:8000/books in your browser.

## Features

- Display all books
- Add books with validation
- Edit existing books
- Delete books after confirmation
- Filter books by status

## AI Usage

I used ChatGPT to understand the Laravel setup, resource routes, database migration, form validation, and CRUD implementation. I reviewed and tested the code while building the application step by step.