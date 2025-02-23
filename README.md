# **Ordering Microservice – Spring Boot**

## 📌 **Overview**
This is an **Ordering Microservice** built using **Spring Boot**, designed for a Blinkit-like platform. It handles **order placement, fetching order details, order history, and invoice generation** while interacting with other microservices.

## 🏰️ **Tech Stack**
- **Java 23**
- **Spring Boot** (Web, JPA)
- **Spring MVC** – Handles HTTP requests
- **Spring Data JPA** – Database interactions
- **PostgreSQL** – Data storage
- **REST API** – Uses `RestTemplate` for communication

## 🛠️ **Key Features**
✅ **Order Management** – Place and track orders
✅ **Fetching Order Details** – Retrieve order information
✅ **Microservices Communication** – Calls **Cart Service, Pricing Service, Identity Service, Inventory Service, and Payment Service**
✅ **Error Handling** – Ensures smooth request processing
✅ **Invoice Generation** – Creates invoices for orders

---

## 🚀 **How to Run Locally**

### **1⃣ Clone the Repository**
```bash
git clone https://github.com/jyotiradityaraghuvanshi/OrderHub.git
cd OrderHub
```

### **2⃣ Set Up PostgreSQL**
- Install and start PostgreSQL.
- Create a database for the application.
- Configure your database credentials in `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/YOUR_DATABASE
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

### **3⃣ Run the Application**
```bash
mvn spring-boot:run
```

---

## 📂 **API Endpoints**

| Method  | Endpoint               | Description                          |
|---------|------------------------|--------------------------------------|
| **POST** | `/orders`             | Create a new order                  |
| **GET**  | `/orders/{id}`        | Get order details                   |
| **GET**  | `/orders/history`     | Fetch order history                 |
| **POST** | `/orders/{id}/invoice` | Generate an invoice for an order    |

---
