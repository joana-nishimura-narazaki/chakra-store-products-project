# 🛍️ Full Stack Product Management App

This project is a full stack web application developed to practise and apply modern web development skills. It combines a RESTful API built with **Node.js**, **Express**, and **MongoDB**, and a responsive frontend using **React**, **Chakra UI**, **React Router**, and **Zustand**.

## ⚙️ Features

- Create, read, update, and delete (CRUD) products  
- Responsive UI with Chakra UI  
- State management using Zustand  
- Edit products via modal with real-time state updates  
- Integrated frontend and backend on a single domain  
- Deployed with production-ready static serving via Express

## 🧠 Technologies Used

### Backend
- Node.js  
- Express.js  
- MongoDB + Mongoose  
- RESTful API  
- Modular code structure (routes, controllers, models)  
- Tested using Insomnia

### Frontend
- React  
- Chakra UI (for components and theming)  
- React Router DOM  
- Zustand (for global state management)  
- Custom components (Navbar, ProductCard, Modal)

## 📁 Project Structure

```bash
root/
├── backend/
│   ├── db.js
│   ├── models/
│   ├── routes/
│   └── controllers/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── store/
```

## 🛠️ How to Run Locally

```bash
# Clone the repository
git clone https://github.com/your-username/product-management-app

# Backend setup
cd backend
npm install
npm run dev

# Frontend setup
cd ../frontend
npm install
npm run dev
```

## 🚀 Deployment

In production, Express serves the React build statically:

```js
if (process.env.NODE_ENV === "production") {
  app.use(express.static(path.join(__dirname, "/frontend/dist")));
  app.get("*", (req, res) => {
    res.sendFile(path.resolve(__dirname, "frontend", "dist", "index.html"));
  });
}
```

This allows frontend and backend to run on the same domain, simplifying deployment and maintenance.

## 👩‍💻 About Me

Hi! I’m **Joana**, a developer passionate about building scalable and well-structured full stack applications. This project was created for my portfolio and reflects the technologies I’ve been learning and applying.

