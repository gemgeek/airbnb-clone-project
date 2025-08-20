# AirBnB Clone Project

## 📌 Project Overview
This is a full-stack clone of the popular accommodation booking platform **Airbnb**.  
The goal is to build a functional web application that allows users to:
- Browse property listings
- View detailed property information
- Complete bookings securely

## 🎯 Project Goals
- Learn to implement responsive UI/UX designs
- Understand how to structure a complex web application
- Develop skills in component-based frontend architecture
- Gain experience working in a collaborative team environment
- Practice best practices in modern web development

## 🛠️ Tech Stack
**Frontend:** HTML, CSS, JavaScript (React)  
**Backend:** Node.js / Express (planned)  
**Database:** PostgreSQL / MongoDB (planned)  
**Version Control:** Git and GitHub  
**Design Tools:** Figma  
**Deployment:** To be decided (Netlify / Vercel / Heroku)

## 📂 Repository Structure
- `README.md` – Project overview and documentation  
- Future folders: `/frontend`, `/backend`, `/design`  

## 🎨 UI/UX Design Planning

### ✅ Design Goals
- Create an **intuitive booking flow** that is easy for users to follow  
- Maintain **visual consistency** across all pages  
- Ensure **fast loading times** for a smooth user experience  
- Prioritize **mobile responsiveness** (mobile-first design)  

### ⭐ Key Features
- **Property search and filtering**  
- **Detailed property viewing** with images and descriptions  
- **Secure checkout process** for bookings  
- **User authentication** (sign up / login)  

### 📄 Primary Pages

| Page | Description |
|------|-------------|
| **Property Listing View** | Displays available properties in a grid layout with filters (price, location, rating). |
| **Listing Detailed View** | Shows complete property details with multiple images, amenities, location map, and booking form. |
| **Simple Checkout View** | Streamlined page for secure payment and booking confirmation. |

### 💡 Importance of User-Friendly Design
A well-designed booking system reduces friction in the user journey, increases conversion rates, and improves customer satisfaction. Clear navigation, intuitive interfaces, and responsive design are critical for success.


### 🎨 Design Properties (from Figma)

