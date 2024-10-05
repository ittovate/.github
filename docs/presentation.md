# General
- Standardization
    - Unified API response throughout the application
    - Code quality using static analysis tools (Checkstyle)
    - Pre-commit hooks
- Secrets management (using Dotenv)
- Global Exception Handling
- Logging
- Swagger

# demo-otp-service
- Overview: 
    - An SMS token sending/verifying service that can be used for authentication/authorization purposes  
- Achievements: 
    - Send SMS to phones using Twilio and store the tokens on Redis for efficient lookups and custom expiration configuration 
    - Added a basic custom build workflow on Github Actions
- Challenges: 
    - Using RedisTemplate vs Spring Data Redis which had some issues with expiration [Salesforces faced a similar issue](https://engineering.salesforce.com/lessons-learned-using-spring-data-redis-f3121f89bff9/)
- Other demo ideas: 
    - Twilio provides a lot of APIs not just for phones , like voice, email, chat, and WhatsApp.
    - Can be used for 2FA

# demo-db-to-kafka-to-db
- Overview: 
    - 
- Achievements: 
    - 
- Challenges: 
    - 

# demo-mongo-crud
- Overview: 
    - 
- Achievements: 
    - 
- Challenges: 
    - 

# demo-redis-crud
- Overview: 
    - 
- Achievements: 
    - 
- Challenges: 
    - 

# demo-cassandra-crud
- Overview: 
    - thymleaf
    - data modeling
    - difference between relational database modeling and cassandra
    - datastax connection
- Achievements
    - created inbox app
    - login with google using spring security
- Challenges:
    - clustering vs partitioning key (revise )
    - thymleaf variables and attributes
    - differences between web-based spring boot and rest-based spring boot

# demo-batch-processing
- Overview: 
    - Batch processing demo using database,kafka readers and csv file writer
- Achievements: 
    - Successfuly run a job that reads from either the database or from kafka and process them even after failure it can be restarted from the last successful committed batch
- Challenges: 
    - **Restartability issues** especially with Spring Batch's design to not restart a job after it is completed 
- Other demo ideas: 
    - Could be used to batch process orders at a specific time e.g: (process all orders at 1 PM every day) 

# demo-email-sender
- Overview: 
    - An email sender that can send emails across different email platforms, including Gmail and Outlook.
- Achievements: 
    - Simultaneous Email Sending : Send emails to many recipients in a single action.
    - Multi-Client Compatibility : Supports Gmail, Outlook, and other email services.
- Challenges: 
    - Sending emails synchronously vs asynchronously

# demo-email-listener
- Overview: 
    - An email listener that can listen on an email provider like Gmail 
    - Implemented this demo in two different ways
        - A way that utilizes Gmail API 
        - A way that utilizes IMAP
- Achievements: 
    - Two demos that can listen on incoming emails and in one of them you can write your own logic of filtration, doing action on these emails
- Challenges: 
    - Integration with Google Cloud and Gmail API
        - Sensitive scopes and consent screen
        - Pubsub mechanisms (Push vs Poll)
        - Publisher using Gmail (Service account)
        - HistoryID flow
        - OAuth2 (without library)
    - Using IMAP and add an email listener to handle the incoming emails 

# demo-kafka
- Overview: 
    - Basic kafka producer,consumer demos for sending and receiving messages
- Achievements: 
    - Successfully send/receive messages with different formats String, JSON , Avro
    - Schema registry for centralization of models 
- Challenges: 
    - Setting up Schema Registry 
    - Creating Avro and its Serialization/Deserialization 

# demo-stripe-manager
- Overview: 
    - It's a platform that allows us to use their endpoints to create a payment method without needing to implement our own payment method endpoints
- Achievements: 
    - integrate with stripe
    - adding products in Stripe
    - creating payment links
    - handling invoices
- Challenges: 
    - swagger docs because of nested objects
    - business understanding
    - where to add products and prices(our database or stripes)
    - invoicing cycle
    - payment links
    - webhook understanding
    - how to pass and use nullable query params
# demo-chatbot
- Overview: 
    -
- Achievements: 
    - 
- Challenges: 
    -


