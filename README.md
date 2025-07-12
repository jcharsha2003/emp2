# 👨‍💼 Employee Management System

**Live App**: [emp.com](#)  
**GitHub Repo**: [GitHub Link](#)

> A robust and scalable Employee Management System built using the **MERN Stack**, fully containerized with **Docker** and deployed to a custom domain via **DuckDNS**. This platform ensures secure authentication, centralized employee records, and streamlined task tracking — perfect for modern businesses and HR workflows.

---

## 🧠 Overview

The **Employee Management System** enables companies to efficiently handle employee data, task assignments, user roles, and login access. It provides full CRUD operations, real-time data access, and secure APIs, making it ideal for HR teams and administrators.

---

## 🛠️ Technologies Used

| Category           | Stack / Tools                                  |
|--------------------|-------------------------------------------------|
| 🎨 Frontend         | React.js, HTML, CSS, JavaScript                 |
| 🗃️ State Mgmt (Opt.) | Redux                                           |
| 🧠 Backend          | Node.js, Express.js                             |
| 🧾 Database         | MongoDB (with Mongoose ODM)                     |
| 🔐 Auth             | JWT (JSON Web Tokens)                           |
| 📦 Containerization | Docker, Docker Compose                          |
| 🌐 Domain Mgmt      | DuckDNS                                         |
| ☁️ Deployment       | Cloud Server (AWS or equivalent)               |
| 🔁 Version Control  | Git, GitHub                                     |

---

## 📁 Folder Structure

```
employee-management/
│
├── client/               # React frontend
│   └── .env              # Contains REACT_APP_API_URL
│
├── server/               # Express backend
│   └── .env              # MongoDB credentials via variables
│       MONGO_USERNAME
│       MONGO_PASSWORD
│       MONGO_DBNAME
│       MONGO_CLUSTER
│
├── Dockerfile            # Image build file
├── docker-compose.yaml   # Docker service configuration
├── README.md             # Project documentation
```

---

## 🔐 Default Admin Login (Database)

- **Username**: `chandu`  
- **Password**: `chandu`

> ⚠️ Please change credentials in production for security.

---

## 🚀 How to Launch the Application

### ✅ With Docker (Recommended)

> Make sure Docker Desktop or Docker Daemon is running on your system.

### Step-by-Step Docker Deployment

1. **Clone the Repository**
   ```bash
   git clone <repository-link>
   cd employee-management
   ```

2. **Build the Docker Image**
   ```bash
   docker-compose build
   ```

3. **Run the Application**
   ```bash
   docker-compose down     # Optional cleanup if previously run
   docker-compose up
   ```

4. **Access the Application**
   - Client App: [http://localhost:3000](http://localhost:3000)
   - Server/API: [http://localhost:5000](http://localhost:5000) *(or as per docker-compose config)*

5. **Stop the Container**
   ```bash
   Ctrl + C
   ```

6. **Remove Containers (optional)**
   ```bash
   docker-compose down
   ```

---

### 🚀 Without Docker

1. **Client Setup**
   ```bash
   cd client
   npm install
   ```

2. **Server Setup**
   ```bash
   cd server
   npm install
   ```

3. **Run Both**
   - **Client**
     ```bash
     npm start
     ```
   - **Server (use app.js as entry)**
     ```bash
     nodemon app.js
     ```

> 💡 For best results, run both in split terminals or two separate terminal tabs.

---

## 📦 Environment Variables

> Place `.env` files in their respective folders.

### client/.env
```env
REACT_APP_API_URL=http://localhost:5000
```

### server/.env
```env
MONGO_USERNAME=myusername
MONGO_PASSWORD=mypassword
MONGO_DBNAME=mydatabase
MONGO_CLUSTER=mycluster
```

> 🔒 Keep this information private when pushing to GitHub!

---

## 📅 Project Timeline

- **Start**: April 2024  
- **End**: June 2024  
- **Status**: ✅ Deployed and Functional  
- **Hosted on**: AWS Cloud using Docker Containers

---

## 🌟 Core Features

- 👤 User Authentication (JWT)
- 📄 Employee CRUD Operations
- 🧑‍💼 Role-based Access Control
- 📋 Task Assignments
- 🌐 Fully Containerized with Docker
- 📈 Performance-optimized API
- 🌍 Deployed with DuckDNS custom domain

---

## 🔮 Future Improvements

- 📊 Admin Analytics Dashboard  
- 📨 Email Notification Integration  
- 🧾 PDF Export for Employee Records  
- 🧑‍🏫 Training Module Assignment  

---

## 🙌 Final Note

The **Employee Management System** brings together seamless UI, secure APIs, and containerized deployment — providing businesses a reliable digital HR solution. Easy to set up, easier to scale.

> 👨‍💻 *Empowering your workforce with technology.*

---

**🧑‍💻 Developed by**: [Your Name]  
**🌐 Website**: [emp.com](#)  
**📚 License**: MIT (optional)  
**📬 Contact**: [your-email@example.com]
