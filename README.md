# Task Board - Execution Tracking with Comments & Guidelines

A simple **task board** (calendar-based) web application that supports:  
- Adding tasks (with sub-tasks/mini-cubes).  
- Adding colored comments on specific days.  
- Multi-day task assignment.  
- Manual **save/load** data to/from a local JSON file.  
- Adding general guidelines that appear in a side panel.

**Table of Contents**  
1. [Overview](#overview)  
2. [Features](#features)  
3. [Installation & Setup](#installation--setup)  
4. [Usage](#usage)  
5. [Data Management](#data-management)  
6. [Contributing](#contributing)  
7. [License](#license)

---

## Overview

This project provides a **calendar-based** task manager, allowing you to add tasks per day and track sub-task completion visually. Users can also add notes (comments) on any day, choose the note color, and store or retrieve everything from a **local JSON file**. Additionally, you can specify multi-day tasks that span a date range, and simple **guidelines** can be maintained on the right panel.

---

## Features

1. **Calendar View**  
   - Dynamically shows each day of the current month, including “blank” cells for days before the 1st.  

2. **Sub-Task Completion**  
   - Each task has a set of **mini-cubes** representing its sub-tasks. Click a cube to fill/unfill, changing the “completed” count.

3. **Colored Comments**  
   - Add short, colored text comments to a specific day. Choose the color and text on the fly.

4. **Multi-Day Task Creation**  
   - Specify a start and end date plus number of sub-tasks, and the application populates each date in that range with the new task.

5. **Manual Save/Load**  
   - Save the entire application state (tasks, comments, guidelines) to a single JSON file.  
   - Load from a file to restore or merge data.  

6. **General Guidelines**  
   - Keep a list of freeform guidelines (text-based notes) on the right-hand side.  
   - Supports adding/removing guidelines, which are numbered automatically.

---

## Installation & Setup

1. **Clone or Download**  
   - Clone this repository (or download the ZIP) to your local machine.  

2. **Open in Browser**  
   - Simply open the `index.html` file in your favorite browser.  
   - No server or build step required (purely client-side JavaScript).

3. **Optional: Local server**  
   - If your browser blocks local file interactions, you can run a simple local server (e.g., `python -m http.server` in Python).  
   - Then visit `http://localhost:8000` (or whichever port) to use the app.

---

## Usage

1. **Navigate Months**  
   - Click **“Previous Month”** or **“Next Month”** to change the displayed month.

2. **Add Single Task**  
   - Hover over a specific day cell.  
   - Click **“Add Task”** → fill out the inline form (task name & sub-task count).  
   - Press **“Add”** to confirm.

3. **Add Multi-Day Task**  
   - In the top multi-day form, type the **Task Name**, choose **# Sub-tasks**, **Start Date**, and **End Date**.  
   - Press **“Add to Days”** to populate every date in that range with the new task.

4. **Mark Sub-Tasks**  
   - In any day’s tasks, click a **mini-cube** to fill/unfill and change the “completed” count.

5. **Add Comments**  
   - Hover over a day cell, click **“Add Comment.”**  
   - Type your comment, pick a color, and press **“Add.”**

6. **Save / Load Data**  
   - **“Save Data”** → Exports the entire state as a `myCalendarData.json` file.  
   - **“Load Data”** → Opens a file dialog to import an existing JSON file.  
   - Upon loading, your tasks/comments/guidelines appear instantly.

7. **General Guidelines**  
   - In the **Guidelines** panel, type your guideline text and press **“Add Guideline.”**  
   - Each guideline is shown in a small list, with a **“Delete”** button on hover.

---

## Data Management

- **Local Storage**  
  - Internally, the application state is automatically saved to the browser’s `localStorage` after every change (tasks, comments, guidelines).  
  - This allows your data to persist **between sessions** (unless you clear your browser data).

- **Manual Save/Load**  
  - If you want to **transfer** your data to another browser or **back it up** offline, use the **“Save Data”** button to download a JSON file.  
  - Then on another machine or browser, press **“Load Data”** to restore it.

---

## Contributing

1. **Fork** this repository on GitHub.  
2. **Create a feature branch**: `git checkout -b feature/my-new-feature`.  
3. **Commit** your changes: `git commit -am 'Add my feature'`.  
4. **Push** to the branch: `git push origin feature/my-new-feature`.  
5. Open a **Pull Request** in this repository describing the changes.

---

## License

> Licensed under the [Apache-2.0 license](LICENSE).  
>  
> **© 2024 Smitrani310@gmail.com. All rights reserved.**

---

**Enjoy your new Task Board and keep track of your tasks, sub-tasks, and guidelines with ease!**
