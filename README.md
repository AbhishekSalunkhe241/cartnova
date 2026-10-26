# 🛍️ CartNova — Modern Online Shopping Platform

CartNova is a full-stack, responsive modern e-commerce web application designed for a smooth and intuitive shopping experience. It features categorized product browsing, real-time search, interactive shopping cart management, toast notifications, order processing, and a MongoDB backend.

---

## ✨ Features

- **Responsive Modern UI**: Built with a sleek design system, fluid animations, and mobile-first responsive layout.
- **Product Catalog & Categorization**: Browse items across categories (Smartphones, Audio, Laptops, Wearables, Accessories).
- **Search & Filtering**: Instant client-side search with debounce and real-time category filtering.
- **Interactive Shopping Cart**: Add, increase, decrease, or remove items with real-time price updates and persistent state.
- **Order Checkout Flow**: Seamless checkout modal with form validation and order confirmation.
- **Backend API**: Built with Node.js and Express to serve products and handle incoming customer orders.
- **Database Integration**: MongoDB schema with Mongoose for products and customer orders.
- **Vercel Serverless Ready**: Configured with `vercel.json` and serverless API handlers for instant deployment.

---

## 🛠️ Tech Stack

- **Frontend**: HTML5, Vanilla JavaScript (ES6+), Tailwind CSS, Lucide Icons
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (Mongoose ODM)
- **Deployment**: Vercel Serverless Functions

---

## 📁 Project Structure

```text
├── api/
│   └── index.js             # Serverless handler for Vercel deployment
├── models/
│   ├── Order.js             # Mongoose order schema & model
│   └── Product.js           # Mongoose product schema & model
├── public/
│   ├── images/              # Optimized product catalog imagery
│   ├── index.html           # Single-page frontend application
│   └── logo.png             # CartNova brand assets
├── .env.example             # Environment variable template
├── .gitignore               # Git ignore rules
├── package.json             # Project dependencies and run scripts
├── seed.js                  # Database seeding script with sample products
├── server.js                # Local Express application server
└── vercel.json              # Vercel deployment configuration
```

---

## 🚀 Getting Started

### 1. Prerequisites
- [Node.js](https://nodejs.org/) (v18 or higher)
- [MongoDB](https://www.mongodb.com/) (Local instance or MongoDB Atlas cluster URI)

### 2. Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/AbhishekSalunkhe241/cartnova.git
cd cartnova
npm install
```

### 3. Environment Configuration
Create a `.env` file from `.env.example`:
```bash
cp .env.example .env
```
Update your MongoDB connection string in `.env`:
```env
PORT=5000
MONGODB_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/cartnova?retryWrites=true&w=majority
```

### 4. Seed Products (Optional)
Populate the database with sample inventory:
```bash
node seed.js
```

### 5. Run the Application
Start the development server:
```bash
npm start
```
Open your browser and navigate to `http://localhost:5000`.

---

## 🌐 Deployment to Vercel

1. Push your code to GitHub.
2. Import the repository into your [Vercel Dashboard](https://vercel.com).
3. Add the `MONGODB_URI` environment variable in your Vercel Project Settings.
4. Deploy!
