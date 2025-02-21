# Ordering Microservice – Spring Boot  

## 📌 Overview  
This is an **Ordering Microservice** built using **Spring Boot**, designed for a Blinkit-like platform. It handles **order placement, order history, and invoice generation** while interacting with other microservices.  

## 🏗️ Tech Stack  
- **Java 17**  
- **Spring Boot** (Web, JPA, Validation)  
- **REST API** with `RestTemplate`  
- **PostgreSQL** for data storage  

## 🔄 Key Features  
✅ **Order Management** – Place and track orders  
✅ **Microservices Communication** – Calls **Cart Service, Pricing Service, Identity Service, Inventory Service, and Payment Service**  
✅ **Error Handling** – Ensures smooth request processing  
✅ **Invoice Generation** – Creates invoices for orders  
## 🚀 How to Run Locally  
1. Clone the repository:  
   ```bash
   git clone https://github.com/jyotiradityaraghuvanshi/OrderHub.git
   cd orderHub

2. **Set up PostgreSQL**:  
   - Install and start PostgreSQL.  
   - Create a database for the application.  
   - Update the `application.properties` file with your database credentials:  

   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/your_database  
   spring.datasource.username=your_username  
   spring.datasource.password=your_password  
   spring.jpa.hibernate.ddl-auto=update  

3. **Run the application**:  
   - Open a terminal and navigate to the project directory.  
   - Run the following command to start the application:  

   ```bash
   mvn spring-boot:run

## 📂 API Endpoints  

| Method  | Endpoint               | Description                          |  
|---------|------------------------|--------------------------------------|  
| **POST** | `/orders`             | Create a new order                  |  
| **GET**  | `/orders/{id}`        | Get order details                   |  
| **GET**  | `/orders/history`     | Fetch order history                 |  
| **POST** | `/orders/{id}/invoice` | Generate an invoice for an order    |  
