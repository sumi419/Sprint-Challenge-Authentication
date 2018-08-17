<!-- Answers to the Short Answer Essay Questions go here -->

1.  Describe Middleware, Sessions (as we know them in express), bcrypt and JWT.

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next. Middleware is used to execute any code and make changes to the request and the response objects. In this project we used middleware to pass in generateToken and authenticaton that was needed in some of our routes.

Sessions allow us to use cookies and this can be a way to keep track of users logged in without using JWT or tokens. A session is a place to store data that you want access to across requests. Each user that visits your website has a unique session. You can use sessions to store and access user data as they browse your application. Sessions allow the application to store state.

Bcrypt is a password hashing function and it is used to protect users and keep their passwords secure.

A JSON Web Token (JWT) is a JSON object that is defined in RFC 7519 as a safe way to represent a set of information between two parties. The token is composed of a header, a payload, and a signature.

2.  What does bcrypt do in order to prevent attacks?

It hashes the password into a string before saving it to the database. Hashing performs a one-way transformation on a password, turning the password into another String, called the hashed password. That way the only person with access to the password is the user.

3.  What are the three parts of the JSON Web Token?

Header, Payload, Signature
