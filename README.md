# P2SubmissionBackend
The Online Auction System Backend uses Node.js, Express.js, and MongoDB for user authentication, auction management, and bidding. Users can sign up, log in, create, edit, delete auctions, and place bids. It ensures secure passwords and auto-closes expired auctions. Run with node server.js. Future update: real-time bidding with WebSockets.


Online Auction System - Backend (MERN Stack)
This is the backend for an Online Auction System, built using Node.js, Express.js, and MongoDB. It provides secure user authentication, auction management, and bidding functionality.

🚀 Features
✔️ User Authentication (Signup & Signin with encrypted passwords)
✔️ Create, Edit, Delete Auctions
✔️ Place Bids (Only if higher than the current bid & auction is active)
✔️ Fetch All or Single Auction Details
✔️ Auction Expiry Handling (Marks auctions as closed when time is up)

📌 API Endpoints
🔐 Authentication
POST /signup → Register a user (password stored securely)
POST /signin → Login user (verifies credentials)
🛒 Auction Management
POST /auction → Create a new auction
GET /auctions → Get all auctions
GET /auctions/:id → Get a specific auction
PUT /auction/:id → Edit an auction
DELETE /auction/:id → Delete an auction
💰 Bidding
POST /bid/:id → Place a bid on an auction
🛠️ Setup & Run
1️⃣ Install dependencies:

sh
Copy
Edit
npm install
2️⃣ Start MongoDB locally:

sh
Copy
Edit
mongod --dbpath "C:\data\db"
3️⃣ Run the server:

sh
Copy
Edit
node server.js
OR with nodemon:

sh
Copy
Edit
nodemon server.js
🛠️ Tech Stack
🔹 Node.js - Server-side runtime
🔹 Express.js - Web framework
🔹 MongoDB & Mongoose - Database & ODM
🔹 bcrypt.js - Password encryption
🔹 CORS & body-parser - Middleware

📌 Future Enhancements: Implement WebSockets (Socket.io) for real-time bidding! 🚀
