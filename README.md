# 🚀 30-Day MERN Chat App Development Plan

Goal: Build a **scalable, real-time chat application** using **MERN stack** with production-grade design, features, and deployment.

---

## 📅 Week 1 – Foundation (MVP Build)

**Theme:** Get the core backend, auth, and real-time chat working.

### **Day 1–2: Project Setup**

**Tasks:**

* Initialize MERN stack projects.
* Create folder structure (`/client`, `/server`).
* Setup MongoDB Atlas connection.
* Initialize GitHub repo.

**How to do it:**

* Use `npx create-react-app client` or Vite for frontend.
* Setup backend with `npm init -y`, install `express`, `mongoose`, `dotenv`, `cors`.
* Connect MongoDB Atlas.

**Resources:**

* [Official MERN Stack Docs](https://www.mongodb.com/mern-stack)
* [MongoDB Atlas Setup](https://www.mongodb.com/atlas)
* [Express.js Setup Guide](https://expressjs.com/en/starter/installing.html)

---

### **Day 3–4: Authentication System**

**Tasks:**

* User signup/login with JWT & bcrypt.
* Setup routes `/api/auth/register` and `/api/auth/login`.
* Create user model in MongoDB.
* Handle token storage (localStorage on frontend).

**How to do it:**

* Use `bcrypt` for password hashing.
* Use `jsonwebtoken` for JWT.
* Setup middleware to protect routes.

**Resources:**

* [JWT Authentication Tutorial](https://www.digitalocean.com/community/tutorials/nodejs-jwt-expressjs)
* [React Auth Context Example](https://react.dev/learn/sharing-state-between-components)

---

### **Day 5–6: Real-time Messaging (Socket.io)**

**Tasks:**

* Integrate Socket.io on backend and frontend.
* Create a room per conversation.
* Send and receive messages in real-time.

**How to do it:**

* Use `socket.join(roomId)` for private chats.
* Emit `message` and listen on frontend.

**Resources:**

* [Socket.io Chat Tutorial](https://socket.io/get-started/chat)
* [Socket.io + React Integration](https://dev.to/karanpratapsingh/socketio-react-real-time-app-4oe4)

---

### **Day 7: Basic Chat UI**

**Tasks:**

* Create simple chat UI.
* Implement message list and input bar.
* Display messages dynamically.

**How to do it:**

* Use Tailwind for layout.
* Store messages in local state.

**Resources:**

* [Tailwind CSS Docs](https://tailwindcss.com/docs)
* [React Hooks Guide](https://react.dev/learn/state-a-components-memory)

🎯 **End of Week 1 Goal:**
Users can sign up, log in, and chat in real-time. Messages are stored in MongoDB.

---

## 💬 Week 2 – Feature Expansion & Structure

**Theme:** Add polish, better structure, and persistence.

### **Day 8–9: Conversation System**

**Tasks:**

* Create Conversation model.
* Store and fetch previous chats.
* Show last message preview in chat list.

**Resources:**

* [MongoDB Relationships Guide](https://www.mongodb.com/docs/manual/tutorial/model-embedded-one-to-many-relationships/)

---

### **Day 10–11: Online Status & Seen Indicators**

**Tasks:**

* Track online users via Socket.io.
* Add seen/unseen markers.

**How to do it:**

* Maintain a global user list in server.
* Emit user join/leave events.

**Resources:**

* [Socket.io Presence Tracking Example](https://socket.io/docs/v4/presence/)

---

### **Day 12–13: File Uploads (Images)**

**Tasks:**

* Allow sending images.
* Use Cloudinary for image hosting.

**How to do it:**

* Integrate Cloudinary SDK.
* Add file input + preview.

**Resources:**

* [Cloudinary Node SDK](https://cloudinary.com/documentation/node_integration)
* [React File Upload Example](https://react-dropzone.js.org/)

---

### **Day 14: Refactor and Clean Code**

**Tasks:**

* Organize backend (controllers, routes, services).
* Setup `.env` for secrets.
* Add error handling middleware.

**Resources:**

* [Node.js Project Structuring Best Practices](https://blog.logrocket.com/organizing-express-js-project-structure-better-productivity/)

🎯 **End of Week 2 Goal:**
App supports persistent conversations, online status, file uploads, and clean modular code.

---

## ⚡ Week 3 – Advanced Features & Scalability

**Theme:** Add group chats, typing indicators, and polish UI.

### **Day 15–16: Group Chats**

**Tasks:**

* Add group creation endpoints.
* Allow adding/removing members.
* Handle group messages via Socket.io rooms.

**Resources:**

* [Socket.io Rooms Docs](https://socket.io/docs/v4/rooms/)

---

### **Day 17–18: Typing Indicators & Delivery Status**

**Tasks:**

* Implement typing indicators.
* Show sent/delivered icons.

**Resources:**

* [Socket.io Typing Example](https://stackoverflow.com/questions/42887509/socket-io-how-to-handle-typing-indicator)

---

### **Day 19: Search & Filters**

**Tasks:**

* Add user and chat search.
* Implement debounce.

**Resources:**

* [React Search Input + Debounce](https://dev.to/nilanth/how-to-debounce-search-input-in-react-3ep1)

---

### **Day 20–21: Responsive UI + Themes**

**Tasks:**

* Mobile responsive layout.
* Add light/dark mode toggle.

**Resources:**

* [Tailwind Dark Mode Guide](https://tailwindcss.com/docs/dark-mode)
* [Responsive Design with Tailwind](https://tailwindcss.com/docs/responsive-design)

🎯 **End of Week 3 Goal:**
Polished, feature-rich chat app with modern UX and full responsiveness.

---

## ☁️ Week 4 – Deployment & Final Touches

**Theme:** Deploy, optimize, and prepare for showcase.

### **Day 22–23: Deploy Backend & Frontend**

**Tasks:**

* Backend → Render / Railway.
* Frontend → Vercel.
* Connect MongoDB Atlas (production URI).

**Resources:**

* [Render Deployment Guide](https://render.com/docs/deploy-node-express-app)
* [Vercel React Deployment](https://vercel.com/docs)

---

### **Day 24–25: Scalability Additions**

**Tasks:**

* Add Redis pub/sub (optional for Socket.io scaling).
* Dockerize backend.
* Add Helmet + rate limiting.

**Resources:**

* [Redis Pub/Sub Basics](https://redis.io/docs/latest/develop/interact/pubsub/)
* [Dockerize Node.js App](https://nodejs.org/en/docs/guides/nodejs-docker-webapp)

---

### **Day 26: Documentation & API Docs**

**Tasks:**

* Write detailed README with setup + screenshots.
* Document APIs using Swagger or Postman.

**Resources:**

* [Swagger Docs](https://swagger.io/tools/swagger-ui/)

---

### **Day 27–28: Testing & QA**

**Tasks:**

* Test all chat flows.
* Check UI across browsers.
* Handle edge cases (disconnect/reconnect, slow net).

**Resources:**

* [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)

---

### **Day 29: Final Polish**

**Tasks:**

* Add small animations (Framer Motion).
* Create profile page.
* Record demo video.

**Resources:**

* [Framer Motion Docs](https://www.framer.com/motion/)

---

### **Day 30: Launch & Resume Update**

**Tasks:**

* Final deploy check.
* Push clean commits.
* Update LinkedIn + resume with project link.

**Resume Line Example:**

> Built a full-stack, real-time chat app using MERN & Socket.io. Implemented authentication, group chats, image uploads, typing indicators, and deployed on Render & Vercel with MongoDB Atlas.

🎯 **End of Week 4 Goal:**
Fully deployed, scalable, production-style chat app — resume-ready and impressive for interviews.
