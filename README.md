# Tea API

This is a simple **Tea API** built using **Node.js** and **Express.js**. It allows users to **perform CRUD operations** on a list of teas, including adding, retrieving, updating, and deleting tea records.

---

## Features 🚀
- **Add a new tea** 🆕
- **Retrieve all teas** 📜
- **Retrieve a tea by ID** 🔍
- **Update a tea's details** ✏️
- **Delete a tea** ❌

---

## Technologies Used 🛠️
- **Node.js**
- **Express.js**
- **dotenv** (for environment variables)

---

## Installation & Setup 🏗️

1. **Clone the repository**
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Install dependencies**
   ```sh
   npm install
   ```

3. **Run the application**
   ```sh
   npm start
   ```

4. The server will start on `http://localhost:3000` (or a port specified in `.env`).

---

## API Endpoints 🌐

### 1️⃣ **Add a New Tea**
- **Endpoint:** `POST /teas`
- **Request Body:**
  ```json
  {
    "name": "Green Tea",
    "price": 10.5
  }
  ```
- **Response:**
  ```json
  {
    "id": 1,
    "name": "Green Tea",
    "price": 10.5
  }
  ```

### 2️⃣ **Get All Teas**
- **Endpoint:** `GET /teas`
- **Response:**
  ```json
  [
    {
      "id": 1,
      "name": "Green Tea",
      "price": 10.5
    }
  ]
  ```

### 3️⃣ **Get a Tea by ID**
- **Endpoint:** `GET /teas/:id`
- **Response (if found):**
  ```json
  {
    "id": 1,
    "name": "Green Tea",
    "price": 10.5
  }
  ```
- **Response (if not found):**
  ```json
  "Tea not found"
  ```

### 4️⃣ **Update a Tea**
- **Endpoint:** `PUT /teas/:id`
- **Request Body:**
  ```json
  {
    "name": "Herbal Tea",
    "price": 12.0
  }
  ```
- **Response:**
  ```json
  {
    "id": 1,
    "name": "Herbal Tea",
    "price": 12.0
  }
  ```

### 5️⃣ **Delete a Tea**
- **Endpoint:** `DELETE /teas/:id`
- **Response:**
  ```json
  "deleted"
  ```

---

## Environment Variables 📌
Create a `.env` file in the root directory and define the `PORT` variable:
```env
PORT=3000
```

---

## Improvements & Future Enhancements 🔮
- ✅ Add a database (MongoDB, PostgreSQL, etc.)
- ✅ Implement authentication for API security
- ✅ Add proper error handling and validation

---

## Author ✍️
**Anant** - Learning backend development and building APIs with Node.js & Express.js.

---



