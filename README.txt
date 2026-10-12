# City Library System 📚🏛️

A comprehensive library management web application built as part of Software Engineering studies at Afeka College. The system consists of multiple modular mini-apps handling patron services, librarian management, and room reservations.

---

## 🏗️ Architecture & Mini-Apps (Client-Side - React)
The frontend is split into 3 distinct React mini-apps:
1. **Librarian Mini-app:** Manages book inventories, user tracking, and administrative controls.
2. **Patron Mini-app:** Allows library members/patrons to browse and interact with library services.
3. **Rooms Mini-app:** Handles study/library room reservations.

> **💡 Port Configuration:** 
> By default, the client-side apps are configured to run on **Ports 3000, 3001, and 3002**. 
> *If you encounter port conflicts or environment issues, you can easily switch back to the default **Port 3000** by following the instructions in the individual `README.md` file located inside each project folder.*

---

## 🗄️ Database & Data Initialization (`Book`, `Room`)

The database manages core entities including **`Book`** and **`Room`**:

- **Rooms Management:** 
  - Room reservation requires pre-existing `Room` objects in the database to handle the room reservation mini-app.
  - Rooms were initially populated using **Swagger (`POST` requests)**. Note that adding new rooms cannot be done directly through the client-side interface.
- **Books Management:** 
  - `Book` objects are added dynamically using the **Librarian Mini-app**.
  - Librarians can add books directly to the database via the API integration (`ManageBooks` -> `Add Books`), supporting multiple methods for data entry.

---

## ⚙️ How to Run
1. Navigate to each mini-app directory (Librarian, Patron, Rooms).
2. Check the local `README.md` inside each folder for specific setup and port instructions.
3. Install dependencies:
   ```bash
   npm install
