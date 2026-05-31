# Company Website CMS Prototype

A lightweight full-stack company website management system built with Flask, SQLite, HTML, CSS, and JavaScript.

This project was designed to simulate a practical business website workflow by integrating frontend pages, admin management, backend APIs, and database support into a lightweight content management system (CMS).

The project focuses on frontend–backend integration, CRUD workflow design, product management, content organization, and lightweight deployment architecture.

---

## Preview

### Frontend Website
- Company homepage
- Product center
- Product detail pages
- Category filtering
- Dynamic product rendering
- Interactive UI effects

### Admin Dashboard
- Login system
- Dashboard overview
- Article management
- Product management
- News & solution management
- CRUD operations

---

## Features

### Website Frontend
- Multi-page company website structure
- Homepage, products, and product detail pages
- Product category filtering
- Dynamic product rendering from backend API
- Interactive UI animations and smooth scrolling
- Responsive layout components

### Admin CMS
- Admin dashboard interface
- Article management system
- Product management workflow
- Solution and news management
- CRUD operations (Create, Read, Update, Delete)
- Lightweight content organization system

### Backend & Database
- Flask backend API
- SQLite database persistence
- REST-style API endpoints
- Frontend–backend data synchronization
- Local data storage and content management

---

## Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript (Vanilla JS)

### Backend
- Python
- Flask

### Database
- SQLite

### Deployment / Environment
- Local Python Server
- Lightweight CMS architecture

---

## System Architecture

text Frontend Website (HTML / CSS / JavaScript)            ↓        Flask Backend          (server.py)            ↓       SQLite Database           (product.db)             ↓        Admin Dashboard (Content / Product Management) 

---

## Project Structure

text project-root/ │ ├── admin/                 # Admin dashboard ├── css/                   # Shared styles ├── db/                    # SQLite database │ ├── index.html             # Homepage ├── products.html          # Product list page ├── product-detail.html    # Product detail page │ ├── server.py              # Flask backend server ├── main.js                # Homepage interaction logic ├── product.js             # Product rendering & API interaction ├── admin.js               # CMS management logic │ └── README.md 

---

## API Example

### Get Product List

http GET /api/products 

### Get Published Products

http GET /api/products?status=上架 

### Create Product

http POST /api/products 

### Update Product

http PUT /api/products/<id> 

### Delete Product

http DELETE /api/products/<id> 

---

## Key Functionalities

### Dynamic Product Rendering
Products are loaded dynamically from backend APIs instead of hardcoded HTML content.

javascript fetch('/api/products?status=上架') 

This allows the frontend website to synchronize automatically with backend-managed content.

### Product Category Filtering
Users can filter products by category through frontend interaction logic.

### CRUD Workflow
The admin dashboard supports content management workflows such as:

- Create products/articles
- Edit existing content
- Delete records
- Update product status
- Organize website content

### Dashboard Management
The admin system includes a lightweight CMS-style interface for website operation and content maintenance.

---

## What I Learned

Through this project, I gained hands-on experience with:

- Frontend and backend integration
- Building lightweight CRUD systems
- REST-style API communication
- SQLite data persistence
- Dynamic frontend rendering
- Admin dashboard workflow design
- Website maintainability and content organization
- Practical prototype development

I also learned how business websites manage structured product information, synchronize frontend pages with backend systems, and maintain scalable content workflows.

---

## Limitations

This project is designed as a lightweight prototype for workflow simulation and learning purposes.

Some production-level features such as authentication security, cloud deployment, and permission control are simplified.

Future improvements may include:

- User authentication system
- Cloud deployment support
- Rich text editor integration
- Image upload optimization
- Search and analytics functionality
- More scalable database architecture

---

## Run Locally

### 1. Clone Repository

bash git clone https://github.com/Monroe01/company-website-cms.git 

### 2. Install Dependencies

bash pip install flask 

### 3. Run Server

bash python server.py 

### 4. Open Website

text Frontend: http://localhost:5000  Admin Dashboard: http://localhost:5000/admin 

---

## Motivation

This project was built to explore how a practical business website system works beyond static pages.

Instead of building a frontend-only website, I wanted to understand:

- How frontend and backend interact
- How data persistence works
- How CRUD systems support content workflows
- How lightweight internal management systems are designed

The goal was to move from static website development toward building usable and maintainable application prototypes.
