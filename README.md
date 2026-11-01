# 🌱 FreshHarvest – Farm-to-Consumer Marketplace

**Connecting Farmers Directly with Consumers and Bulk Buyers**

FreshHarvest is a web-based farm-to-consumer marketplace that connects farmers directly with customers, restaurants, grocery shops, hotels, and other bulk buyers. The platform aims to reduce middlemen, improve farmers' income, provide fresh agricultural products at fair prices, and make local produce easier to discover and purchase.

---

## 📌 Table of Contents

1. Project Overview
2. Problem Statement
3. Project Objectives
4. Key Features
5. User Roles
6. Modules
7. Technology Stack
8. System Architecture
9. Project Structure
10. Figma UI/UX Design
11. Application Workflow
12. Database Design
13. Installation and Setup
14. Environment Configuration
15. Running the Application
16. API and Backend
17. Testing
18. Deployment
19. Future Enhancements
20. SDG Contributions
21. Team
22. License

---

## 1. Project Overview

FreshHarvest is an online agricultural marketplace designed to establish a direct connection between farmers and buyers.

Traditional agricultural supply chains involve multiple intermediaries, which can increase product prices and reduce the profit received by farmers. FreshHarvest addresses this problem by providing a common digital platform where farmers can list their agricultural products and buyers can purchase them directly.

The platform supports individual customers as well as bulk buyers. It also provides product availability, harvest information, farmer details, transparent pricing, order tracking, and delivery coordination.

**Project Name:** FreshHarvest  
**Project Type:** Web-Based Farm-to-Consumer Marketplace  
**Domain:** Agriculture and E-Commerce  
**Frontend:** React.js  
**Backend:** Node.js and Express.js  
**Database:** MongoDB  

## 2. Problem Statement

Farmers often depend on middlemen to sell their agricultural products. This can result in lower profits for farmers and higher prices for consumers.

Buyers also face difficulties in finding fresh local produce, checking product availability, identifying actual farmers, and understanding product quality.

FreshHarvest aims to solve these problems through a centralized digital marketplace that supports direct farmer-to-consumer and farmer-to-business transactions.

## 3. Project Objectives

- Connect farmers directly with consumers and bulk buyers.
- Reduce dependency on middlemen.
- Provide transparent and fair product pricing.
- Help customers discover fresh and locally available produce.
- Display farmer details, farm location, and harvest information.
- Support bulk purchasing for businesses.
- Reduce food waste through surplus produce listings.
- Provide secure authentication and payment options.
- Improve order management and delivery tracking.
- Create a simple and user-friendly shopping experience.

## 4. Key Features

### Direct Farmer-to-Consumer Connection
Customers can discover agricultural products and purchase them directly from farmers.

### Farmer Information
Customers can view farmer names, farm locations, and available farm and product details.

### Product Discovery
Users can search and filter products based on category, price, and location.

### Harvest and Availability
Farmers can provide harvest dates, available quantities, and stock information.

### Transparent Pricing
Buyers can view product prices and compare available products.

### Bulk Ordering
Restaurants, hotels, grocery shops, and other businesses can purchase agricultural products in larger quantities.

### Surplus Produce Management
Farmers can list unsold or surplus produce at discounted prices to reduce food waste.

### Order Tracking
Customers can follow their orders through different order-processing stages.

### Delivery Management
Delivery partners can view assigned orders and update delivery status.

### Ratings and Reviews
Customers can share feedback about products and their purchasing experience.

---

## 5. User Roles

FreshHarvest supports five main user roles.

| User Role | Responsibilities |
|---|---|
| Customer | Browse products, purchase items, make payments, track orders, and provide reviews. |
| Farmer | Manage farm profiles, add products, update stock, accept orders, and monitor earnings. |
| Bulk Buyer | Purchase products in bulk, manage business orders, and communicate with farmers. |
| Delivery Partner | View assigned deliveries, update delivery status, and manage delivery information. |
| Admin | Manage users, products, orders, complaints, platform activities, and reports. |

---

## 6. Project Modules

FreshHarvest is organized into the following functional modules.

### A. User Management

1. User Registration and Authentication
2. Farmer Registration and Verification
3. Customer Profile Management
4. User Management – Admin
5. Role-Based Access Control

### B. Product and Farmer Management

6. Product Management
7. Product Discovery and Search
8. Farmer Profile and Farm Information
9. Inventory and Stock Management
10. Native-Based Farmer Search
11. Harvest Date and Availability
12. Transparent Pricing

### C. Customer and Business Operations

13. Direct Farmer–Buyer Communication
14. Bulk Buyer Management
15. Bulk Order Management
16. Shopping Cart
17. Checkout and Address Management
18. Payment Management
19. Order Management
20. Surplus and Unsold Produce Management

