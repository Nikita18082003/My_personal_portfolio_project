# My_personal_portfolio_project
Task of web development internship given by TechnoHacks

📝 Simple To-Do List Application

📌 Overview

This is a basic To-Do List application built using HTML, CSS, and JavaScript. It allows users to add tasks, remove tasks, and mark tasks as completed, providing a simple and interactive way to manage daily tasks.

🎯 Features

✅ Add new tasks

✅ Remove tasks

✅ Mark tasks as completed

✅ Interactive UI with a clean and responsive design

🛠️ Tech Stack

Frontend: HTML, CSS, JavaScript



🚀 Getting Started

🔹 Clone the Repository

git clone https://github.com/your-username/My_personal_portfolio_project.git

cd My_personal_portfolio_project

🖥️ Code Implementation

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To-Do List</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 400px;
            margin: 50px auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        input {
            width: 70%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 10px;
            border: none;
            background: #28a745;
            color: white;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background: #218838;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            background: #fff;
            margin: 10px 0;
            padding: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }
        .completed {
            text-decoration: line-through;
            color: gray;
        }
        .delete {
            background: red;
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>To-Do List</h1>
        <input type="text" id="taskInput" placeholder="Enter a task...">
        <button onclick="addTask()">Add Task</button>
        <ul id="taskList"></ul>
    </div>
    <script>
        function addTask() {
            let taskInput = document.getElementById("taskInput");
            let taskText = taskInput.value.trim();
            if (taskText === "") return;

            let li = document.createElement("li");
            li.innerHTML = `<span onclick="toggleTask(this)">${taskText}</span> <button class='delete' onclick='removeTask(this)'>Delete</button>`;
            document.getElementById("taskList").appendChild(li);
            taskInput.value = "";
        }
        
        function toggleTask(task) {
            task.classList.toggle("completed");
        }
        
        function removeTask(button) {
            button.parentElement.remove();
        }
    </script>
</body>
</html>


📢 Connect with Me

🔗 GitHub: https://github.com/Nikita18082003

🔗 LinkedIn: www.linkedin.com/in/nikita-borkar-790277270 










