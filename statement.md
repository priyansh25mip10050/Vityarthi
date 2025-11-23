# Project Statement: Task Scheduler & Wellness Tracker

## Problem Statement

In the modern environment, individuals often struggle to manage their professional and personal commitments while maintaining mental well-being. Existing tools typically separate task management from wellness tracking, leading to fragmented efforts. This disconnect makes it difficult for users to visualize the relationship between their workload, deadlines, and their corresponding stress levels and mood. The lack of a centralized, simple platform prevents users from proactively adjusting their schedule to prioritize mental health.

## Scope of the Project

The primary scope of this project is to develop a single, lightweight web application that integrates two core functions:

Task Scheduling: Enabling the input, organization, and tracking of tasks based on priority and deadlines.

Wellness Logging: Allowing users to log daily emotional states, stress rates, and the context of their stress.

The application will be built using Python (Flask) and SQLite for simple local deployment.

### **In Scope:**

CRUD operations (Create, Read, Update, Delete) for tasks.

Logging and viewing historical wellness entries.

Basic data persistence using SQLite/Flask-SQLAlchemy.

Viewing tasks sorted by priority.

### **Out of Scope *(Future Enhancements)***:

User authentication/multiple user accounts.

Advanced data visualization (e.g., charts showing stress trends over time).

Notification or reminder systems.

External API integrations.

## Target Users

The application is designed for individuals seeking a straightforward tool to improve personal productivity and self-awareness regarding mental health.

Students: Who need to manage assignments, deadlines, and study stress.

Freelancers & Solopreneurs: Who balance multiple small projects and need to track time and prevent burnout.


## High-Level Features

The high-level features of this application are organized into two primary functional areas:

### **Task Management *(Model: sheduling, Route: /)***

**Task Management:** Users can add a new task, complete with a description, deadline, and a numerical priority level *(Route: /)*.

**Task Review:** Users can view all scheduled tasks, which are automatically ordered by priority *(Route: /sheduling or /progress)*.

**Task Completion:** Users have the functionality to delete a completed task from the progress list *(Route: /delete/<sno>)*.

### **Wellness Tracking *(Model: wellnesstracker, Route: /tracker)***

**Wellness Tracking:** Users can log their mood, stress rate, stress context, and assign a category (type) to the entry *(Route: /tracker)*.

**Wellness History:** Users can view a complete list of all past logged wellness entries to observe personal trends *(Route: /tracker)*.