### D. Delivery and Customer Experience

21. Delivery Partner Assignment and Tracking
22. Ratings and Reviews
23. Notifications Center
24. Complaint and Support Management

### E. Administration and Technical Operations

25. Farmer Dashboard and Earnings
26. Bulk Buyer Dashboard
27. Platform Management – Admin
28. Reports and Analytics
29. Database Management
30. Security and Authorization
31. API and Integration
32. Testing, Deployment, and Maintenance

---

## 7. Technology Stack

| Layer | Technology |
|---|---|
| Frontend | React.js |
| Frontend Build Tool | Vite |
| Styling | CSS / Tailwind CSS, where used |
| Backend | Node.js |
| Backend Framework | Express.js |
| Database | MongoDB |
| Database Connectivity | Mongoose, where used |
| Authentication | Role-based authentication |
| API Testing | Postman |
| UI/UX Design | Figma |
| Version Control | Git and GitHub |
| Deployment | Vercel and Render |

**Note:** The table describes the project's technology stack. Confirm the actual packages and configuration files in the repository before treating every optional technology as an implemented dependency.

---

## 8. System Architecture

FreshHarvest follows a client-server architecture.

```text
              USERS
                |
    ---------------------------
    |      |       |          |
 Customer Farmer Bulk Buyer Admin
    |      |       |          |
    ---------------------------
                |
         REACT FRONTEND
                |
          HTTP / REST API
                |
        NODE.JS + EXPRESS
                |
    ---------------------------
    |           |             |
 Authentication Product     Orders
    |         Management   Management
    |           |             |
    ---------------------------
                |
             MONGODB
                |
       STORED APPLICATION DATA
```

### Frontend
Provides the user interface for customers, farmers, bulk buyers, delivery partners, and administrators.

### Backend
Handles authentication, business logic, product operations, orders, payments, and communication between the frontend and database.

### Database
MongoDB stores user information, farmer details, product listings, inventory, orders, and other application data.

---

## 9. Project Structure

The project can be organized into the following structure. Adjust folder names to match the actual repository.

```text
FreshHarvest/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── services/
│   │   ├── hooks/
│   │   ├── context/
│   │   ├── styles/
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── utils/
│   ├── data/
│   ├── server.js
│   └── package.json
│
├── README.md
├── .gitignore
└── .env.example
```

---

# 10. Figma UI/UX Design

FreshHarvest uses Figma for user research, affinity mapping, wireframing, UI design, component creation, and interactive prototyping.

The design focuses on simplicity, accessibility, consistency, and a natural agricultural theme.

## 10.1 Design Objectives

- Create an easy-to-understand interface.
- Provide separate dashboards for different user roles.
- Make product discovery simple.
- Display important product and farmer information clearly.
- Maintain consistent colors, typography, and components.
- Reduce unnecessary visual elements.
- Support a responsive user experience.

## 10.2 Design Tool

**Tool:** Figma  
**Design Type:** Web Application UI/UX  
**Design Approach:** User-Centered Design  
**Prototype Type:** Interactive Prototype

## 10.3 Color Palette

The FreshHarvest interface uses a natural green-based color palette.

| Color | Hex Code | Usage |
|---|---|---|
| Forest Green | `#244C3A` | Primary buttons, headings, navigation |
| Secondary Green | `#477A49` | Secondary actions and highlights |
| Light Sage | `#E9EFE5` | Backgrounds and selected sections |
| Main Background | `#F8F7F1` | Page background |
| White | `#FFFFFF` | Cards and content sections |
| Main Text | `#303830` | Primary text |
| Muted Text | `#737A70` | Secondary text |
| Terracotta | `#B56E43` | Small accent elements |

## 10.4 Typography

The design uses a clean sans-serif typography system.

| Element | Suggested Size |
|---|---|
| Main Heading | 28–32 px |
| Section Heading | 20–24 px |
| Card Heading | 16–18 px |
| Body Text | 14–16 px |
| Supporting Text | 12–14 px |

**Suggested Font:** Poppins

## 10.5 Figma Design Frames

The following screens form the main FreshHarvest UI design.

### Authentication Screens
- Login Page
- Registration Page
- Two-Factor Authentication Flow

### Customer Screens
- Home Page
- Consumer Dashboard
- Find Farmers
- Product Details
- Shopping Cart
- Checkout
- Order Tracking
- Customer Profile

### Farmer Screens
- Farmer Dashboard
- Farmer Profile
- Farm Details
- Product Management
- Inventory Management
- Farmer Orders
- Earnings
- Surplus Produce Management

### Bulk Buyer Screens
- Bulk Buyer Dashboard
- Bulk Product Discovery
- Bulk Order Management
- Farmer Communication

