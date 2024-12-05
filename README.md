# সিলেটী দোকান 🛍️
- [Software Requirements Specification](README.md)
- [REST API Endpoints](REST-API-Design.md)
- [Wireframe or Mockup File](Wireframe-of-SD.md)

## Software Requirements Specification (SRS)  
📑Project Name: সিলেটী দোকান   
👩🏻‍💻 Prepared By: Mehedi Hasan Parvez (Software Developer)    
📆 Date: 15 Octobar 2024   

## 1. Introduction 🛒

### 1.1 Purpose  
The objective of this document is to define the requirements for creating a Sylheti-Dukan.com (সিলেটী দোকান) using the MERN stack. This e-commerce platform will enable users to browse products, manage their accounts, add items to their cart, and complete purchases through a secure payment system.

### 1.2 Scope  
This project involves developing a fully functional e-commerce website with features including:  
- Product browsing and filtering.  
- Secure user authentication and account management.  
- Shopping cart functionality.  
- Integration with payment gateways.    

The system will be scalable, user-friendly, and optimized for performance. To enhance performance, a caching system will be implemented using "Node-Cache".  

### 1.3 Definitions, Acronyms
- MERN: MongoDB, Express.js, React.js, Node.js.  
- API: Application Programming Interface.  
- CRUD: Create, Read, Update, Delete operations.   

## 2. Overall Description 🛒  

### 2.1 Product Perspective  
The Sylheti-Dukan.com (সিলেটী দোকান) will function as a standalone web application. It will follow a modular design to ensure ease of maintenance and future scalability.  

### 2.2 Product Features  
- User Authentication - Secure login and registration.  
- Product Catalog - Categorized and searchable product listings.  
- Cart System - Add, update, and remove items.  
- Order Management - Track orders and view purchase history.  
- Payment Gateway - Process payments securely.  
- Admin Panel - Manage inventory, orders, and analytics.  

### 2.3 User Classes and Characteristics  
- Customers: Individuals purchasing items.  
- Admins: Manage products, categories, and orders.  

### 2.4 Operating Environment  
- Frontend: React.js, Sass for styling.  
- Backend: Node.js and Express.js.  
- Database: MongoDB hosted on MongoDB Atlas.  

### 2.5 Assumptions and Dependencies  
- Reliable internet connection.  
- Integration with "Bkash" for payments.  

## 3. Functional Requirements 🛒   

### 3.1 User Authentication  
- Users must register and log in using email and password.  
- Passwords are stored securely using bcrypt.  
- JWT tokens are used for secure sessions.  

### 3.2 Product Management  
- Users can browse products by category or use a search bar.  
- Product pages include images, descriptions, pricing, and availability.  

### 3.3 Cart Functionality  
- Users can add, update, and remove items in their cart.  
- Cart data persists across sessions for logged-in users.  

### 3.4 Order Processing  
- Checkout includes address entry and payment processing.  
- Order details are saved and viewable in the user's profile.  

### 3.5 Admin Panel Features

### **📅 Dashboard**
The dashboard provides an overview of the platform’s key metrics, including:
- **Summary Metrics**:
  - Current revenue.
  - Total users.
  - Total products.
  - Recent transactions.
- **Additional Insights**:
  - Inventory ratio.
  - Gender ratio of users.
  - Top transactions displayed in a table.

### **🧱 Management Section**
Admins can manage core aspects of the platform, including:
- **Products**: Add, edit, and delete items.
- **Orders**: Track, update, and fulfill orders.
- **Customers**: Manage user information and interactions.

### **📊 Charts Overview**

### **Bar Charts**
1. **Top Transactions & Top Customers**: Displays data for the last 6 months.
2. **Orders Throughout the Year**: Monthly order trends.

### **Pie and Doughnut Charts**
1. **Order Fulfillment Ratio**: Percentage of completed vs. pending orders.
2. **User Age Group Distribution**: Breakdown of users by age group.
3. **Product Category Ratio**: Distribution of products across categories.
4. **Stock Availability**: Ratio of in-stock vs. out-of-stock products.
5. **Revenue Distribution**: Revenue contribution by various sources.
6. **Admin-to-Customer Ratio**: Proportion of admins to customers.

### **Line Charts**
1. **Active Users**: Tracks active users over the past 12 months.
2. **Total Products (SKU)**: Monthly SKU count trends for the last year.
3. **Total Revenue**: Revenue trends over the last 12 months.
4. **Discounts Allotted**: Trends in discounts provided over the year.

## 4. Non-Functional Requirements 🛒

### 4.1 Performance Requirements  
- Load time for each page must not exceed 2 seconds.  
- Handle up to 200 concurrent users.  

### 4.2 Security Requirements  
- Use HTTPS for secure communication.  
- Encrypt sensitive user data.  
- Implement role-based access control.  

### 4.3 Usability Requirements  
- Responsive design for mobile and desktop.  
- Easy navigation and intuitive UI.  

### 4.4 Scalability  
- Support increasing user base and expanding inventory. 

### 4.5 Caching System 
- API requests for cached data will first check the cache before querying the database.
- Automatically clear outdated or expired cache entries.

## 5. System Architecture 🛒

### 5.1 Frontend  
- React.js for the user interface.  
- React Router for navigation.  

### 5.2 Backend  
- Node.js with Express.js for REST APIs.  

### 5.3 Database  
- MongoDB for storing user, product, and order data.  

### 5.4 Third-Party Integrations  
- Payment gateway (Bkash Payment).  

## 6. Design Constraints 🛒 
- The application must be built using the MERN stack.  
- Deployment should use platforms like Vercel (frontend), Heroku (backend), and MongoDB Atlas (database).  

## 7. Appendices 🛒 

### 7.1 Tools and Technologies  
- Visual Studio Code, Postman, Git.  

### 7.2 References  
- Original website: [SylhetiDukan.com](https://mmmm.com)
