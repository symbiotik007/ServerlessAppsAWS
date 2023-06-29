# ServerlessAppsAWS
Build, Secure, Manage Serverless Applications at Scale on AWS

Cloud Infrastructure: 

![image](https://github.com/symbiotik007/ServerlessAppsAWS/assets/69918011/49cecc35-4df9-4af7-92a5-2c88aff34958)

Our orders microservice is composed of the following resources:

/orders: This resources allows users to list their orders and create new ones

GET: List orders - API Gateway -> Lambda -> DynamoDB
POST: Create New Order - API Gateway -> SQS -> Lambda -> DynamoDB
/orders/{id}: Users can call this resource to show their order details

GET: Show order details - API Gateway -> Lambda -> DynamoDB
PUT: Update order status - API Gateway -> Lambda -> DynamoDB
DELETE: Cancel order - API Gateway -> Lambda -> DynamoDB
