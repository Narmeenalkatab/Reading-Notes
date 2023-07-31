## class: 34 : Reading Questions

1. **Key principles for organizing and configuring Django settings**:
   - Separate settings into multiple files based on concerns (base, development, production).
   - Use environment variables for sensitive data.
   - Set default values for common settings.
   - Protect sensitive data and use settings packages for easier management.

2. **White Noise library in Django**:
   - White Noise efficiently serves static files in production by serving them directly from the web server, reducing Python application server overhead.
   - Steps to integrate White Noise: Install, configure middleware, set STATIC_ROOT, run `collectstatic`, configure web server.

3. **Cross-Origin Resource Sharing (CORS) in Django**:
   - CORS controls access to resources on different domains to enforce same-origin policy.
   - Implementing CORS in Django: Install `django-cors-headers`, add to `INSTALLED_APPS` and `MIDDLEWARE`, configure CORS settings, optionally use `@cors_headers` decorator for specific URLs.