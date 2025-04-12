# Food Delivery App

This is a **Food Delivery App** built using **React** and **Vite**. The application allows users to browse a menu, add items to their cart, and place orders. It features a clean and responsive design, making it easy to use on both desktop and mobile devices.

## Features

- **Home Page**: Displays a header, menu categories, and a list of food items.
- **Cart**: Allows users to view items added to their cart, update quantities, and proceed to checkout.
- **Place Order**: Collects delivery information and calculates the total cost, including a delivery fee.
- **Login Popup**: Provides a modal for user login or account creation.
- **Responsive Design**: Optimized for various screen sizes.
- **Context API**: Manages global state for cart items and food data.

## Project Structure

```
DeliveryApp_Project/
├── public/                # Public assets (e.g., images, icons)
├── src/                   # Source code
│   ├── assets/            # Images and static assets
│   ├── components/        # Reusable UI components
│   │   ├── Navbar/        # Navigation bar
│   │   ├── Header/        # Header section
│   │   ├── Footer/        # Footer section
│   │   ├── FoodItem/      # Individual food item card
│   │   ├── FoodDisplay/   # Displays a list of food items
│   │   ├── ExploreMenu/   # Menu category selector
│   │   ├── LoginPopup/    # Login and signup modal
│   ├── context/           # Context API for global state management
│   ├── pages/             # Application pages
│   │   ├── Home/          # Home page
│   │   ├── Cart/          # Cart page
│   │   ├── PlaceOrder/    # Place order page
│   ├── App.jsx            # Main application component
│   ├── main.jsx           # Entry point
│   ├── index.css          # Global styles
├── .gitignore             # Git ignore file
├── package.json           # Project dependencies and scripts
├── vite.config.js         # Vite configuration
├── eslint.config.js       # ESLint configuration
└── README.md              # Project documentation
```

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd DeliveryApp_Project
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open the app in your browser at `http://localhost:5173`.

## Scripts

- `npm run dev`: Starts the development server.
- `npm run build`: Builds the app for production.
- `npm run preview`: Previews the production build.
- `npm run lint`: Runs ESLint to check for code quality issues.

## Technologies Used

- **React**: Frontend library for building user interfaces.
- **Vite**: Fast build tool for modern web projects.
- **React Router**: For routing between pages.
- **Context API**: For state management.
- **CSS**: For styling components.

## Key Components

### 1. Navbar
- Displays navigation links and a cart icon.
- Shows a dot indicator if there are items in the cart.

### 2. Home Page
- Features a header, menu categories, and a list of food items filtered by category.

### 3. Cart Page
- Lists items added to the cart with options to update quantities or remove items.
- Displays the subtotal, delivery fee, and total cost.

### 4. Place Order Page
- Collects user delivery information.
- Displays a summary of the cart total and delivery fee.

### 5. Login Popup
- Modal for user login or account creation.

## State Management

The app uses the `StoreContext` from the `context/StoreContext.jsx` file to manage global state, including:
- `cartItems`: Tracks items in the cart.
- `food_list`: Contains the list of available food items.
- `addToCart` and `removeFromCart`: Functions to modify the cart.
- `getTotalCartAmount`: Calculates the total cost of items in the cart.

## Assets

The `assets/` folder contains:
- Food images
- Icons for UI elements (e.g., cart, search, add/remove buttons)
- Logos and social media icons

## Future Enhancements

- Add user authentication and profile management.
- Integrate a payment gateway for order processing.
- Implement backend APIs for dynamic data fetching.
- Add order history and tracking features.

## License

This project is licensed under the MIT License.

---

Feel free to contribute to this project by submitting issues or pull requests!