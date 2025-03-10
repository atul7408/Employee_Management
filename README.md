Employee Management System 🚀
Overview
The Employee Management System is a web application built with Angular and JSON Server for managing employee details. It provides features such as employee listing, editing, and viewing employee details in a dialog popup.

Features ✨
✅ View all employees in a table format
✅ Edit employee details in a popup dialog
✅ Tooltip on employee First Name for better UX
✅ Fetch employee data from a JSON Server
✅ Responsive Angular Material UI

Tech Stack 🛠️
Frontend: Angular (Standalone Components), Angular Material
Backend: JSON Server (Mock API)
Styling: Angular Material, CSS
Data Handling: HttpClient (REST API Calls)

Installation & Setup 🚀
1️⃣ Clone the Repository
sh
Copy
Edit
git clone https://github.com/atul7408/Employee_Management.git
cd Employee_Management
2️⃣ Install Dependencies
sh
Copy
Edit
npm install

3️⃣ Run JSON Server (Mock API)
sh
Copy
Edit
json-server --watch db.json --port 3000

4️⃣ Run Angular Application
sh
Copy
Edit
ng serve
🔹 Open your browser and go to http://localhost:4200/

Project Structure 📂
pgsql
Copy
Edit
Employee_Management/
│── src/
│   ├── app/
│   │   ├── employee-list/
│   │   ├── employee-detail-dialog/
│   │   ├── layout/
│   │   ├── services/ (Employee API service)
│   ├── assets/
│   ├── environments/
│── db.json (Mock JSON database)
│── package.json
│── angular.json
│── README.md


Contributing 🤝
🔹 Fork the repo
🔹 Create a feature branch (git checkout -b feature-branch)
🔹 Commit changes (git commit -m "Added new feature")
🔹 Push to branch (git push origin feature-branch)
🔹 Create a Pull Request

License 📝
This project is licensed under the MIT License.

Author 👨‍💻
Developed by Atul Verma

📧 Contact: atul7408@gmail.com
🔗 GitHub: @atul7408


Conclusion
The Employee Management System effectively showcases fundamental Angular concepts, including routing, reactive forms, service-based data handling, and UI design using Angular Material. The project fulfills the XEBO.Ai assignment requirements while maintaining a scalable and modular structure. Additionally, it is designed to be easily extended and integrated with a real backend for future enhancements.

--This is assignment of XEBO.AI 
Let me know if you need modifications! 🚀

