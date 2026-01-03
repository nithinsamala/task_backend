# task_backend
A MERN stack task management app that helps users organize tasks with priorities, due dates, status tracking, and filtering using REST APIs and MongoDB.

step 1 Clone the Repository from GitHub
git clone https://github.com/nithinsamala/task_backend.git 
{This will download the entire backend folder to your system.}

step 2:Go Inside the Project Folder
cd task_backend
Check files by : ls
You should see:
server.js
package.json
package-lock.json
README.md

step 3: Install Dependencies
Run:
npm install

This will create:
node_modules/

step 4. Create .env File
Inside the project root, create a file:
.env
Add this 2 inside .env:
PORT=5000
MONGODB_URI=mongodb://127.0.0.1:27017/taskmanager

step 6. Run the Backend Server
 nodemon server.js

step 7. Verify Backend is Working

Open browser and visit:
http://localhost:5000/api/tasks
✔ You should see:
[]
(or list of tasks)

step 8. Test with Postman / Browser
Create Task (POST)
http://localhost:5000/api/tasks

Body:
{
  "title": "Test Task",
  "description": "Testing locally",
  "priority": "medium",
  "dueDate": "2026-01-05",
  "completed": false
}

