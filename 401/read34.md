# API Deployment

## Django Settings Best Practices

- Use environment variables: Store sensitive information, such as database credentials, in environment variables rather than hard-coding them into the settings file. This makes it easier to manage different configurations for different environments, such as development, staging, and production.
- Use a separate settings file for each environment: Create separate settings files for each environment, such as development, staging, and production, to manage environment-specific configurations.
- Keep secrets out of version control: Do not store sensitive information, such as secret keys and passwords, in version control. Instead, use environment variables or encrypted configuration files to manage secrets securely.
- Use an external configuration management tool: Use an external configuration management tool, such as Ansible or Chef, to manage configurations and automate deployment processes.
- Set DEBUG to False in production: Make sure to set the DEBUG setting to False in production to ensure that sensitive information is not displayed in error pages.
- Use HTTPS in production: Use HTTPS to secure communication between the client and server in production environments.
- Use caching: Enable caching in the production environment to improve performance and reduce the load on the server.
- Use a production-ready database: Use a production-ready database, such as PostgreSQL or MySQL, in production environments.
- 12 Factors is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the Cloud. It was created by Heroku
  - Codebase
  - Dependencies
  - Config
  - Backing services
  - Build, release, run
  - Processes
  - Port binding
  - Concurrency
  - Disposability
  - Dev/prod parity
  - Logs
  - Admin processes
- WhiteNoise is a Python library for serving static files during development and production for Django projects. It provides a simple way to handle static files by automatically configuring and serving static files, such as CSS, JavaScript, images, and other media, directly from the Django application.
- WhiteNoise makes it easy to serve static files from Django, regardless of whether you're using Django's built-in development server or a production-ready web server such as Gunicorn or uWSGI. This is especially useful in production environments where performance is a concern and serving static files directly from the application server is more efficient than relying on a separate web server to handle static files.
- Use Django-environ to store .env variables (like API keys)

### Things I want to know more about

- What is the best way to set up my Django environment settings?

### Sources

- <https://djangostars.com/blog/configuring-django-settings-best-practices/>
- <https://whitenoise.evans.io/en/stable/>
- <https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing>

[Back To Home](../README.md)