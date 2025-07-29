# 🧑‍💻 Minimal User REST API with Node.js, Express & MongoDB

A simple and modular REST API built with **Node.js**, **Express**, and **MongoDB** to handle:

- ✅ User registration and login
- 🔐 Authentication & JWT authorization
- 🧠 Password hashing with `bcryptjs`
- 🖼️ User-specific data: saved artworks (favourites)
- 📜 Search history tracking

---

## 🔧 Technologies Used

- **Node.js**
- **Express**
- **MongoDB (with Mongoose)**
- **bcryptjs** – for password hashing
- **jsonwebtoken** – for issuing JWT tokens
- **passport & passport-jwt** – for authentication middleware
- **dotenv** – for managing environment variables
- **CORS** – for cross-origin support

## 🚀 Try the App
## 📦 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/user-api.git
cd user-api
```

### 2. Install Dependencies
```bash
npm install
```
### 3. Create .env File
Create a .env file in the root directory with the following:

    PORT=8080
    JWT_SECRET=create_your_own_secret_key
    MONGO_URL=your_mongo_url_here

### 4. Run the server
```bash
node server.js
```

### 5. Test the API
Use Postman or any HTTP client to test the API by making requests to the endpoints.

    POST /api/user/register — Register a new user

    POST /api/user/login — Login and receive a JWT<your_token>

Use the JWT to access protected routes like:

- GET /api/user/favourites
- PUT /api/user/favourites/:id
- DELETE /api/user/favourites/:id
- GET /api/user/history
- PUT /api/user/history/:id
- DELETE /api/user/history/:id

Include the JWT token in the Authorization header like this:
    
    Authorization: jwt <your_token>

## 📄 License

MIT License

## ✍️ Author

Sonam Jamtsho

📧 sjjamtsho@gmail.com | 
🔗 [LinkedIn](https://www.linkedin.com/in/sonam-jamtsho-944288228/)
