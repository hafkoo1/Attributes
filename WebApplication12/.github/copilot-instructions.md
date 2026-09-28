# Project Instructions

## Project

This is an ASP.NET Core Web API project for managing products/orders, creating, searching and displaying data.

### Architecture

* Controllers/ — API controllers
* Models/ — DTOs and models
* Entities/ — database entities
* Services/ — business and database logic
* Data/ — AppDbContext

Keep database logic in services, not controllers.

## Rules

### Coding

* Keep code simple and readable
* Follow the existing project structure
* Do not add unnecessary libraries or abstractions
* Avoid duplicate code
* Use explicit types instead of `var`
* Do not add unnecessary comments or debug code

### Controllers

* Controllers handle HTTP requests and responses
* Use services for business/database logic
* Validate incoming models
* Return correct HTTP status codes
* Keep controller actions short

### Models and Entities

* Use DTOs for API requests and responses
* Do not expose database entities directly unless necessary
* Use validation attributes such as `[Required]`, `[StringLength]` and `[Range]`

### Services

* Put business and database operations in services
* Use dependency injection
* Use `AppDbContext` through services

### Testing

* Write unit tests for controller actions
* Use xUnit
* Use Moq for dependencies
* Test both success and failure scenarios
* 
### Before Changing Code

* Review existing code first
* Check existing controllers, services, models and entities
* Reuse existing code when possible
* Do not change unrelated code

### After

* Build the project and run tests
* Remove debug or unused code
* Check for compilation errors
* Update Swagger/OpenAPI documentation if it exists
* Keep changes small and simple
