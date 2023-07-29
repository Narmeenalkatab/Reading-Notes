**Reading Questions**

1. **What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?**

  JWTs are compact, self-contained tokens used for secure transmission of information between parties. They consist of three parts: header, payload, and signature. JWTs encode user-related data and claims in the payload, and a signature ensures their integrity. Servers create JWTs by encoding the header and payload with a secret key. When clients send a JWT, the server verifies its authenticity by recalculating the signature.

2. **How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?**

   Django REST Framework (DRF) uses JWT Authentication to secure API endpoints. Key components involved are:
     - DRF Views and Endpoints representing API resources and functionality.
     - Authentication Classes like `JSONWebTokenAuthentication` to validate JWTs.
     - JSON Web Tokens issued to users upon login and sent in the Authorization header.
     - Authentication Backend verifying JWT and authenticating users.
     - DRF permissions classes controlling user access based on roles and permissions.

3. **Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?**

 `runserver` lacks production readiness due to its single-threaded nature and security concerns. Alternative server options include Gunicorn, uWSGI, nginx, and Apache, which offer better performance, scalability, and security. Docker and Kubernetes help with containerization and orchestration, while cloud platforms like AWS, Google Cloud, and Azure provide services for deploying Django applications.