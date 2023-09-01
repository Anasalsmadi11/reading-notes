# Login  and Auth 

## [What is Role Based Access Control (RBAC)?](https://www.digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)




### What is Role Based Access Control (RBAC)?

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control.


### Share some an example of RBAC including all possible CRUD operations and correlating roles.

Through RBAC, you can control what end-users can do at both broad and granular levels. You can designate whether the user is an administrator, a specialist user, or an end-user

What if an end-user's job changes? You may need to manually assign their role to another user, or you can also assign roles to a role group or use a role assignment policy to add or remove members of a role group.

Some of the designations in an RBAC tool can include:

* Management role scope – it limits what objects the role group is allowed to manage.

* Management role group – you can add and remove members.
* Management role – these are the types of tasks that can be performed by a specific role group.
* Management role assignment – this links a role to a role group.


### What are the Benefits of RBAC?

 Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization.

 1. Reducing administrative work and IT support. 
 1. Maximizing operational efficiency.
 1. Improving compliance.

 ### Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.


## [react-cookie library](https://www.npmjs.com/package/react-cookie)

## [react-cookies component](https://www.npmjs.com/package/react-cookies)




### Describe some react-cookie features.

#### const [cookies, setCookie, removeCookie] = useCookies(['cookie-name']);

#### useCookies([dependencies])

1. dependencies (optional): Let you optionally specify a list of cookie names your component depend on or that should trigger a re-render. If unspecified, it will render on every cookie change.

1. setCookie(name, value, [options]): sets acookie value

    * name (string): cookie name
    * value (string|object): save the value and stringify the object if needed

    * options (object): Support all the cookie options from RFC 6265


1. removeCookie(name, [options])

    * name (string): cookie name
   
    * options (object): Support all the cookie options from RFC 6265


1. updateCookies(): Read back the cookies from the browser and triggers the change listeners. This should normally **not be necessary** because this library detects cookie changes automatically.

1. withCookies(Component): Give access to your cookies anywhere. Add the following props to your component:

    * cookies: Cookies instance allowing you to get, set and remove cookies.
    * allCookies: All your current cookies in an object.


1. 
### Describe some react-cookies features.

1. load(name, [doNotParse]): Load the cookie value.
Returns undefined if the cookie does not exist.

    * name: 
        
        * type: string
        * Required 

    * doNotParse

        * Type: boolean
        * Default: fals

1. loadAll(): 

Load all available cookies.

1. select([regex])
Find all the cookies with a name that match the regex.
Returns an object with the cookie name as the key.

1. .save(name, value, [options])

    * name

        * Type: string
        * Required

    * value
    
        * Type: string||number||
        * object
        * Required

1. options
Support all the cookie options from the RFC 6265.

    * Type: object 


### Which library would you prefer would you prefer? Why?

 I'd lean towards react-cookie for a few reasons:

 1. Community and Maintenance: react-cookie had a more active community and was regularly maintained. 

 1. Features: react-cookie seemed to have a more extensive feature set, which can be beneficial if I need to implement advanced cookie-related functionality. 

 1. Documentation: I found the documentation for react-cookie to be well-structured and easy to follow.
