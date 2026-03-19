Skill-10: React State Management using useState Object
=======================================================

Student   : Y. AdithyaCharan
ID        : 2400080194
Section   : 01
GitHub    : https://github.com/Adithya-charan/FullStack-Skill-10

--------------------------------------------------
AIM
--------------------------------------------------
To build a React StudentManager component using the
useState hook to manage an array of student objects.

Users can:
  - Add new students using input fields
  - View the full student list in a table
  - Delete any student instantly
  - UI updates automatically without page refresh

--------------------------------------------------
WHAT IS THIS PROJECT?
--------------------------------------------------
This project is a React web application that manages
a list of students using React Hooks (useState).

Instead of reloading the page every time data changes,
React automatically re-renders the UI whenever the
state (students list) is updated.

Example:
  When you click "+ Add Student", the new student
  is added to the array and the table updates instantly.

  When you click "Delete", that student is removed
  from the array and disappears from the table instantly.

--------------------------------------------------
KEY CONCEPTS USED
--------------------------------------------------
useState Hook
  - Used to store and update data inside a component
  - When state changes, React re-renders the UI

Spread Operator (...)
  - Used to add new student to existing array
  - setStudents([...students, newStudent])

Array.filter()
  - Used to delete a student by ID
  - students.filter(s => s.id !== id)

onChange Handler
  - Updates newStudent fields as user types in inputs
  - Uses computed property [e.target.name] for dynamic update

--------------------------------------------------
STATE VARIABLES
--------------------------------------------------
State Variable   Type             Purpose
--------------   ---------------  --------------------------------
students         Array of Objects Stores all student records
newStudent       Object           Holds current input field values

Setter Function  Purpose
---------------  ----------------------------------------
setStudents()    Updates list - triggers UI re-render
setNewStudent()  Clears input fields after adding student

--------------------------------------------------
PROJECT FILES
--------------------------------------------------
FullStack-Skill-10/
  src/
    StudentManager.jsx    - Main component with all logic
    StudentManager.css    - Styling for table, inputs, buttons
    App.jsx               - Root component that loads StudentManager
  package.json            - Project config and dependencies
  README.md               - Project documentation

--------------------------------------------------
TECH STACK
--------------------------------------------------
Technology   Version   Purpose
-----------  --------  ----------------------------
React        18.2.0    Frontend UI library
useState     Hook      State management
CSS          -         Styling and layout
Node.js      16+       Runtime environment
npm          -         Package manager

--------------------------------------------------
HOW TO RUN
--------------------------------------------------
Step 1 - Create React App (first time only)
  npx create-react-app student-manager
  cd student-manager

Step 2 - Replace these files in src/ folder
  - Replace App.jsx with the given App.jsx
  - Copy StudentManager.jsx into src/
  - Copy StudentManager.css into src/

Step 3 - Start the app
  npm start

Step 4 - Open browser
  http://localhost:3000

--------------------------------------------------
EXPECTED OUTPUT
--------------------------------------------------
When app loads, you will see a table like this:

  +----+---------+-----------------+--------+
  | ID | Name    | Course          | Action |
  +----+---------+-----------------+--------+
  | 1  | Adithya | Full Stack Dev  | Delete |
  | 2  | Ravi    | Java Backend    | Delete |
  | 3  | Priya   | UI/UX Design    | Delete |
  | 4  | Kiran   | Cloud Computing | Delete |
  | 5  | Sneha   | Data Science    | Delete |
  +----+---------+-----------------+--------+

Add Student:
  - Enter ID, Name, Course in the input boxes
  - Click "+ Add Student"
  - New row appears at the bottom of the table

Delete Student:
  - Click "Delete" button on any row
  - That row disappears instantly

Empty List:
  - If all students are deleted, shows:
    "No students available"

--------------------------------------------------
TASKS COMPLETED
--------------------------------------------------
Task 1  - Created StudentManager React component
Task 2  - Added 5 initial student objects
Task 3  - Used useState for students array and newStudent
Task 4  - Created input boxes with onChange handler
Task 5  - Add Student button with spread operator
Task 6  - Displayed student list using map()
Task 7  - Delete button using Array.filter()
Task 8  - Empty message when list is empty
Task 9  - Added CSS styling for table and buttons
Task 10 - Pushed project to GitHub

--------------------------------------------------
GIT COMMANDS TO PUSH TO GITHUB
--------------------------------------------------
Step 1 - Go into the project folder
  cd C:\Users\HP\student-manager

Step 2 - Initialize git
  git init

Step 3 - Stage all files
  git add .

Step 4 - Commit with message
  git commit -m "Skill10: React useState StudentManager"

Step 5 - Add remote origin
  git remote add origin https://Adithya-charan@github.com/Adithya-charan/FullStack-Skill-10.git

Step 6 - Rename branch to main
  git branch -M main

Step 7 - Push to GitHub
  git push -u origin main --force

Note: When asked for password, enter your
      Personal Access Token (not GitHub password)

--------------------------------------------------
