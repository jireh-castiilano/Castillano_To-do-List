# Jireh Todolist

Jireh Todolist is a calm and simple task management application for organizing daily responsibilities. It helps users create, update, complete, categorize, and track tasks in a clean workspace.

## Purpose

I created this project to provide a useful and practical to-do list for my classmates. I also built it to gain hands-on experience in web development, learn how frontend and backend technologies work together, and improve my skills through a complete, real-world project.

## Features

- Add, edit, and delete tasks
- Mark tasks as completed
- Add due dates and reminders
- Organize tasks by Today, Upcoming, Missed, Calendar, and Completed views
- Add notes and color categories to tasks
- Filter tasks by category or search for a task
- Choose between several workspace themes
- Use browser notifications for due-task reminders
- Store tasks locally when cloud services are unavailable
- Synchronize tasks with Supabase for authenticated users

## Built With

- Svelte 5
- Vite
- JavaScript
- Supabase
- CSS

## Getting Started

### Prerequisites

- Node.js 18 or newer
- npm
- A Supabase project, if cloud synchronization is enabled

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/jireh-castiilano/Castillano_To-do-List.git
   cd Castillano_To-do-List
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the project root using `.env.example`:

   ```env
   VITE_SUPABASE_URL=your-supabase-project-url
   VITE_SUPABASE_ANON_KEY=your-supabase-anon-key
   ```

   Supabase variables are optional. Without them, the application stores tasks in browser local storage.

### Supabase Setup

1. Create a Supabase project.
2. Open the SQL Editor.
3. Run the SQL statements in `supabase/schema.sql`.
4. Add your Supabase project URL and anonymous key to `.env`.

The schema creates the tasks table, database indexes, and row-level security policies that allow users to access only their own tasks.

### Run the Application

```bash
npm run dev
```

Open the local address shown in the terminal, usually `http://localhost:5173`.

### Build for Production

```bash
npm run build
```

The generated production files are placed in the `dist` directory.

## Project Structure

```text
src/
  lib/
    supabase.js
  App.svelte
  app.css
  main.js
supabase/
  schema.sql
```

## Author

Ken (Fushitowa)
