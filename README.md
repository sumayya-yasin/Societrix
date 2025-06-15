Societrix – University Society & Event Management Platform
Societrix is an all-in-one digital solution designed for universities and institutions to streamline the management of student societies, event coordination, budget approvals, and internal communication between student organizations and administrative staff.
________________________________________
🔐 Login Workflow
On the Login Page, users are prompted to select their role:
•	Administrator
•	Society Member
🔸 Administrator Login
(Admin credentials are pre-seeded in the database)
•	Email: admin@societrix.com
•	Password: admin123
🔸 Society Login
•	Societies are added by the admin.
•	On their first login, users are required to change their password.
•	Upon successful login, they're redirected to their Society Dashboard.
________________________________________
🛠️Admin Dashboard Features
Top Bar
•	Dark/Light Theme Toggle 🌙/☀️
•	Notifications Center
•	Profile Dropdown: View Profile | Logout
Overview Dashboard
•	Total Registered Societies
•	Upcoming Events
•	Event Count
•	Recent Activity
•	Active Societies Overview
Add a New Society
•	Form-based interface to register a new society.
•	Automatically generates unique login credentials for new entries.
📥 Event Request Management
•	Displays Available Budget
•	Fund Management form for allocations
•	Review incoming event proposals:
o	Approve/Reject requests with optional feedback
o	Approvals dynamically adjust available funds
o	Sponsorships credited to fund pool
🗓️ Event Calendar
•	Visual schedule of all planned events
•	Toggle views: Day, Week, or Month
•	Cancel or remove approved events directly
🧾 Society Directory
•	View all societies registered in the system
•	Access detailed information or remove entries
📑 Event Reports & Ratings
•	View detailed reports post-events
•	Admins can rate society performance
•	Rankings visible on a sidebar leaderboard
💬 Messaging Hub
•	Announcements broadcasted to all societies
•	1-on-1 messaging with individual societies
•	Fully integrated internal messaging system
________________________________________
👥 Society Panel Features
🔝 Top Bar
•	Light/Dark Theme Switch 🌙/☀️
•	Notifications Panel
•	Profile Access: View/Edit | Logout
📊 Society Dashboard
•	Total Societies in the system
•	List of Upcoming Events
•	Events Organized
•	Recent Society Activities
•	Active Societies Summary
🧑‍💼 Society Profile Management
•	Update society profile and information
•	Add or edit description and member list
📑 Submit Event Reports
•	Upload and manage reports for past events
📝 Event Proposals
•	View calendar of upcoming events
•	Click "Request New Event" to open submission form:
o	Fill in event details
o	Upload documents
o	Add sponsorship information if applicable
💬 Communication Tools
•	Participate in general announcement chat
•	Direct messaging with Admin
•	Inter-society private chat feature
⚙️ Settings
•	Access and update profile settings
________________________________________
🚀 Project Setup Guide
1. Clone the Repository
git clone https://github.com/zaynah024/Societrix.git
cd Societrix
2. Configure Environment Variables
Create a .env file inside the server/ directory with the following content:
MONGO_URI=mongodb://localhost:27017/Societrix
PORT=5000
JWT_SECRET=nhiHoRahaAbMereSe
NODE_ENV=development
________________________________________
▶️ Running the Application
🔧 Backend (Server)
cd server
node index.mjs
🌐 Frontend (Client)
cd client
npm install
npm run dev

