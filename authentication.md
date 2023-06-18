#  Authentication

## [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)
### Explain to a non-technical friend how you would safely hash and store a password.

Hashing is a process that takes a password and transforms it into a fixed-length string of characters. The key thing about hashing is that it's a one-way process. This means that once a password is hashed, it's nearly impossible to reverse the process and obtain the original password. 

### What is Bcrypt?

Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.

### Why might you use something like Bcrypt?

1. Slowing down brute force attacks: Bcrypt is intentionally designed to be slow. 

2. Resistance against rainbow table attacks: A rainbow table is a precomputed table of password hashes and their corresponding plaintext passwords. 

3. Built-in salt generation: Bcrypt includes salt generation as part of the algorithm.

## [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)


### What is Basic Authentication?

 basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic credentials

### What properties are necessary in the header of a Basic Auth request?


In a Basic Authentication request, the necessary properties are included in the request header. The header must contain the following properties:

1. Authorization: This property specifies the authentication scheme being used, which is "Basic" in this case. It is followed by a space.

2. Base64-encoded credentials: After the space, the header should include the user credentials encoded in Base64 format. The credentials should be in the form of "username:password". The username and password are concatenated with a colon (":") between them.

### How are username:password in Basic Auth encoded?

 Encode the concatenated string using Base64 encoding. Base64 encoding converts the binary data into a set of ASCII characters. Each three bytes of binary data are converted into four ASCII characters.

## [OWASP auth cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

### Define the authentication process to a non-technical recruiter.

 Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

### How should your error messaging respond (both HTTP and HTML)? Why?

### Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

**HTTP Status Codes:** 

* 200 OK: This status code indicates a successful request.

* 4xx Client Errors: These status codes indicate that there was an error with the client's request. Examples include:

1. 400 Bad Request: The server couldn't understand the request due to invalid syntax or missing information.

2. 401 Unauthorized: The client needs to provide valid credentials to access the requested resource.

2. 403 Forbidden: The client does not have permission to access the requested resource.

2. 404 Not Found: The requested resource could not be found on the server.

**5xx Server Errors:**

1. 500 Internal Server Error: An unexpected error occurred on the server.

2. 503 Service Unavailable: The server is temporarily unable to handle the request.