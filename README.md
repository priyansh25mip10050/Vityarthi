# 📅 Task Scheduler & Wellness Tracker

## 📝 Overview of the Project

A lightweight web application built with Python's Flask framework designed to provide users with a dual-purpose tool: managing tasks and monitoring mental wellness. It uses a simple SQLite database for persistence, making it easy to run locally.
## ✨ Features

This application combines task management and mental wellness tracking into a single, cohesive platform.

**Task Scheduling:** Add new tasks with details, deadlines, and numerical priority levels.

**Priority Listing:** Tasks are displayed on the scheduling and progress pages, ordered by their priority level.

**Progress Tracking:** Ability to view all tasks and delete them upon completion.

**Mood Logging:** Record daily mood, stress rate, and detailed descriptions.

**Categorization:** Tag wellness entries with a TYPE (e.g., Personal, Work, Health) for analysis.

**History:** View all past wellness entries on the tracker page.

## 💻 Technologies/Tools Used

**Backend Framework:** Flask (Python)

**Database:** SQLite (*Managed via SQLAlchemy*)

**ORM:** Flask-SQLAlchemy

**Templating:** HTML templates (index.html, sheduling.html, progress.html, Wellness.html).

## ⚙️ Steps to Install & Run the Project

Follow these steps to get the application running on your local machine.

Prerequisites

Python 3.8+

### 1. Clone the Repository

git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name


### 2. Create and Activate a Virtual Environment

**Create environment**
python -m venv venv

**Activate on macOS/Linux**
source venv/bin/activate

**Activate on Windows (Command Prompt)**
venv\Scripts\activate


### 3. Install Dependencies

pip install Flask Flask-SQLAlchemy


### 4. Run the Application

The database (task.db) and tables will be created automatically on the first run.

python app.py

## 🧪 Instructions for Testing

Since this is a Flask application, testing is primarily manual through the web interface.

### 1. Task Scheduling Tests

Create Task: Navigate to */* and submit a task with Priority 1 (high) and another with Priority 5 (low).

Verify Sorting: Navigate to */sheduling* or */progress* and confirm that the Priority 1 task appears before the Priority 5 task.

Delete Task: On the */progress page*, click the delete link for a task and ensure the task is immediately removed from the list and the database.

### 2. Wellness Tracker Tests

Create Entry: Navigate to */tracker* and submit a new wellness entry, ensuring all required fields (Mood, Stress Rate, Stress context, Type) are filled.

Verify History: Check the list of entries below the submission form on the */tracker* page to confirm the new entry was successfully added and displayed.
The application should now be accessible at: http://127.0.0.1:5000/
