#  Access Control (ACL)

## [5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

### What is Role Based Access Control (RBAC) and why do we care?

RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

### Describe a Role/Permission heirarchy that you might implement using RBAC.

like the capapilities that an dmin have and the user not
### What approach might you take to implement RBAC?

1. Identify Roles: Identify the different roles that exist within your system or organization. 
1. Determine Permissions: Determine the permissions or actions that each role needs to perform their job effectively. 

1. Group Permissions into Roles: Group related permissions together to create roles. 

1. Assign Users to Roles: Assign individual users or employees to the appropriate roles based on their job responsibilities.
1. Implement Access Control: Implement access control mechanisms based on the assigned roles.
1. Enforce Access Control: Implement mechanisms to enforce access control decisions. 
1. Regularly Review and Update: Periodically review and update the roles, permissions, and user assignments as your organization evolves.

## [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

### If Authentication is “you are who you say you are,” what is Authorization?

Authorization is the process of determining what actions or resources an authenticated user is allowed to access or perform. While authentication verifies the identity of a user, authorization focuses on granting or denying access rights based on the user's identity and associated permissions.

### Name three primary rules defined for RBAC.

1. Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.

2. Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.

2. Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

### Describe RBAC to a non-technical friend.

For example, let's say we have three roles in a company: manager, team lead, and employee. The manager role might have permissions to access sensitive information, make important decisions, and manage teams. The team lead role might have permissions to access specific resources and supervise a team. And the employee role might have permissions to access basic resources and perform regular tasks.

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

### What Are access rights Associated with? The User? or The Role? Explain.

Access rights in RBAC are associated with roles rather than individual users. 
When users are assigned to roles, they inherit the access rights associated with those roles. This means that all users within a specific role have the same set of permissions.    
### Access Rights, or Authorization, is activated after a user successfully does what?

Access rights, or authorization, is activated after a user successfully undergoes the process of authentication. 

### Explain how RBAC might benefit a business.
1. Improved Security: RBAC helps enhance security by ensuring that users only have access to the resources and actions they need to perform their job functions. 

1. Access Control Simplification: RBAC simplifies access control management by organizing permissions into roles. 

1. Scalability and Flexibility: RBAC provides a scalable and flexible framework for managing access control as an organization grows or changes. 

2. Regulatory Compliance: RBAC helps businesses comply with regulatory requirements and industry standards.