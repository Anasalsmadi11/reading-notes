# API Integration

##[Review API Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/)




### Explain the different between a query string parameter and a path parameter.

Query string parameters and path parameters are two common ways to pass data to a web server when making HTTP requests.

**Path Parameters:**

* Location: Path parameters are part of the URL's path itself.
* Format: They are typically enclosed within curly braces {} or identified by a specific structure in the URL path.
* Purpose: Path parameters are used to specify variable values within the URL path, allowing you to identify a specific resource or endpoint.

* Example: In the URL "https://example.com/users/{userID}", "{userID}" is a path parameter, and it represents a dynamic value that can change, such as "https://example.com/users/123".



**Query String Parameters:**

* Location: Query string parameters are appended to the end of the URL after a question mark "?".

* Format: They are represented as key-value pairs, separated by "&" and using the format "key=value".
* Purpose: Query string parameters are used to send additional data to the server as part of the request. They are commonly used for filtering, sorting, or providing optional parameters.
* Example: In the URL "https://example.com/search?query=term&page=2", "query" and "page" are query string parameters, and they provide additional information to the server for a search operation.

### What would our API URL with a path id parameter be given the following information:
Domain: http://our-site.com

v3

model name: stuff

id: things


the URL would typically follow this pattern:

http://our-site.com/v3/model-name/{id}


### We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.


think of a dynamic API with an "interface" as a menu for computers. It shows you how to ask for things from a computer system. You don't need to know the technical stuff; you just follow the menu's instructions to get what you want. It's like ordering food in a restaurant without needing to be a chef.  

## [Review Auth Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/)




### Describe how you would use middleware to implement basic and bearer auth.

**Basic Authentication:**

* Use middleware to check for a username and password in the request headers.

* Validate the credentials against your database.
* If valid, allow access; otherwise, deny with a 401 Unauthorized response.

**Bearer Authentication:**

* Employ middleware to extract a token from the request headers.

* Verify the token's validity (e.g., check expiration).
* If valid, grant access; otherwise, deny with a 401 Unauthorized response.

### Describe the handshake necessary to implement OAuth.


* Client Registration: The client app registers with the OAuth service.

* **Authorization Request:** The client asks the user to log in and grant permission.

* **User Authentication:** The user logs in and approves access.

* **Authorization Grant:** The server generates an access token.

* **Accessing Resources:** The client uses the token to access user data.

* **Token Refresh (Optional):** If needed, the client can get a new token.

### Describe how Role Based Access Control works to a non-technical friend.


"Role-Based Access Control (RBAC) is like assigning roles in a game or permissions in a building. Each role has specific abilities or access levels. People or characters get a role, and they can only do what that role allows. It keeps things organized and secure."