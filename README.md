# 🚀 RocketNotes API

**"Organize your thoughts, one note at a time!"**  
A robust and secure RESTful API for managing user notes, built with Node.js and Express.

---

## 📦 Overview

Welcome to **RocketNotes API** — a backend service designed to handle user authentication and note management. This API allows users to register, log in, and manage their personal notes with ease.

---

## 🚀 Features

- 🔐 **User Authentication**: Secure registration and login using JWT.
- 📝 **Note Management**: Create, read, update, and delete notes.
- 🏷️ **Tag Support**: Organize notes with tags.
- 📎 **Link Association**: Add relevant links to your notes.
- 🖼️ **Avatar Upload**: Personalize your profile with an avatar.

---

## 🛠️ Tech Stack

- **Node.js** 🟢
- **Express.js** 🚂
- **SQLite** 🗄️
- **Knex.js** 🔗
- **JWT** 🔐
- **Multer** 📁
- **Bcrypt.js** 🔒
- **Dotenv** 🧪

---

## 📂 Folder Structure

```
RocketNotesApi/
├── src/
│   ├── controllers/       # Route handlers
│   ├── routes/            # API routes
│   ├── models/            # Database models
│   ├── middlewares/       # Custom middleware
│   ├── config/            # Configuration files
│   └── utils/             # Utility functions
├── tmp/
│   └── uploads/           # Uploaded files (e.g., avatars)
├── knexfile.js            # Knex configuration
├── package.json           # Project metadata and scripts
└── README.md              # Project documentation
```

---

## 🔧 Installation

To set up the project locally:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yruamkaffer/RocketNotesApi.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd RocketNotesApi
   ```

3. **Install dependencies**:

   ```bash
   npm install
   ```

4. **Set up environment variables**:

   - Create a `.env` file in the root directory.
   - Add the necessary environment variables as shown in `.env.example`.

5. **Run database migrations**:

   ```bash
   npx knex migrate:latest
   ```

6. **Start the development server**:

   ```bash
   npm run dev
   ```

   The server will start on `http://localhost:3333`.

---

## ▶️ How to Use

Once the server is running, you can interact with the API using tools like [Insomnia](https://insomnia.rest/) or [Postman](https://www.postman.com/). Here's a brief overview of the available endpoints:

### Authentication

- `POST /users`: Register a new user.
- `POST /sessions`: Log in and receive a JWT token.

### User Profile

- `GET /users`: Retrieve user profile information.
- `PUT /users`: Update user details.
- `PATCH /users/avatar`: Upload or update user avatar.

### Notes

- `POST /notes`: Create a new note.
- `GET /notes`: Retrieve all notes for the authenticated user.
- `GET /notes/:id`: Retrieve a specific note by ID.
- `DELETE /notes/:id`: Delete a note by ID.

### Tags

- `GET /tags`: Retrieve all tags associated with the user's notes.

### Files

- `GET /files/:filename`: Access uploaded files (e.g., avatars).

---

## 🧪 Tests

This project does not include automated tests. However, manual testing can be performed by:

- Sending HTTP requests to the API endpoints using tools like Insomnia or Postman.
- Verifying the responses and ensuring the expected behavior.

---

## 🙋‍♂️ Contributing

Contributions are welcome! If you'd like to enhance this project:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeature`.
3. Commit your changes: `git commit -m 'Add YourFeature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Open a pull request.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 💬 Contact

Created with ❤️ by [Yruam Käffer de Faria](https://github.com/yruamkaffer)  
📍 Joinville, SC - Brazil  
📸 [Instagram](https://instagram.com/yruamkaffer)
