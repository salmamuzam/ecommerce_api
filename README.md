# Aaliyah's Collection – Static JSON API

[![Platform](https://img.shields.io/badge/Platform-GitHub%20Pages-black?logo=github)](https://salmamuzam.github.io/ecommerce_api/)
[![Data Format](https://img.shields.io/badge/Data-JSON-lightgrey?logo=json)](https://json.org)

This repository serves as the **External Data Source** for the Aaliyah's Collection Mobile Application. It hosts structured JSON files via GitHub Pages to simulate a RESTful API environment, providing critical data for products, reviews, categories, and user mocks.

---

## 📖 Table of Contents
- [Project Purpose](#-project-purpose)
- [Available Endpoints](#-available-endpoints)
- [Technical Features](#-technical-features)
- [Data Schema Examples](#-data-schema-examples)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Folder Structure](#-folder-structure)

---

## 🎯 Project Purpose
The goal of this repository is to provide a reliable, globally accessible backend for the mobile application without the overhead of a full database server during development and testing.

- **High Availability:** Hosted on GitHub Pages for 99.9% uptime.  
- **Consistent Schemas:** Ensures the mobile app receives predictable data structures for seamless parsing.  
- **Easy Scalability:** New products or categories can be added by simply updating a JSON file.  

---

## 🌐 Available Endpoints
The base URL for all endpoints is: `https://salmamuzam.github.io/ecommerce_api/`

| Endpoint | Description |
| :--- | :--- |
| `product.json` | The master catalog containing all product details, prices, and media links. |
| `category.json` | Metadata for fashion categories (Abayas, Hijabs, Kaftans, etc.). |
| `review.json` | User-generated reviews, star ratings, and testimonials. |
| `user.json` | Mock user data used for testing profile and authentication layouts. |

---

## ✨ Technical Features
- **JSON Consistency:** All files follow a strict schema to prevent parsing errors in the Flutter app.  
- **Cross-Origin Ready:** Accessible by the mobile application from any network without CORS issues.  
- **Media Integration:** Contains direct links to assets hosted in the main mobile repository.  

---

## 📄 Data Schema Examples

### Product Sample
```json
{
  "id": 101,
  "name": "Classic Black Abaya",
  "price": "4500.00",
  "category_id": 1,
  "description": "Minimalist design with premium fabric...",
  "thumbnail": "https://raw.githubusercontent.com/salmamuzam/.../abaya.jpg"
}
```

### Review Sample
```json
{
  "id": 1,
  "product_id": 101,
  "username": "Salma",
  "rating": 5,
  "comment": "Perfect fit and very comfortable!"
}
```

---

## 🛠️ Tech Stack
- **Hosting:** GitHub Pages (Static Site Hosting)  
- **Data Format:** JSON (JavaScript Object Notation)  
- **Version Control:** Git  
- **Editor:** VS Code / Submarine  

---

## 🚀 Getting Started
To contribute or modify data:

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/salmamuzam/ecommerce_api.git
cd ecommerce_api
```

### 2️⃣ Update Content
Modify the `.json` files as needed.

### 3️⃣ Verify JSON
Ensure no trailing commas or syntax errors exist.

### 4️⃣ Push to Live
```bash
git add .
git commit -m "feat: update product stock and reviews"
git push origin main
```

---

## 📂 Folder Structure
```text
repository/
├── product.json     # Product Catalog List
├── category.json    # Category Metadata
├── review.json      # Product Reviews
├── user.json        # Test User Data
└── README.md        # API Documentation
```