#### 🎨 Color Styles
- **Primary Color:** Green (#008489)  
- **Secondary Color:** Yellow  
- **Secondary Text / Black:** #000000  
- **Shimmer / Gray:** Gray  

#### ✍️ Typography
- **Font Family:** Source Sans Pro  
- **Font Weights:** Regular (400), Medium (500), Bold (700)  
- **Font Sizes:**  
  - Body text: 14px – 16px  
  - Headings: 24px – 32px  

### 💡 Why Identifying Design Properties Matters
Identifying color styles and typography early in the design process helps to:  
- Maintain **visual consistency** across the application  
- Ensure the design matches the **brand identity**  
- Make collaboration between designers and developers smoother  
- Speed up development by using a **design system** (reusable styles and components)  


## 👥 Project Roles and Responsibilities

### 📌 Roles and Their Contributions

#### 🗂️ Project Manager
- Oversees the project timeline and deliverables  
- Coordinates tasks across the team  
- Ensures milestones are met on schedule  

#### 💻 Frontend Developers
- Build and implement the user interface using React, HTML, CSS, and JavaScript  
- Ensure the design is responsive and accessible  
- Integrate frontend with backend APIs  

#### ⚙️ Backend Developers
- Build and maintain the application’s server, APIs, and database  
- Implement business logic and data handling  
- Ensure performance, security, and scalability  

#### 🎨 Designers
- Create mockups and maintain the design system (colors, typography, components)  
- Ensure a user-friendly experience  
- Collaborate closely with developers to align design and implementation  

#### 🧪 QA/Testers
- Write test cases (unit, integration, end-to-end)  
- Test application features for bugs or issues  
- Report issues and verify fixes before deployment  

#### 🔧 DevOps Engineers
- Set up and manage deployment environments  
- Create CI/CD pipelines for continuous delivery  
- Monitor servers and application uptime  

#### 📋 Product Owner
- Define project requirements and user stories  
- Prioritize features based on user needs and business goals  
- Act as the link between the team and stakeholders  

#### 🔄 Scrum Master
- Facilitate agile processes (daily standups, sprint planning, retrospectives)  
- Remove blockers to keep the team productive  
- Ensure smooth communication and workflow within the team  


## 🧩 UI Component Patterns

To ensure consistency and reusability across the project, we will use a **component-based architecture**.  
Below are the planned UI components:

### 🔝 Navbar
- Contains the **logo**, **search bar**, and **user navigation**  
- Includes a **responsive menu** for mobile devices  
- Provides quick access to major sections of the site  

### 🏡 Property Card
- Displays **property image** and **basic details** (price, location, rating)  
- Includes a **favorite button** for saving properties  
- Designed with a responsive layout for grid and mobile views  

### 📄 Footer
- Displays **site links** (About, Contact, Help)  
- Includes **company information** and **social media links**  
- Shows **copyright information**  

---


# ⚙️ ProDev Back-end

This section documents the planning and development of the back-end part of the AirBnB Clone project.

# 👥 Team Roles

In this project, several team roles ensure smooth collaboration and development:

- **Backend Developer**: Builds the application logic, APIs, and connects the frontend with the database.  
- **Database Administrator (DBA)**: Designs, manages, and optimizes the database to ensure data integrity and performance.  
- **Frontend Developer**: Implements the user interface and integrates with the backend APIs.  
- **Designer (UI/UX)**: Creates the layouts, wireframes, and ensures the application is user-friendly.  
- **QA/Testers**: Write and execute tests, find bugs, and ensure quality before release.  
- **DevOps Engineer**: Manages deployments, CI/CD pipelines, and infrastructure.  
- **Project Manager**: Organizes the team, tracks progress, and ensures deadlines are met.  
- **Scrum Master**: Facilitates Agile practices, removes blockers, and supports the team’s workflow.  
- **Product Owner**: Defines project goals, prioritizes features, and represents user needs.  


# 🛠 Technology Stack

Our AirBnB Clone project leverages a set of powerful technologies that work together to deliver a robust and scalable application:

- **Django**: A high-level Python web framework used for building the backend and RESTful APIs. It handles business logic, routing, and integrates with the database.  
- **PostgreSQL**: A reliable and powerful relational database system that stores application data such as users, bookings, and properties.  
- **GraphQL**: An API query language that allows flexible data fetching, enabling the frontend to request exactly what it needs.  
- **HTML/CSS/JavaScript**: Core web technologies for building and styling the user interface.  
- **React (optional)**: A modern JavaScript library that can be used for building dynamic frontend components.  
- **Docker**: Containerization tool to ensure consistent environments and simplify deployment.  
- **Git & GitHub**: Version control and collaboration platform for managing source code.  


# 🗄 Database Design

The AirBnB Clone project requires several core entities to manage users, properties, and reservations. Below is an overview of the key entities and their relationships:

### Entities and Fields
- **Users**
  - `id` (Primary Key)
  - `name`
  - `email`
  - `password`
  - `role` (guest, host, admin)

- **Properties**
  - `id` (Primary Key)
  - `title`
  - `description`
  - `location`
  - `price_per_night`
  - `host_id` (Foreign Key → Users)

- **Bookings**
  - `id` (Primary Key)
  - `user_id` (Foreign Key → Users)
  - `property_id` (Foreign Key → Properties)
  - `check_in_date`
  - `check_out_date`
  - `status` (pending, confirmed, canceled)

- **Reviews**
  - `id` (Primary Key)
  - `user_id` (Foreign Key → Users)
  - `property_id` (Foreign Key → Properties)
  - `rating`
  - `comment`

- **Payments**
  - `id` (Primary Key)
  - `booking_id` (Foreign Key → Bookings)
  - `amount`
  - `payment_method`
  - `status` (successful, failed, pending)

### Relationships
- A **User** can list multiple **Properties** (1-to-many).  
- A **User** can make multiple **Bookings** (1-to-many).  
- A **Property** can have many **Bookings** (1-to-many).  
- A **Property** can have many **Reviews**, each left by a different User (1-to-many).  
- Each **Booking** is linked to exactly one **Payment** (1-to-1).  


# ✨ Feature Breakdown

The AirBnB Clone project will include several core features that replicate the functionality of the Airbnb platform. Each feature contributes to delivering a complete user experience.

### 1. User Management
Allows users to create accounts, log in, and manage their profiles. This feature ensures secure authentication and supports both guests (renters) and hosts (property owners).

### 2. Property Management
Hosts can add, update, and remove property listings. This feature provides detailed property information such as descriptions, amenities, pricing, and availability.

### 3. Booking System
Enables guests to search for properties, view availability, and make reservations. This feature manages check-in and check-out dates, booking status, and prevents scheduling conflicts.

### 4. Review System
Guests can leave reviews and ratings for properties they’ve stayed at. This builds trust in the platform and helps future guests make informed decisions.

### 5. Payment Integration
Supports secure payment processing for bookings. This feature ensures that hosts are paid and guests are charged accurately, with support for multiple payment methods.

### 6. Search and Filtering
Allows users to search for properties by location, price, dates, and other filters. This feature improves usability by helping guests quickly find the most relevant listings.

### 7. Admin Dashboard (optional extension)
Provides administrators with tools to monitor activity, manage users, and ensure the platform is running smoothly.


## API Security

To protect the integrity of the AirBnB Clone backend, several key security measures will be implemented:

- **Authentication**: Verifies the identity of users before granting access. This ensures that only legitimate users can log in and interact with the system, protecting user accounts and personal data.

- **Authorization**: Defines what authenticated users are allowed to do. For example, property owners can manage their listings, while guests can make bookings. This prevents unauthorized actions within the system.

- **Rate Limiting**: Controls the number of requests a user or client can make in a given timeframe. This helps protect against abuse, such as denial-of-service (DoS) attacks or brute-force login attempts.

- **Data Encryption**: All sensitive data (like passwords and payment information) will be encrypted both in transit (via HTTPS/TLS) and at rest. This secures critical information from being exposed if intercepted.

- **Input Validation**: Ensures that any data received by the API is clean and expected, helping defend against SQL injection, cross-site scripting (XSS), and other malicious attacks.

### Why Security is Crucial

- Protects sensitive **user data** (personal information, login credentials).  
- Secures **payments and transactions** against fraud.  
- Maintains the **trustworthiness** of the platform by preventing unauthorized access or malicious activity.  
- Ensures compliance with data protection standards and regulations.


## CI/CD Pipeline

A **CI/CD pipeline** (Continuous Integration and Continuous Deployment) is a set of automated processes that help developers deliver code changes more reliably and efficiently.  

- **Continuous Integration (CI)**: Ensures that new code changes are automatically tested and integrated into the project. This reduces bugs and helps catch errors early in development.  
- **Continuous Deployment (CD)**: Automates the release process so that tested changes can be quickly and safely deployed to production.  

### Why CI/CD is Important
- Speeds up development by automating testing and deployment.  
- Reduces human error by standardizing the release process.  
- Ensures high-quality code is always ready to be deployed.  
- Provides faster feedback to developers when something breaks.  

### Tools We Could Use
- **GitHub Actions**: Automates workflows for building, testing, and deploying the project directly from GitHub.  
- **Docker**: Ensures consistent environments across development, testing, and production.  
- **Jenkins**: A widely used automation server for managing CI/CD pipelines.  
- **Kubernetes** (optional, for scaling): Helps manage and deploy applications in containers at scale.  

### Example GitHub Actions Workflow

Here’s a simple CI workflow (`.github/workflows/ci.yml`) that runs whenever code is pushed to the repo:

```yaml
name: CI Pipeline

on: [push, pull_request]

jobs:
  build:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Set up Python
        uses: actions/setup-python@v4
        with:
          python-version: '3.10'

      - name: Install dependencies
        run: |
          python -m pip install --upgrade pip
          pip install -r requirements.txt

      - name: Run tests
        run: |
          pytest

          
---
🚀 *This project is part of the ProDev Full-Stack Development course.*