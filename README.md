# HabeshaCart Frontend Project StructureHere’s a **short chat version** of the full frontend plan for your **HabeshaCart** multivendor e-commerce app:
🌍 **Project Name**: HabeshaCart
A multivendor e-commerce platform connecting customers with Ethiopian vendors. Built with **React Native + Expo Router** (frontend) and **Django + DRF** (backend).
🔧 **Frontend Tech Stack**
* React Native (Expo)
* Expo Router
* Axios (API)
* React Context (auth/session)
* Shadcn-style UI components
* Tailwind for styling (via NativeWind or similar)
* LocalStorage (AsyncStorage) for session tokens
🔐 **Authentication**
* JWT-based login (`/api/auth/token/`)
* Registration with role: `Customer` or `Vendor` (`/api/auth/register/`)
* Auth persistence + token refresh
* Role-based dashboard routing:
   * Customer → `/dashboard/customer`
   * Vendor → `/dashboard/vendor`
🧱 **UI Structure**
* Welcome Screen (Sign In / Sign Up)
* Sign In
* Sign Up (role-based)
* Customer Dashboard:
   * Browse Products
   * My Wishlist
   * My Cart
   * My Orders
   * Notifications
   * Sign Out
* Vendor Dashboard:
   * My Products
   * Add Product
   * Orders
   * Payouts
   * Notifications
   * Sign Out
💼 **Business Logic**
* Vendors need admin approval after signup
* Orders are split by vendor
* Customers can add products to wishlist/cart
* Checkout triggers vendor notifications
* Payments handled per vendor (Chapa/Stripe)
🔁 **API References**
* `/api/auth/register/` → POST new user
* `/api/auth/token/` → POST for JWT login
* `/api/auth/me/` → GET user info
* `/api/products/` → Browse products
* `/api/wishlist/` → Wishlist logic
* `/api/cart/` → Cart logic
* `/api/orders/` → Order placement, status
* `/api/vendor/payouts/` → Vendor payout info
🎨 **Branding & Styling**
* Clean, minimal UI
* Rounded corners, soft shadows
* Product-first interface
* Bold headers, simple icons
* Consistent brand colors (Ethiopian-themed optional)
✅ **Core Functionalities**
* Register/Login/Logout
* Role-based UI
* Product Browsing
* Wishlist/Cart/Orders
* Notifications
* Vendor tools (Products, Payouts, Orders)
Let me know if you want this turned into a live README, formatted PDF, or editable doc!
