# e-plantShopping
An online shopping application for a plant nursery (**Paradise Nursery**) offering a variety of house plants. Built with **React** and **Redux Toolkit** to manage the shopping cart state dynamically and seamlessly.

---

## 📋 Table of Contents
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Key Components Overview](#-key-components-overview)
- [License](#-license)

---

## ✨ Features

1. **Landing Page:**
   - Welcome section introducing Paradise Nursery.
   - Quick action button ("Get Started" / "Start Shopping") to transition to the product listing page.

2. **Navigation Bar:**
   - Navigation links to effortlessly switch between the Landing Page, Product Listing, and Shopping Cart.
   - Dynamic cart icon showing the total count of items currently in the cart in real-time.

3. **Product Listing Page:**
   - Plants categorized into at least two sections: **Aromatic Plants** and **Medicinal Plants**.
   - Individual plant cards showcasing:
     - Plant image & name
     - Detailed description
     - Price
     - "Add to Cart" button (disabled or updated to "Added" once the item is added to prevent duplicates).

4. **Shopping Cart Page:**
   - Dedicated cart cards for each added item showing thumbnail, unit price, and subtotal.
   - Quantity adjustment controls (`+` and `-`) that update the subtotal and global total dynamically.
   - **Delete** button to remove an item entirely from the cart.
   - Total cost summary for all items in the cart.
   - **Continue Shopping** button to return to the product listing page.
   - **Checkout** button to finalize the order.

---

## 🛠 Technologies Used

- **React.js** (Functional Components, Hooks: `useState`, `useEffect`)
- **Redux Toolkit** (`@reduxjs/toolkit` & `react-redux`) for global state management
- **HTML5 & CSS3** for responsive and user-friendly styling
- **Git & GitHub** for version control and hosting

---

## 📁 Project Structure

```text
e-plantShopping/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── AboutUs.jsx       # Landing page introduction component
│   │   ├── ProductList.jsx   # Product listing and categories component
│   │   └── CartItem.jsx      # Shopping cart display and controls component
│   ├── redux/
│   │   └── CartSlice.jsx     # Redux slice for managing cart state and reducers
│   ├── App.css               # Main application styles
│   ├── App.jsx               # Root component handling layout and navigation state
│   └── index.js              # Application entry point with Redux Provider setup
├── package.json
└── README.md

🚀 Getting Started
Follow these steps to get a local copy up and running on your machine:
 
1. 🚀 Getting Started
Follow these steps to get a local copy up and running on your machine:
git clone [https://github.com/MaryamOmran1/e-plantShopping.git](https://github.com/MaryamOmran1/e-plantShopping.git)
cd e-plantShopping

2. Install dependencies:
npm install

3. Run the development server:
npm start


Open ⁠http://localhost:3000⁠ to view the application in your browser.

🧩 Key Components Overview 
App.jsx⁠: Manages state-driven navigation across the Landing Page, Product Listing, and Cart Page.
 ⁠AboutUs.jsx⁠: Displays company information and background on the landing view.
 ⁠ProductList.jsx⁠: Renders plant data by category and dispatches ⁠addItem⁠ Redux actions when items are selected.
 ⁠CartSlice.jsx⁠: Defines the Redux slice for the cart state with reducers:
 ⁠addItem⁠: Adds or increments an item in the cart array.
 ⁠removeItem⁠: Filters out an item by ID.
 ⁠updateQuantity⁠: Updates the quantity for a given item.
 ⁠CartItem.jsx⁠: Renders cart items with quantity controls, subtotal calculations, and checkout buttons.
📄 License
This project is licensed under the Apache 2.0 License.
