# FilteringAccessChainOfResponsibiliity
Chain of Responsibiliity Pattern Filtering Access

## Java Class :
* Middleware.java: Basic validation interface
* ThrottlingMiddleware.java: Check request amount limit
* UserExistsMiddleware.java: Check user’s credentials
* RoleCheckMiddleware.java: Check user’s role
* Server.java: Authorization target
* Demo.java: Client code

## Output with registered email and password :
```
Enter email: admin@example.com
Input password: admin_pass
Hello, admin!
Authorization have been successful!

or

Enter email: user@example.com
Input password: user_pass
Hello, user!
Authorization have been successful!
```

## Output  with wrong email and password:
```
Enter email: bukanadmin@example.com
Input password: IniPassword
This email is not registered!

or

Enter email: admin@example.com
Input password: IniPassword
Wrong password!
```
