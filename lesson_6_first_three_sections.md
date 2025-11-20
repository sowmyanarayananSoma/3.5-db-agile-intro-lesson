# 🧭 Lesson 6 — Intro to Databases
## **Back-End Development**
This document covers the first three sections of today’s lesson:
1. **Recap** (Servers & APIs)  
2. **Infrastructure of the Web**  
3. **Databases Introduction**

Use this as your teaching guide and student reference.

---

## 🔁 1. Recap — Servers & APIs (10 minutes)
A quick warm‑up to connect previous lessons with today’s database topics.

### **What is a server?**
A computer that listens for requests and sends back responses.

### **What is an API?**
An interface/communication methodology that allows clients (like browsers) to communicate with servers.

### **Simple Request/Response Flow:**
```
Client (Browser) → API → Server → Database (optional) → Response → Client
```

### **Why recap this?**
Before we learn where data is stored, students must remember **how data travels**.

---

## 🏗️ 2. Infrastructure of the Web (20 minutes)
Today students learn **how the database fits into the full web system**.

### **Client → Server → Database Architecture**
```
[ Client ] → sends request
[ Server ] → processes request, applies logic
[ Database ] → stores & retrieves data
```

### **What each part does:**
- **Client** — Browser, mobile app, desktop app
- **Server** — Backend code that decides what to do
- **Database** — Stores long‑term information

### **Common Tech Stacks**
Introduce common combinations:
- **LAMP** — Linux, Apache, MySQL, PHP
- **LEMP** — Linux, Nginx, MySQL, PHP
- **MEAN** — MongoDB, Express, Angular, Node
- **MERN** — MongoDB, Express, React, Node

### **Key Point for Students**
> All modern web apps follow this pattern: a client, a backend, and a database working together.

This sets the foundation for understanding databases.

---

## 🗄️ 3. Introduction to Databases (40 minutes)
This section helps students understand **why databases exist and how data is stored**.

---

### 3.1 What is a Database? (5 minutes)
A database is a **structured system for storing information** so that applications can retrieve it later.

Examples of stored information:
- Users
- Messages
- Orders
- Notes
- Products

---

### 3.2 Why Databases Are Important (5 minutes)
Almost every app needs to **remember things**.

Examples:
- Instagram remembers your posts
- Uber saves ride history
- Netflix saves your watch list
- A note app stores your notes

Applications without databases cannot store user data.

---

### 3.3 Types of Databases (15 minutes)
Start from the simplest forms to real databases.

### **Basic Data Storage Types:**
- JSON files
- CSV files
- Spreadsheets

Explain that these **store data**, but are limited.

### **Relational Databases (SQL)**
Structured, table‑based systems:
```
Users Table
----------------------
id | name | email
1  | Alex | alex@mail.com
```
Used when relationships matter.

### **SQL Concepts (High Level):**
- Tables
- Rows
- Columns
- Queries (SELECT, INSERT, UPDATE, DELETE)

---

### 3.4 NoSQL Databases (15 minutes)
A more flexible approach.

### **NoSQL = Not Only SQL**
Stores data in JSON‑like documents.

Example (MongoDB):
```json
{
  "id": 1,
  "title": "My First Note",
  "tags": ["school", "urgent"],
  "completed": false
}
```

### **Why Developers Use NoSQL?**
- Flexible structure
- Easy to scale
- Great for apps with changing data shapes

---

## 🛠️ 4. CRUD Operations (20 minutes)
CRUD represents the four fundamental operations that applications perform on data.

### **What is CRUD?**
CRUD stands for:
- **C – Create** → Add new data
- **R – Read** → Retrieve existing data
- **U – Update** → Modify existing data
- **D – Delete** → Remove data

These actions map directly to both **databases** and **HTTP methods**.

---

### **CRUD in Real Applications**
| CRUD | App Example | Database Action | HTTP Verb |
|------|-------------|-----------------|-----------|
| **Create** | Creating a new Instagram post | INSERT | POST |
| **Read** | Loading your feed | SELECT | GET |
| **Update** | Editing your profile | UPDATE | PUT/PATCH |
| **Delete** | Deleting a comment | DELETE | DELETE |

---

### **Why CRUD Matters**
CRUD is the foundation of almost every software application:
- Social media apps (posts, likes, comments)
- Banking apps (transactions, balances)
- Note‑taking apps (notes, folders)
- Shopping apps (products, carts, orders)

Understanding CRUD prepares students for full‑stack development.

---

### **High‑Level Examples**
**Create:**
```sql
INSERT INTO users (name, email) VALUES ("Alex", "alex@mail.com");
```
**Read:**
```sql
SELECT * FROM users;
```
**Update:**
```sql
UPDATE users SET name = "Alicia" WHERE id = 1;
```
**Delete:**
```sql
DELETE FROM users WHERE id = 1;
```

---

## 🎯 Summary of First Three Sections
By this point students should understand:
- How the client → server → database flow works
- Why databases are essential
- Difference between SQL and NoSQL
- Basic data storage concepts (JSON, CSV, spreadsheets)

These concepts prepare them for the next section on **CRUD operations** and later for **building full‑stack apps**.

---

