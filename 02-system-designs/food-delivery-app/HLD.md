	# High-Level Design: Food Delivery App (Swiggy/Zomato)

## 1. Requirements
- Customers browse restaurants & order food
- Restaurants update menu
- Delivery partners accept & deliver orders
- Real-time order tracking
- Payments (COD + Online)

## 2. High-Level Architecture
- Client (Web/Mobile App)
- API Gateway
- Microservices:
  - User Service
  - Restaurant Service
  - Order Service
  - Delivery Service
  - Payment Service
- Database:
  - Relational DB for transactions
  - NoSQL DB for menus
- Messaging Queue (Kafka/SQS) for order events
- CDN for images
- Notifications Service (SMS/Push)

## 3. Scalability Considerations
- Caching (Redis) for frequently accessed data
- Load Balancer for API servers
- DB sharding by region
- Asynchronous processing for delivery updates
![Food Delivery HLD](./diagrams/hld.png)
