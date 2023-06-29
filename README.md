# ServerlessAppsAWS
Build, Secure, Manage Serverless Applications at Scale on AWS

Cloud Infrastructure: 

<img>https://static.us-east-1.prod.workshops.aws/public/39f3bd8a-235f-4f3c-a23a-e49064f9d420/static/3-orderservice/images/order-arc-v6-cognito.png</img>

Our orders microservice is composed of the following resources:

/orders: This resources allows users to list their orders and create new ones

GET: List orders - API Gateway -> Lambda -> DynamoDB
POST: Create New Order - API Gateway -> SQS -> Lambda -> DynamoDB
/orders/{id}: Users can call this resource to show their order details

GET: Show order details - API Gateway -> Lambda -> DynamoDB
PUT: Update order status - API Gateway -> Lambda -> DynamoDB
DELETE: Cancel order - API Gateway -> Lambda -> DynamoDB
