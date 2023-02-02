# Authentication & Production Server

## JSON Web Tokens

- JSON Web Token(JWT): A way to securely transmit info between parties as JSON Objects
- JWT are analogous to having a stamp to get back into a nightclub
- JWT is used most commonly for Authorization, once a user logs in, they get a JWT token and this gives them access without having to re-sign in
- JWT is also used for information exchange, it allows you to safely send information to a verified individual
- JWT consists of a Header, Payload, and Signature
- Header contains the type of token that is used (JWT Token) and the signing algorithm that is used
- Payload contains claims which can be registered, public or private claims
- Import to not store sensitive session info in the browser like SSN or Credit Card info due to the lack of security
- Signed tokens expose all the information they contain and are viewable to other parties, so don’t add secret info here.
- JSON parsers are common in most programming languages

## DRF JWT Authentication

- The JWT is acquired by exchanging an username + password for an access token and an refresh token.
- The access token is usually short-lived (expires in 5 min or so, can be customized though).
- The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.
- First step is to authenticate and obtain the token. The endpoint is /api/token/ and it only accepts POST requests.
- To get a new access token, you should use the refresh token endpoint /api/token/refresh/ posting the refresh token

## Django Runserver Is Not Your Production Server

- Django's development server, "runserver", is not suitable for production use
- Development server is single-threaded and does not handle multiple requests simultaneously
- It does not automatically restart when code changes are made
- It also does not provide robust error handling
- It is not optimized for performance
- For these reasons, it is important to use a production-ready server when deploying Django applications Some common options include:
  - Gunicorn
  - uWSGI
  - Apache with mod_wsgi
- These servers provide multi-threading, automatic process management, and better error handling. Also they provide advanced features like:
  - load balancing
  - SSL support
  - request proxying
- When deploying a Django application, it is important to carefully choose a production-ready server that meets the specific needs of the application, taking into account factors such as performance, ease of use, and cost.

### Things I want to know more about

- How does JWT compare to other authentication methods like Auth0?

### Sources

- <https://jwt.io/introduction/>
- <https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html>
- <https://vsupalov.com/django-runserver-in-production/>

[Back To Home](../README.md)