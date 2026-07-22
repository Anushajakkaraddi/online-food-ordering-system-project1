Markdown
# 🍔 CraveCraft — Online Food Ordering System


https://github.com/user-attachments/assets/ae11e65a-c565-4cc3-bb35-cbfdfdb572af


> A full-stack, enterprise-ready online food ordering platform built with **React 19**, **TypeScript**, **Tailwind CSS v4**, **Node.js/Express**, and integrated with the **Google Gemini API** for smart food recommendations.

---

## 📌 Project Overview

**CraveCraft** is a feature-rich, high-performance web application designed for gourmet restaurant discovery, custom dish ordering, real-time tracking, multi-gateway payments, dynamic coupon redemptions, and user role management (Customer, Restaurant Owner, System Admin).

This repository is configured out-of-the-box as a complete academic or production-ready web application showcasing full-stack integration, reactive UI components, mock data persistence, and an express backend server.

---

## ⚡ Core Capabilities & Features

### 👤 Multi-Persona System (Role Switching)
* **Customer Dashboard:** Browse food items, manage delivery addresses, track live orders, apply discount coupons, manage wishlists, and leave reviews.
* **Restaurant Owner Panel:** View incoming restaurant orders, review analytics, and manage menu availability.
* **System Admin Panel:** Comprehensive analytics suite tracking daily/monthly sales metrics, top dishes, active restaurants, and revenue breakdowns.

### 🍕 Restaurant Discovery & Customization
* **Advanced Search & Filtering:** Filter restaurants by cuisine, veg/non-veg flags, delivery time, ratings, or cost for two.
* **Dish Customization Engine:** Dynamic options for crust choices, portions, extra toppings, and custom chef instructions.
* **Interactive Food Cart:** Real-time subtotal calculation, free delivery thresholds ($25+ waiver), packaging fee computation, and customizable delivery tips.

### 💳 Checkout & Order Tracking
* **Multi-Gateway Checkout Simulation:** Native support for Razorpay, Stripe, PayPal, UPI, Credit Cards, Cash on Delivery (COD), and Wallet balances.
* **Live Order Tracking:** Real-time order progress timeline (`Placed` ➔ `Confirmed` ➔ `Preparing` ➔ `Out for Delivery` ➔ `Delivered`) complete with assigned delivery driver details.

### 🤖 Smart AI Capabilities
* Integrated server-side capabilities with **Google Gemini API** (`@google/genai`) for intelligent food recommendations and context-aware suggestions.

---

## 🛠️ Tech Stack & Dependencies

### **Frontend**
* **Framework:** React 19 (`react`, `react-dom`)
* **Language:** TypeScript (`~5.8.2`)
* **Styling:** Tailwind CSS v4 (`@tailwindcss/vite`, `tailwindcss`)
* **Icons & Motion:** Lucide React (`lucide-react`), Motion (`motion`), Canvas Confetti (`canvas-confetti`)
* **Charts:** Recharts (`recharts`)
* **Build Tool:** Vite 6 (`vite`)

### **Backend & Server**
* **Runtime / Framework:** Node.js, Express (`express`)
* **TypeScript Execution:** `tsx`, `esbuild`
* **AI Integration:** `@google/genai`
* **Environment Configuration:** `dotenv`

---

## 📂 Repository Structure

```text
├── metadata.json          # Application capabilities & framework metadata
├── package.json           # Scripts and dependency declarations
├── server.ts              # Express API server & Vite dev middleware
└── src/
    ├── types.ts           # Core TypeScript definitions (User, Order, FoodItem, etc.)
    ├── data/
    │   └── mockData.ts    # Initial database mock records (Users, Items, Restaurants)
    ├── context/
    │   └── AppContext.tsx # Centralized React Context state provider & hooks
    └── components/
        ├── Header.tsx                 # Navigation bar & role toggle menu
        ├── HeroBanner.tsx             # Main landing hero section with quick filters
        ├── CategoryBar.tsx            # Food category grid slider
        ├── OffersSection.tsx          # Dynamic coupon promo banner
        ├── RestaurantCard.tsx         # Restaurant listing item card
        ├── FoodCard.tsx               # Individual food dish card
        ├── FoodCustomizationModal.tsx # Options & add-ons modal popup
        └── CartDrawer.tsx             # Slide-over food basket drawer
🚀 Getting Started
Prerequisites
Node.js: v18.0.0 or higher

npm or yarn / pnpm

Installation & Setup
Clone the repository:

Bash
git clone [https://github.com/your-username/cravecraft-food-ordering.git](https://github.com/your-username/cravecraft-food-ordering.git)
cd cravecraft-food-ordering
Install dependencies:

Bash
npm install
Configure Environment Variables:
Create a .env file in the root directory:

Code snippet
PORT=3000
GEMINI_API_KEY=your_google_gemini_api_key_here
Start the Development Server:

Bash
npm run dev
The application will launch automatically at http://localhost:3000.
