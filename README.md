Money transfer Rest API

A Java RESTful API for money transfers between users accounts.

Technologies:

JAX-RS API
H2 in memory database
Log4j
Jetty Container (for Test and Demo app)
Apache HTTP Client


How to run:
Execute this command > 
mvn exec:java

Application starts a jetty server on localhost port 8080 An H2 in memory database 
initialized with some sample user and account data To view.

http://localhost:8080/user/test1


http://localhost:8080/user/test2


http://localhost:8080/account/1


http://localhost:8080/account/2


Http Status:

200 OK: The request has succeeded
400 Bad Request: The request could not be understood by the server 
404 Not Found: The requested resource cannot be found
500 Internal Server Error: The server encountered an unexpected condition 

Sample JSON for User and Account:

User:
{  
  "userName":"test1",
  "emailAddress":"test1@gmail.com"
} 
User Account:
{  
   "userName":"test1",
   "balance":10.0000,
   "currencyCode":"GBP"
}
User Transaction:
{  
   "currencyCode":"EUR",
   "amount":100000.0000,
   "fromAccountId":1,
   "toAccountId":2
}



Thank you.
