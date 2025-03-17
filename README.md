
# **Tea API ☕**  

A simple **CRUD API** for managing tea records, built using **Node.js and Express.js**.  

---

## **Features 🚀**  
✅ Add, view, update, and delete tea records  
✅ Uses **Express.js** for routing  
✅ Middleware for JSON parsing  
✅ Error handling and validation  
✅ Integrated logging for request tracking and debugging  
✅ Future-ready for database integration  

---

## **Getting Started 🛠**  

### **1️⃣ Prerequisites**  
Ensure you have the following installed:  
- [Node.js](https://nodejs.org/)  
- [npm](https://www.npmjs.com/) 

### **2️⃣ Installation**  
Clone the repository and install dependencies:  
```bash
git clone https://github.com/AnantSingla412/express.git  
cd express  
npm install  
```

### **3️⃣ Running the Server**  
Start the server using:  
```bash
npm start  # Runs the server on default port 3000  
```
For development mode with auto-restart:  
```bash
npm run dev  # Uses nodemon  
```

---

## **API Endpoints 🔗**  

| Method | Endpoint | Description |  
|--------|----------|------------|  
| **POST** | `/teas` | Add a new tea |  
| **GET** | `/teas` | Get all teas |  
| **GET** | `/teas/:id` | Get a tea by ID |  
| **PUT** | `/teas/:id` | Update a tea |  
| **DELETE** | `/teas/:id` | Delete a tea |  

📌 **Request & Response Example:**  

**POST /teas**  
_Request:_  
```json
{
  "name": "Green Tea",
  "price": 20
}
```
_Response:_  
```json
{
  "id": 1,
  "name": "Green Tea",
  "price": 20
}
```

---

## **Logging & Debugging 📝**  

This API includes logging to track incoming requests and errors. Logging helps in debugging, monitoring, and improving performance.  

### **1️⃣ Request Logging with Morgan**  
[**Morgan**](https://www.npmjs.com/package/morgan) is used to log HTTP requests. It captures request details like method, URL, status code, response time, and more.  

Example log format:  
```bash
GET /teas 200 10ms
POST /teas 201 15ms
PUT /teas/1 404 5ms
```

### **2️⃣ Application Logging with Winston**  
[**Winston**](https://www.npmjs.com/package/winston) is used for structured logging and error tracking. It allows:  
✅ Logging at different levels (`info`, `warn`, `error`, etc.)  
✅ Storing logs in a file for debugging  
✅ Custom log formatting  

Example log output:  
```bash
[INFO] Server started on port 3000
[ERROR] Tea not found (ID: 5)
```

To enable logging, install the required packages:  
```bash
npm install morgan winston
```

---

## **Improvements & Future Enhancements 🔮**  

- ✅ Add a database (MongoDB, PostgreSQL, etc.)  
- ✅ Implement authentication for API security  
- ✅ Improve request validation & error handling  
- ✅ Enhance logging with structured logs & persistent storage  

---

## **Author ✍️**  
**Anant** - Learning backend development and building APIs with **Node.js & Express.js**.  

---
