# 📱 Social Media Clone

A personal project recreating the core features of a social media platform. It’s built to learn full‑stack development by implementing user registration, posting, commenting, liking, and real-time interaction.

---

## 🎯 Purpose

This project is designed to:

- Practice building a full-stack web app from scratch  
- Understand authentication, database relations, and API development  
- Gain hands-on experience with frontend state management and real-time UI updates  
- Bridge the gap between learning and building a real-world social platform

---

## 🚀 Features

- ✅ User registration and login (with password hashing and validation)  
- 📝 Create, edit, and delete posts  
- ❤️ Like/unlike posts  
- 💬 Comment on posts  
- 🕒 Real-time updates (e.g., adding comments, toggling likes)  
- 🔒 Protected routes and API endpoints for users only

---
## 🧩 User Interface
<img width="1266" height="826" alt="Screenshot from 2025-08-10 17-30-26" src="https://github.com/user-attachments/assets/2cd735ed-076a-4a06-b955-d789e98a93d9" />

<img width="1266" height="826" alt="Screenshot from 2025-08-10 17-30-44" src="https://github.com/user-attachments/assets/7d89cec3-e49b-4a42-b041-eae41940e14a" />

---

## 🧰 Technologies

- **Frontend**: React, React Router, Context API or Redux  
- **Backend**: Node.js, Express  
- **Database**: MongoDB (NoSQL)  
- **Real-time**: WebSockets (Socket.io) or polling  
- **Auth**: JSON Web Tokens (JWT)  
- **Styling**: CSS or styled-components / UI framework of choice

---

## ⚙️ Setup & Running

### 1. Clone the repo  
```bash
git clone https://github.com/shubhamparulekar/social_media_clone.git
cd social_media_clone
````

### 2. Install dependencies

```bash
# For backend
cd server
npm install

# For frontend
cd ../client
npm install
```

### 3. Configure environment

Create a `.env` file in `server/` with:

```
PORT=5000
MONGO_URI=<your_mongo_connection_string>
JWT_SECRET=<your_secret_key>
```

### 4. Run the app

```bash
# From root directory
npm run dev
```

This will start both server and client (via concurrently or separate tabs).

* Backend runs on `http://localhost:5000`
* Frontend runs on `http://localhost:3000`

---

## 🧩 How It Works

* **Client** communicates with the Express API via REST endpoints
* **Authentication** uses JWT stored in HTTP-only cookies or localStorage
* **Real-time features** (likes/comments) are powered by WebSockets or polling
* **Protected routes** verify tokens before granting access

---

## 📝 API Overview

| Method | Endpoint                 | Description                        |
| ------ | ------------------------ | ---------------------------------- |
| POST   | `/api/auth/register`     | Register a new user                |
| POST   | `/api/auth/login`        | User login returns a JWT           |
| GET    | `/api/posts`             | Fetch all posts                    |
| POST   | `/api/posts`             | Create a new post                  |
| PUT    | `/api/posts/:id`         | Edit an existing post (owner only) |
| DELETE | `/api/posts/:id`         | Delete post (owner only)           |
| POST   | `/api/posts/:id/like`    | Toggle like on a specific post     |
| POST   | `/api/posts/:id/comment` | Add a comment to a specific post   |

---

## 📌 Future Enhancements

* Add photo/video uploads
* Implement user profiles and follow/unfollow system
* Add notifications and real-time chat
* Improve UI/UX (infinite scroll, mobile responsiveness, theming)
* Add tests and CI/CD integration

---

## 🙌 Contributions

This is a personal learning project, but contributions are welcome!

If you'd like to help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature-xyz`)
3. Add and test your feature
4. Commit and push your changes
5. Open a pull request with a description of your updates

Feel free to improve documentation, add features, or fix bugs!

---

## 📄 License

This project is released under the **MIT License**. See the [LICENSE](LICENSE) file for full details.

---

Thanks for stopping by! Feel free to explore the code, clone it, and add your own extensions. 🚀
