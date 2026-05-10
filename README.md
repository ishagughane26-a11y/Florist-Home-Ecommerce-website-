# Florist-Home-Ecommerce-website-
# 🌸 Lily Lane — eCommerce Web Application

> *Blossom with us.* A beautifully crafted online flower shop offering fresh, handcrafted arrangements delivered with love.

---

## 📖 Description

**Lily Lane** is a full-stack eCommerce web application specializing in fresh flowers and floral arrangements. It provides customers with an elegant shopping experience — from browsing a curated collection of blooms to placing orders and tracking purchase history. Built with a clean HTML/CSS/JS frontend and a lightweight Node.js + Express.js backend, it uses an Excel-based database for user management.

---

## ✨ Features

- 🔐 **User Authentication** — Sign up and login with email/password; session managed via `localStorage`
- 🛍️ **Product Catalogue** — Browse a wide range of flowers including Roses, Lilies, Orchids, Tulips, Sunflowers, Jasmine, Marigold, Dahlia, Lavender, and more
- 🛒 **Shopping Cart** — Add/remove items, adjust quantities, view total price, all persisted via `localStorage`
- 💳 **Checkout & Order Placement** — Place orders with a confirmation flow
- 📦 **Order History** — View past orders with order ID, date, items, and status
- 👤 **User Profile** — View logged-in user details and manage account
- 📱 **Responsive Design** — Mobile-friendly layout with hamburger navigation
- 🎬 **About Section** — Embedded brand video showcasing the floral experience
- 🔗 **Social Links & Footer** — Contact info, social media, payment gateway icons, and app store links

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | HTML5, CSS3, Vanilla JavaScript |
| **Backend** | Node.js, Express.js |
| **Database** | Excel (`.xlsx`) via `xlsx` npm package |
| **Styling** | Custom CSS, Google Fonts (WindSong, Major Mono Display) |
| **Icons** | Font Awesome 6 |
| **API Communication** | Fetch API (REST) |
| **State Management** | Browser `localStorage` |

---

## 📁 Folder Structure

```
lilylane/
├── frontend/
│   ├── ecommerce.html        # Home page (landing + featured products)
│   ├── product.html          # Full product listing page
│   ├── cart.html             # Shopping cart page
│   ├── login.html            # Login & Sign Up page
│   ├── profile.html          # User profile page
│   ├── order_history.html    # Order history page
│   ├── ecommerce.css         # Global stylesheet
│   ├── ecommerce.js          # Shared JavaScript utilities
│   ├── hero.jpg              # Hero banner image
│   ├── logo.png              # Brand logo
│   ├── Lily lane.mp4         # About section video
│   ├── *.jpg / *.jpeg        # Product images (roses, lilies, orchids, etc.)
│   ├── app.png               # App Store badge
│   ├── google2.png           # Google Play badge
│   └── card.jpg              # Payment gateway image
│
└── backend/
    ├── server.js             # Express.js server & API routes
    ├── excelHandler.js       # Excel read/write helper functions
    ├── database.xlsx         # User data storage (auto-created)
    ├── package.json          # Dependencies
    └── node_modules/         # Installed packages
```

---

## ⚙️ Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or above)
- npm (comes with Node.js)

### Steps

1. **Clone or extract the project**
   ```bash
   unzip lilylane.zip
   cd lilylane
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Start the backend server**
   ```bash
   npm start
   ```
   The server will start at `http://localhost:3000`

4. **Open the frontend**

   Open `frontend/ecommerce.html` directly in your browser, or use a local server (e.g., VS Code Live Server extension).

   > ⚠️ Make sure the backend server is running before using the app, as login/signup require API calls.

---

## 🚀 Usage Guide

1. **Sign Up** — Visit `login.html`, enter your name, email, and password to create an account.
2. **Login** — Use your registered email and password to log in.
3. **Browse Products** — Explore featured products on the home page or visit `product.html` for the full catalogue.
4. **Add to Cart** — Click "Add to Cart" on any product card; the cart count in the navbar updates live.
5. **View Cart** — Navigate to `cart.html` to review items, update quantities, or remove products.
6. **Place Order** — Click "Buy Now" in the cart to confirm your order.
7. **Order History** — Visit `order_history.html` to view all past orders.
8. **Profile** — Access your account details via the profile icon in the header.
9. **Logout** — Click Logout from the dropdown to end your session.

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/signup` | Register a new user |
| `POST` | `/login` | Authenticate an existing user |

### Sample Request — Signup
```json
POST http://localhost:3000/signup
{
  "name": "Anjali",
  "email": "anjali@example.com",
  "password": "securepassword"
}
```

### Sample Response — Login Success
```json
{
  "message": "Login success",
  "user": {
    "name": "Anjali",
    "email": "anjali@example.com"
  }
}
```

---

## 🔮 Future Enhancements

- [ ] **SQL/MongoDB Database** — Replace Excel storage with a proper database for scalability
- [ ] **Password Hashing** — Implement bcrypt for secure password storage
- [ ] **JWT Authentication** — Token-based session management instead of `localStorage`
- [ ] **Payment Gateway** — Integrate Razorpay / Stripe for real transactions
- [ ] **Admin Panel** — Dashboard to manage products, inventory, and orders
- [ ] **Product Search & Filters** — Search by name, filter by price/category
- [ ] **Wishlist** — Save favourite products for later
- [ ] **Product Reviews** — Allow users to rate and review flowers
- [ ] **Email Notifications** — Order confirmation and delivery updates
- [ ] **Mobile App** — React Native version for iOS and Android

---

## 👩‍💻 Team

| Name | Roll No. |
|---|---|
| Anjali Patalbansi | 03 |
| Annanya Kesharwani | 06 |
| Isha Gughane | 18 |

**Section:** B | **Subject:** Advanced Web Development (AWD)

---

## 📄 License

This project is developed for academic purposes.

---

*Made with 🌸 by Team Lily Lane*
