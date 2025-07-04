# To-Do Java Console Application

A **console-based Java To-Do List application** that allows you to create, update, search, delete, and display tasks.  
It uses Java object serialization (`tasks.dat`) to persist your data between runs.

---

## Features

✅ Add new tasks with name, description, and completion deadline  
✅ Update task name, description, deadline, or status  
✅ Soft-delete tasks (keeps in data file, marked as `Deleted`)  
✅ Search tasks by name  
✅ Print all tasks in a formatted table

---

## 📂 Project Structure
Java-todoapplication/
├─ src/
│ └─ com/
│ └─ backend/
│ └─ todo/
│ ├─ dto/
│ ├─ repo/
│ ├─ utils/
│ └─ view/
├─ src/files/tasks.dat # created at runtime
├─ messages.properties
└─ out/ # generated compiled classes

---

## ⚙️ Requirements

- Java 11 or later (tested on Java 21)
- Works on Windows, macOS, Linux (adjust classpath separator `;` vs `:`)

---
## Installation
Follow these steps to download the project on your local machine:

1. **Clone the Repository**
   
   git clone https://github.com/Jai-Anand-JA/To-Do-Application
3. **Navigate to the Project Directory**
   
   cd To-Do-Application

---

## How to Compile & Run

From inside the project root (where `src` folder exists):

### 1️. Compile
javac -d out -sourcepath src src/com/backend/todo/view/ToDoView.java

### 2️. Run  
java -cp "out;src" com.backend.todo.view.ToDoView

---

## 💾 Data Storage
All tasks are serialized to a binary file:  

src/files/tasks.dat

---

## Sample Usage
1. Add a New Task
2. Delete Task
3. Update Task
4. Search a Task
5. Print All Tasks
6. Exit from Application 
Enter your choice:

---

## Notes
- Dates are entered in the format: dd/MM/yyyy HH:mm (e.g. 08/07/2025 14:00).
- Deleted tasks are retained with status Deleted for audit.
- Application handles missing dates gracefully by printing N/A.

---

## Author
- Jai Anand
