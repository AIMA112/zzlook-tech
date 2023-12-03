# Guidlines
- Adopt contributor guidelines similar to those established by notable open-source projects like Kubernetes, TensorFlow, or Node.js. 
- Follow the Model-View-Controller (MVC) architectural pattern ensuring separation of concerns and scalability. Utilize clear directory structures for models, views, and controllers. 


# Reference(s)
- Kubernetes Contributor Guide, TensorFlow Contributor Guide, Node.js Contribution Guide
- General MVC architectural principles



### Overview of the Project Structure:

This project sets up an API for managing items, using the Model-View-Controller (MVC) pattern to organize its components:

1. Model (com.example.crudapi.model):
   - The Item class defines the structure of an item with attributes like id, name, and price. This class represents the basic data model for items.

2. Repository (com.example.crudapi.repository):
   - The ItemRepository interface extends JpaRepository and handles database operations for the Item entity. It allows the application to perform CRUD operations on the items.

3. Controller (com.example.crudapi.controller):
   - The ItemController manages incoming HTTP requests related to items. It has several endpoints:
     - GET /api/items: Retrieves all items.
     - GET /api/items/{id}: Retrieves a specific item by its ID.
     - POST /api/items: Saves a new item.
     - DELETE /api/items/{id}: Deletes an item by its ID.

4. Service Layer (Presumed, not explicitly shown):
   - The ItemService likely handles business logic related to items. It would contain methods that interact with the ItemRepository, keeping the controller lean by separating concerns.

5. Main Application (com.example.crudapi.CrudApiApplication):
   - The CrudApiApplication class serves as the entry point for the application. It contains the main() method to start the Spring Boot application.

6.Developer Guidelines (Developer_Guidelines):
   - This section suggests exploring different contributor guidelines in open-source projects. It could be a resource guiding potential contributors on how to effectively contribute to this specific project.

### Understanding the MVC Structure:

- Model (Item Class): Defines the basic structure of items.
- Controller (ItemController): Manages incoming requests and defines endpoints for item-related operations.
-Service Layer (Assumed): Likely handles business logic, allowing separation from the controller for better maintainability.
  
               