### Delivery Screens
- Delivery Partner Dashboard
- Assigned Orders
- Delivery Status Updates

### Admin Screens
- Admin Dashboard
- User Management
- Product Management
- Order Management
- Complaint Management
- Reports and Analytics

### Design Reference Screens
- FreshHarvest UI Style Guide
- Affinity Mapping
- Wireframes
- High-Fidelity Mockups
- Interactive Prototype

## 10.6 Affinity Mapping

Affinity mapping is used to organize user research findings into related groups and identify common problems and user requirements.

The FreshHarvest affinity mapping is based on user feedback and the problems identified during the research process.

**Raw user ideas include:**
- Difficult to find fresh produce locally.
- Middlemen increase prices.
- Product quality is uncertain.
- Difficult to identify actual farmers.
- Product availability is unknown.
- Need to buy directly from farmers.
- Need to know product prices and farmer details.
- Need easy product searching.
- Need filtering by price, category, and location.
- Want secure payment options.
- Want timely delivery.
- Want order tracking.
- Registration should be easy.
- Need clear product details and images.

**Grouped research findings:**

| Group | Identified Needs |
|---|---|
| Customer Needs | Fresh produce, clear prices, farmer details, easy search, secure payments, order tracking |
| Farmer Needs | Direct selling, fair prices, inventory management, customer communication |
| Bulk Buyer Needs | Bulk ordering, reliable supply, price comparison, product availability |
| Delivery Needs | Assigned deliveries, route information, status updates |
| Platform Needs | Easy registration, secure login, clear product information, simple interface |

**Key Insights:**
- Users prefer buying fresh produce directly from farmers.
- Transparency in pricing and farmer details builds trust.
- Product search and filtering should be simple.
- Farmers need an easy way to manage products and orders.
- Bulk buyers require larger quantities and reliable availability.

## 10.7 Main UI Components

Reusable Figma components include:

- Primary and secondary buttons
- Input fields
- Search bar
- Navigation bar
- Sidebar navigation
- Product cards
- Farmer information cards
- Dashboard summary cards
- Status badges
- Tables
- Modal dialogs
- Notification components
- Profile components

## 10.8 Prototype Interactions

The interactive prototype demonstrates important user journeys.

- Login and registration navigation.
- Submit button success interaction.
- Home page to product details.
- Product details to shopping cart.
- Cart to checkout.
- Checkout to order confirmation.
- Dashboard navigation.
- Farmer product management navigation.
- Order status and tracking interactions.

**Figma Design Link:** [Add your Figma project link here]

---

## 11. Application Workflow

### Customer Workflow

```text
Register / Login
       |
       v
   Home Page
       |
       v
 Discover Products
       |
       v
 View Product Details
       |
       v
 Add to Cart
       |
       v
    Checkout
       |
       v
  Make Payment
       |
       v
  Place Order
       |
       v
 Track Delivery
       |
       v
  Give Review
```

### Farmer Workflow

```text
Farmer Registration
        |
        v
  Farmer Verification
        |
        v
   Farmer Dashboard
        |
        v
  Add / Manage Products
        |
        v
  Update Stock Details
        |
        v
  Receive Customer Orders
        |
        v
  Accept and Process Orders
        |
        v
  Manage Earnings
```

### Bulk Buyer Workflow

```text
Bulk Buyer Login
       |
       v
 Bulk Dashboard
       |
       v
 Discover Products
       |
       v
 Select Quantity
       |
       v
 Contact Farmer / Place Order
       |
       v
 Track Bulk Order
```

### Delivery Partner Workflow

```text
Delivery Partner Login
         |
         v
 View Assigned Orders
         |
         v
 View Delivery Details
         |
         v
 Update Delivery Status
         |
         v
 Complete Delivery
```

---

## 12. Database Design

MongoDB is used as the database for storing application information.

The main data collections may include:

| Collection | Purpose |
|---|---|
| Users | User authentication and profile information |
| Farmers | Farmer and farm details |
| Products | Agricultural product information |
| Categories | Product categories |
| Inventory | Product stock and availability |
| Orders | Customer and bulk orders |
| Payments | Payment transaction details |
| Addresses | Customer delivery addresses |
| Reviews | Customer ratings and reviews |
| Notifications | User notifications |
| Complaints | Support requests and complaints |
| Deliveries | Delivery assignments and status |

The final collection names and relationships should be verified against the actual MongoDB models.

---

## 13. Installation and Setup

### Prerequisites

Install the following software:

- Node.js
- npm
- MongoDB Community Server
- Git
- Visual Studio Code
- Postman (for API testing)

### Step 1: Clone the Repository

```bash
git clone https://github.com/arunpcse/Farm-to-Consumer.git
```

### Step 2: Open the Project

```bash
cd Farm-to-Consumer
```

