# Overview
[ittovate organization](https://github.com/ittovate)
- demo-otp-service.
- demo-db-to-kafka-to-db.
- demo-mongo-crud.
- demo-redis-crud.
- demo-cassandra-crud.
- demo-batch-processing.
- demo-email-sender.
- demo-email-listener.
- demo-kafka.
- demo-stripe-manager.
- demo-chatbot.
# Learning Outcomes
- Standardize code (e.g. Logging, Exception Handling)
- Apply code quality (Checkstyle & SonarLint & pre-commit hooks) 
- Manage application secrets
- Add Unit/Integration tests.
- Write Documentation
- Use CI Workflow pipeline.
- Understand technologies documentations.
- Apply Authentication & authorization.
# Challenges
- Standardize Code.
- Apply Git & GitHub best practices.
- demo-otp-service
	- Using `RedisTemplate` vs Spring Data Redis which had some issues with expiration [Salesforces faced a similar issue](https://engineering.salesforce.com/lessons-learned-using-spring-data-redis-f3121f89bff9/).
- demo-batch-processing
	- **Restartability issues** especially with Spring Batch's design to not restart a job after it is completed
- demo-email-listener
	- Integration with Google Cloud and Gmail API
	- Using Spring Email IMAP protocol.
- demo-kafka
	- Setting up Schema Registry.
	- Creating Avro and its Serialization/Deserialization.
- demo-stripe-manager
	- Understanding payment gateway integration.
# Skills

| Team      | Skills                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Andrew    | ???<br>???<br>???                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Sabry     | AI, LLMs, Python, C#, Computer Vision                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Abuelmgad | Java, Javascript, Spring, Spring Boot, Spring Reactive, Spring Security, Redis, Kafka, Relational DB (Postgres), Non-Relational DB (MongoDB, Cassandra), Unit Testing, Mock Testing, Docker, Git & Github, Integration, Debugging, C#, Express JS, Static Code Analysis, SonarLint, Angular, React, Flutter, MySQL, SQLite, Github Actions, Ngrok, Reverse Proxy, AOP, Webclient, Authentication, Authorization, OAuth, API Development (REST) |
| Mohanad   | C/C++, Java ,Spring/Spring Boot/Spring Data/Spring Batch, Javascript/Typescript , Node.js/Express.js , Docker , Kafka , Git/Github, PostgreSQL, MySQL, MongoDB ,Redis, Unit Testing, Ngrok                                                                                                                                                                                                                                                                                                 |
| Hussein   | C++ , Java , Relational DB, Mongo DB , Unit testing, Kafka, Docker , HTML , CSS , Bootstrap                                                                                                                                                                                                                                                                                                                                                                                                |
| Al-Deeb   | C++, Java, JavaScript, Python.<br>Spring, Node.js, Django.<br>Relational DB, MongoDB.<br>Unit testing, Documentation. <br>Kafka, Docker, Git & GitHub, Problem Solving                                                                                                                                                                                                                                                                                                                     |
# What is next? 👀
