🧠 AI Text-to-Image Generator (Full Stack MERN + AI SaaS)
📘 Overview

This project is a Full Stack AI SaaS Application built using MongoDB, Express, React, and Node.js.
It allows users to generate AI-powered images from text prompts using the ClipDrop API.
The app includes a credit system, secure authentication, and online payment integration for purchasing additional credits.

🚀 Features

🧾 User Authentication — Sign up, login, and manage accounts (MongoDB, Express, JWT).

🎨 AI Image Generation — Generate high-quality images from text using the ClipDrop API.

💳 Credit System — Users get free credits and can purchase more using integrated payment gateway.

🖼️ Image Gallery — View and download previously generated images.

🔒 Secure Backend — Protected routes and token-based authentication.

💡 Responsive Frontend — Built using React and Tailwind CSS for a modern UI.

🛠️ Tech Stack
Layer	Technology
Frontend	React.js, Tailwind CSS, Axios
Backend	Node.js, Express.js
Database	MongoDB (Mongoose ORM)
Authentication	JWT (JSON Web Tokens)
Payment Gateway	Razorpay / Stripe (as configured)
AI API	ClipDrop API
Deployment	Render / Vercel / MongoDB Atlas
⚙️ Installation & Setup

Clone the repository

git clone https://github.com/your-username/ai-text-to-image-generator.git
cd ai-text-to-image-generator


Install dependencies

# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install


Setup Environment Variables
Create a .env file in both server and client folders with:

MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLIPDROP_API_KEY=your_clipdrop_api_key
PAYMENT_API_KEY=your_payment_gateway_key


Run the application

# Run backend
cd server
npm start

# Run frontend
cd ../client
npm run dev


Visit the app

http://localhost:5173

💰 Credit System

Each user starts with a limited number of free credits.

Every image generation request deducts one credit.

When credits run out, users can securely purchase more using the integrated payment gateway.

🤖 API Used

ClipDrop API
 — Used for generating AI-based images from text prompts.
