# Exaple initial of Serving Web Content with Spring MVC
Example of an implementation of MVC with Spring
This is a simple web application that:

- Serves a static home page at `/`
- Responds to HTTP GET requests at `/greeting`

When you access the following URL:
http://localhost:8080/greeting

It returns an HTML page displaying:
Hello, World!

You can customize the greeting using an optional `name` parameter in the query string:

http://localhost:8080/greeting?name=User

Hello, User!

## How It Works

- The `/greeting` route accepts a `name` parameter
- If no name is provided, it defaults to `"World"`
- The app renders a basic HTML page with the greeting message

## Examples

- **Default greeting:**  
  [http://localhost:8080/greeting](http://localhost:8080/greeting)  
  Output: `Hello, World!`

- **Custom greeting:**  
  [http://localhost:8080/greeting?name=Alex](http://localhost:8080/greeting?name=Daniel)  
  Output: `Hello, Daniel!`