### Step 3: Install Frontend Dependencies

Run this command in the directory containing the frontend `package.json`.

```bash
npm install
```

### Step 4: Install Backend Dependencies

```bash
cd backend
npm install
```

### Step 5: Configure MongoDB

Start your local MongoDB server.

The local development database URL used for FreshHarvest is:

```env
MONGODB_URI=mongodb://127.0.0.1:27017/freshharvest
```

---

## 14. Environment Configuration

Create an environment file in the appropriate backend directory.

Example `.env`:

```env
PORT=5000
MONGODB_URI=mongodb://127.0.0.1:27017/freshharvest
JWT_SECRET=your_secret_key
```

Add any additional environment variables required by the actual application, such as payment gateway credentials or frontend API URLs.

**Important:** Never upload real passwords, API keys, database credentials, or payment secrets to GitHub.

---

## 15. Running the Application

### Start the Backend

Open a terminal inside the backend directory:

```bash
npm run dev
```

The backend is configured to use port:

```text
http://localhost:5000
```

### Start the Frontend

Open another terminal in the directory containing the frontend `package.json`:

```bash
npm run dev
```

Vite commonly runs the frontend at:

```text
http://localhost:5173
```

If the terminal displays a different port, use the URL shown there.

---

## 16. API and Backend

The backend uses Node.js and Express.js to provide REST API functionality.

Main API areas include:

- Authentication APIs
- User APIs
- Farmer APIs
- Product APIs
- Inventory APIs
- Cart APIs
- Order APIs
- Payment APIs
- Bulk Buyer APIs
- Delivery APIs
- Review APIs
- Notification APIs
- Admin APIs
- Support APIs

The exact endpoints, HTTP methods, request formats, and response structures are defined by the implemented backend routes.

Postman can be used to test the API requests and responses.

---

## 17. Testing

Testing is important to ensure that FreshHarvest works correctly.

### Testing Areas

1. User registration and login.
2. Farmer profile management.
3. Product creation and updating.
4. Inventory and stock management.
5. Product searching and filtering.
6. Cart and checkout operations.
7. Payment reliability.
8. Order processing.
9. Bulk buyer operations.
10. Delivery status updates.
11. Admin operations.
12. Database persistence.
13. Frontend production build.

### Example Testing Commands

Run only the scripts that actually exist in the project:

```bash
node test_phase5_farmer_operations.js
node verify_persistence.js
node test_payment_reliability.js
node test_admin_and_fulfillment.js
node api.test.js
```

### Frontend Build Test

```bash
npm run build
```

Record the actual test results and any issues in the project test report.

---

## 18. Deployment

FreshHarvest uses the following deployment services in its project workflow:

| Component | Platform |
|---|---|
| Frontend | Vercel |
| Backend | Render |
| Database | MongoDB |

### Deployment Process

1. Push the latest project code to GitHub.
2. Configure the frontend deployment on Vercel.
3. Configure the backend deployment on Render.
4. Set production environment variables.
5. Configure the MongoDB connection string.
6. Set the frontend API base URL to the deployed backend.
7. Configure CORS for the deployed frontend domain.
8. Test the deployed application.

**Deployment Links:**

- GitHub Repository: https://github.com/arunpcse/Farm-to-Consumer
- Frontend: Add your Vercel deployment URL.
- Backend: Add your Render deployment URL.
- Figma: Add your Figma design URL.

---

## 19. Future Enhancements

The following features can improve the FreshHarvest platform in future versions:

- AI-based product recommendations.
- Weather-based farming information.
- Advanced demand prediction.
- Improved delivery route optimization.
- Multilingual user interface.
- Real-time chat between farmers and buyers.
- Advanced analytics for farmers.
- Mobile application for customers and farmers.
- More detailed product quality verification.

---

## 20. SDG Contributions

FreshHarvest supports the following United Nations Sustainable Development Goals.

| SDG | Goal | Contribution |
|---|---|---|
| SDG 2 | Zero Hunger | Improves access to fresh agricultural products. |
| SDG 8 | Decent Work and Economic Growth | Supports farmers through direct selling opportunities. |
| SDG 12 | Responsible Consumption and Production | Encourages responsible purchasing and reduces surplus food waste. |

---

## 21. Team

**Project:** FreshHarvest – Farm-to-Consumer Marketplace

| Name | Role |
|---|---|
| Arun P | Project Team Member |
| Aathavan R | Project Team Member |
| Anbarasan A | Project Team Member |
| Arisudhan P | Project Team Member |

---

## 22. License

This project is developed for academic and educational purposes.

You may update the licensing information based on the final project requirements.

---

## 🌾 FreshHarvest

**Fresh Food. Fair Prices. Better Farming.**

Connecting farmers and buyers through a simple digital marketplace.
