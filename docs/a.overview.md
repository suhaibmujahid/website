---
id: a.overview
title: Building a Dockerized RESTful API application
---

In this section, we are going to build a RESTful API application to manage a simple bookshelf. And in here, we are discussing,

1. Creating a new Go project.
    - Creating a remote repository
    - Creating a Go module
2. Adding initial HTTP server.
3. Adding initial Docker files.
    - Adding a Dockerfile
    - Adding a docker-compose.yml
    - Support Docker multi-stage builds
4. Adding initial configurations.
    - Using environment variables for configurations
    - Populating data from environment variables
5. Adding [Chi router](https://github.com/go-chi/chi).
6. Adding [Zerolog logger](https://github.com/rs/zerolog).
    - Adding Zerolog as the Syslog logger
    - Implementing a request logger
    - Creating the main app package
7. Adding DB docker file.
8. Adding initial database migrations.
    - Implementing a DB adapter
    - Implementing a DB migration tool using Goose
    - Adding initial SQL migrations
    - Running migrations at the application startup
9. Adding [GORM](http://gorm.io/).
    - Implementing a GORM adapter
    - Adding GORM adapter to the main app
    - Checking application health
10. Adding initial books API routes.
    - Implementing initial books API Handlers
    - Implementing Content-Type JSON middleware
11. Implementing RESTful handlers.
    - Completing list books functionality
    - Completing read book functionality
    - Completing delete book functionality
    - Completing create book functionality
    - Completing update book functionality
12. Adding [Validator.v9](https://github.com/go-playground/validator).
    - Adding initial validator
    - Implementing custom validation messages
    - Implementing custom validation types

The completed project can be found in [learning-cloud-native-go/myapp](https://github.com/learning-cloud-native-go/myapp) GitHub repository and you can check the code on each step by using `step-` branches in the GitHub repository. The completed API application supports the following API endpoints.

![API Endpoints](assets/a.endpoints.png)

OK, Let's get it started!