## Class 33: Authentication & Production Server

### What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

The primary purpose of JSON Web Tokens (JWTs) is to securely transmit information between parties as a compact and self-contained data structure. JWTs are typically used for authentication and authorization purposes in web applications. They work by encoding the data (payload) in a JSON format and signing it with a secret key or a public/private key pair. The encoded payload contains information about the user or any other data that needs to be shared. When a client sends a JWT to the server, the server can validate the integrity of the token by verifying its signature using the secret or public key. If the signature is valid, the server can trust the data in the token and use the information for authentication or authorization purposes. JWTs are stateless, meaning the server doesn't need to store any session information, making them scalable and suitable for use in distributed systems.

### How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

JWT authentication can be integrated with Django REST Framework (DRF) to secure API endpoints by using the djangorestframework-simplejwt library or other similar JWT packages. The key components involved in this process are:

1. **Authentication Backends:** DRF provides authentication backends that handle authentication logic. The JWT authentication backend is added to the list of authentication backends in the project settings.

2. **Views and Endpoints:** In the Django views where API endpoints are defined, decorators or mixins are used to specify that JWT authentication is required for accessing those endpoints.

3. **Token Generation:** When a user logs in or registers, a JSON Web Token is generated and returned to the client upon successful authentication.

4. **Token Verification:** For secured endpoints, the client must include the JWT in the request headers. The DRF authentication middleware then verifies the token's validity and decodes the payload to identify the user or their permissions.

5. **Permission Classes:** DRF also provides permission classes that determine whether a user has the required permissions to access specific API endpoints. These permission classes are used in conjunction with JWT authentication to control access to resources.

### Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

Django's built-in development server (runserver) is not suitable for production environments primarily because it is designed for development purposes and lacks essential features and optimizations required for handling high traffic, security, and performance in a production setting. It is single-threaded, not meant for handling multiple concurrent requests, and may not be as robust as production-grade servers. For deploying a Django application in a production environment, alternative server options should be considered. Some popular choices are Gunicorn (Green Unicorn), uWSGI, and Apache with mod_wsgi. These servers are capable of handling multiple concurrent requests, offer better performance, and come with additional features like load balancing, process management, and better security configurations, making them more suitable for hosting Django applications in production environments.
