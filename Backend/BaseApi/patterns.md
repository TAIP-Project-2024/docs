# Design Patterns

### Layered Architecture (Lazurca Samuel-Ionut)

- The **Base API** contains 3 main layers: _presentation, application, data access_
- Controllers represent the **Presentation** layer
- Services represent the **Application/Bussiness** layer
- Repositories and the entities(models) represent the **Data Access/Persistence** layer
- In addition to those 3, there will be a **Middleware** for _authentication/authorization_.

### Repository (Hriscu Alexandru-Grabriel)

- The **Repository Design Pattern** creates and abstraction layer for data access.
- This pattern encapsulates the logic required to access data.
- It isolates data access logic from business logic.
- It is used in **MongoDBRepository** and **PostgresRepository** classes.
- Will be implemented for every entity.
  
### Template (Nestor Maria)

- The **Template Design Pattern** is used to define a base repository interface for database.
- The concrete classes, **MongoDBRepository** and **PostgresRepository** implement the base methods defined in template.
- This allows flexibility in the underlying database logic.
- It is present in **DbTemplate** class

### Active Record (Maria)

- The **Active Record Design Pattern** is an architectural pattern to accessing data in a database
- A database table is wrapped into a class
- This pattern is used by object-relational mapping (ORM) by default

### Factory Method (Hriscu Alexandru-Gabriel)

- Implemented in the ``AnalysisFactory`` class to create instances of different analysis components based on the type requested. This promotes loose coupling between components.

### Chain of Responsibility (Lazurca Samuel-Ionut)

- Requests are passed along a chain of handlers.
- The middleware is a good example as it handles the request before passing it to the controllers
- The controllers also pass the request to the services that return the reponse.

### Visitor (Rotaru Florin)

- Lets us separate algorithms from the objects on which they operate
- A good example is the GraphDrawing class

### Dependency Injection Pattern (Hriscu Alexandru-Gabriel)

- Used in ``ControllerUser`` to inject ``User``, ``ViewLogin``, and ``PostgresRepository`` dependencies.

### Adapter (Rotaru Florin)

- Used in ``Graph`` class.

### DTO (Alex, Stefan)

### Singleton (Nastasiu Stefan)

- Used for ``Evaluation Metrics``

### Builder (Stefan)

### Observer (Stefan)
