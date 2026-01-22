# 🛒 E-Commerce Website

A full-stack e-commerce web application built with **React.js** and **Node.js/Express**, featuring product browsing, shopping cart functionality, user authentication, and Paytm payment integration.

![React](https://img.shields.io/badge/React-18.1.0-61DAFB?logo=react&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Mongoose-47A248?logo=mongodb&logoColor=white)
![Material UI](https://img.shields.io/badge/Material_UI-5.7.0-007FFF?logo=mui&logoColor=white)

---

## ✨ Features

- 🏠 **Home Page** - Browse products with carousel displays and deal highlights
- 🔍 **Product Details** - View detailed product information with images
- 🛒 **Shopping Cart** - Add/remove items, view cart summary and totals
- 👤 **User Authentication** - Login/signup functionality
- 💳 **Payment Integration** - Secure checkout with Paytm payment gateway
- 📱 **Responsive Design** - Optimized for all device sizes
- 🔄 **State Management** - Redux for predictable state management

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|------------|---------|
| React 18 | UI Framework |
| Material UI | Component Library |
| Redux + Redux Thunk | State Management |
| React Router v6 | Client-side Routing |
| Axios | HTTP Client |

### Backend
| Technology | Purpose |
|------------|---------|
| Node.js | Runtime Environment |
| Express.js | Web Framework |
| MongoDB | Database |
| Mongoose | ODM |
| Paytm SDK | Payment Processing |

---

## 📁 Project Structure

```
ecommerce-site/
├── client/                 # React Frontend
│   ├── public/
│   └── src/
│       ├── Components/     # React Components
│       │   ├── Cart/       # Shopping cart components
│       │   ├── Header/     # Navigation & profile components
│       │   ├── Home/       # Homepage components
│       │   ├── ItemDetails/# Product detail view
│       │   └── Login/      # Authentication components
│       ├── redux/          # Redux store & actions
│       ├── context/        # React Context providers
│       ├── service/        # API service layer
│       └── utils/          # Utility functions
│
└── server/                 # Node.js Backend
    ├── controller/         # Route controllers
    ├── database/           # Database connection
    ├── model/              # Mongoose schemas
    ├── routes/             # API routes
    └── paytm/              # Payment integration
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local or Atlas)

### Environment Variables

Create a `.env` file in the `server/` directory:

```env
PORT=8000
DB_USERNAME=your_mongodb_username
DB_PASSWORD=your_mongodb_password
PAYTM_MID=your_paytm_merchant_id
PAYTM_MERCHANT_KEY=your_paytm_merchant_key
PAYTM_WEBSITE=WEBSTAGING
PAYTM_CHANNEL_ID=WEB
PAYTM_INDUSTRY_TYPE_ID=Retail
PAYTM_CUST_ID=customer_id
```

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ecommerce-site.git
   cd ecommerce-site
   ```

2. **Install server dependencies**
   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies**
   ```bash
   cd ../client
   npm install
   ```

### Running the Application

1. **Start the backend server**
   ```bash
   cd server
   npm start
   ```
   Server runs on `http://localhost:8000`

2. **Start the frontend development server**
   ```bash
   cd client
   npm start
   ```
   Client runs on `http://localhost:3000`

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/products` | Fetch all products |
| GET | `/product/:id` | Fetch single product |
| POST | `/cart/add` | Add item to cart |
| POST | `/user/signup` | User registration |
| POST | `/user/login` | User authentication |
| POST | `/payment` | Initialize payment |
| POST | `/callback` | Payment callback |

---


## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---
