Here’s a **step-by-step, real-world Mini Project: To-Do App in Vanilla JavaScript**, designed exactly like a **job-relevant exercise**. This covers **variables, functions, arrays/objects, loops, and conditional logic**.

---

# **Mini Project: To-Do App (Vanilla JS)**

💼 **Why this is important for jobs:**

* Covers core JS concepts: variables, functions, arrays/objects, loops, conditions
* Shows you can **manage dynamic data and UI updates**
* Portfolio-ready project for frontend interviews

---

## **1️⃣ Project Goal**

Build a **simple To-Do App** where a user can:

* Add tasks
* Delete tasks
* Mark tasks as completed
* View tasks dynamically

All **using Vanilla JS, HTML, and CSS**.

---

## **2️⃣ Folder Structure (Simple)**

```
todo-app/
├── index.html
├── style.css
└── script.js
```

---

## **3️⃣ HTML (UI Skeleton)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>To-Do App</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h1>To-Do List</h1>
    <input type="text" id="taskInput" placeholder="Add new task">
    <button id="addBtn">Add Task</button>
    <ul id="taskList"></ul>
  </div>
  <script src="script.js"></script>
</body>
</html>
```

---

## **4️⃣ CSS (Basic Styling)**

```css
body {
  font-family: Arial, sans-serif;
  background: #f4f4f4;
  display: flex;
  justify-content: center;
  padding-top: 50px;
}

.container {
  background: white;
  padding: 20px;
  border-radius: 8px;
  width: 300px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

input, button {
  width: 100%;
  padding: 10px;
  margin: 5px 0;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  padding: 10px;
  background: #e2e2e2;
  margin-bottom: 5px;
  display: flex;
  justify-content: space-between;
  border-radius: 4px;
}

li.completed {
  text-decoration: line-through;
  opacity: 0.6;
}

button.deleteBtn {
  background: red;
  color: white;
  border: none;
  padding: 5px;
  cursor: pointer;
  border-radius: 4px;
}
```

---

## **5️⃣ JavaScript (Logic)**

```javascript
// 1️⃣ Variables
const taskInput = document.getElementById("taskInput");
const addBtn = document.getElementById("addBtn");
const taskList = document.getElementById("taskList");

// 2️⃣ Array to store tasks
let tasks = [];

// 3️⃣ Functions
function renderTasks() {
  taskList.innerHTML = ""; // Clear list
  tasks.forEach((task, index) => {
    const li = document.createElement("li");
    li.textContent = task.text;

    // Mark completed
    if(task.completed) {
      li.classList.add("completed");
    }

    li.addEventListener("click", () => toggleComplete(index));

    // Delete button
    const deleteBtn = document.createElement("button");
    deleteBtn.textContent = "Delete";
    deleteBtn.classList.add("deleteBtn");
    deleteBtn.addEventListener("click", (e) => {
      e.stopPropagation(); // Prevent marking complete
      deleteTask(index);
    });

    li.appendChild(deleteBtn);
    taskList.appendChild(li);
  });
}

function addTask() {
  const taskText = taskInput.value.trim();
  if(taskText === "") {
    alert("Enter a task!");
    return;
  }
  tasks.push({ text: taskText, completed: false });
  taskInput.value = "";
  renderTasks();
}

function toggleComplete(index) {
  tasks[index].completed = !tasks[index].completed;
  renderTasks();
}

function deleteTask(index) {
  tasks.splice(index, 1);
  renderTasks();
}

// 4️⃣ Event Listener
addBtn.addEventListener("click", addTask);

// Optional: add task on Enter key
taskInput.addEventListener("keypress", (e) => {
  if(e.key === "Enter") addTask();
});
```

---

## **6️⃣ Key Concepts Covered (Job-Relevant)**

| Concept                    | Usage in Project                                         |
| -------------------------- | -------------------------------------------------------- |
| Variables (`const`, `let`) | Store DOM elements and task array                        |
| Functions                  | `addTask`, `renderTasks`, `toggleComplete`, `deleteTask` |
| Arrays                     | Store list of tasks dynamically                          |
| Objects                    | Each task is `{text, completed}`                         |
| Loops (`forEach`)          | Render tasks dynamically                                 |
| Conditional (`if`)         | Validate input, mark completed                           |
| Event Listeners            | Handle click & Enter key events                          |
| DOM Manipulation           | Add/remove tasks dynamically                             |

---

## **7️⃣ Enhancements (Portfolio/Job-Level)**

* Save tasks in **localStorage** to persist after reload
* Add **due dates** and **priority levels**
* Filter tasks: All / Completed / Pending
* Add **dark mode toggle**
* Use **React** to convert into a modern frontend project

---

## **8️⃣ Summary**

* Simple, clean, **full JS logic project**
* Covers **all basic JS concepts**: variables, functions, arrays/objects, loops, conditionals
* Fully dynamic and interactive
* Ready for portfolio or coding interview demonstration

---

If you want, I can **upgrade this To-Do app into a React version next**, including **state management, reusable components, and conditional rendering**, which is **exactly like a job-level project**.

Do you want me to do that?
