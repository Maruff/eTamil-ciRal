# eTamil-ciRal
A framework of tools and libraries for eTamil

### Overview of ciRal Framework Development

The goal is to develop ciRal, a framework using Rust and eTamil to offer functionalities similar to FilamentPHP but developed in a modular fashion, akin to the Flask approach. Each functionality will be developed as a standalone library or tool, which can later be combined to form the full framework.

### Key Considerations:
1. **ciRal Usability for Rust Development**: ciRal is intended to be a flexible framework usable with both eTamil and Rust. Developers can write application logic in either language, and ciRal will support Rust natively while providing seamless interoperability with eTamil.

2. **Use of Existing Rust Frameworks and Libraries**: ciRal can and should leverage existing Rust libraries and frameworks where appropriate. This includes using libraries for routing, ORM, authentication, etc., and extending or wrapping them to ensure compatibility with eTamil.

3. **eTamil's Use of Existing Rust Tools and Libraries**: eTamil can interact with existing Rust tools and libraries via FFI (Foreign Function Interface) or bindings, enabling reuse of the robust Rust ecosystem.

### Overall Project Structure

    **Prerequisite Libraries for eTamil Language**
    **Core Tools/Libraries Development**
        Routing System
        Service Container (Dependency Injection)
        ORM/Database Abstraction
        Authentication and Authorization
        Form and Table Handling
        CRUD Operations Generator
        Resource Management
        Customizable Widgets
        Localization Support
        Notification and Alert System
        Plugin and Extensibility System
    **Integration and Framework Compilation**

### **Step-by-Step Procedure for ciRal Development**

#### **1. Prerequisite Tools and Libraries for eTamil Language**

##### 1.1. **eTamil Language Compiler/Interpreter**
   - **Tasks**:
     - Develop a Rust-based compiler or interpreter for eTamil using LLVM.
     - Ensure support for both procedural and object-oriented programming paradigms.
   - **Estimated Man-Days**: **20 man-days**

##### 1.2. **Standard Library for eTamil**
   - **Tasks**:
     - Develop a standard library in Rust for eTamil, providing basic data structures, utilities, and I/O handling.
   - **Estimated Man-Days**: **15 man-days**

##### 1.3. **Package Manager for eTamil**
   - **Tasks**:
     - Create a Rust-based package manager for eTamil, akin to Cargo, to manage dependencies, versioning, and distribution.
   - **Estimated Man-Days**: **10 man-days**

---

#### **2. Core Tools/Libraries for ciRal Framework**

##### 2.1. **Routing System Library**
   - **Tasks**:
     - Develop a flexible routing system in Rust, allowing both eTamil and Rust handlers to be used.
     - Support middleware and RESTful routing.
     - Consider using or adapting existing Rust libraries (e.g., Actix Web's routing or Rocket’s routing system).
   - **Estimated Man-Days**: **10 man-days**

##### 2.2. **Service Container and Dependency Injection**
   - **Tasks**:
     - Implement a service container in Rust to manage dependency injection.
     - Ensure it supports both eTamil and Rust services.
   - **Estimated Man-Days**: **8 man-days**

##### 2.3. **ORM/Database Abstraction Layer**
   - **Tasks**:
     - Develop an ORM in Rust, making it accessible from eTamil.
     - Include migrations, schema management, relationships, and query building.
     - Leverage Diesel ORM or SeaORM from Rust as a foundation.
   - **Estimated Man-Days**: **15 man-days**

##### 2.4. **Authentication and Authorization Library**
   - **Tasks**:
     - Develop authentication and authorization libraries in Rust with eTamil bindings.
     - Support session-based and token-based authentication.
     - Implement role-based access control (RBAC).
     - Utilize existing Rust libraries like `jsonwebtoken` or `actix-identity`.
   - **Estimated Man-Days**: **12 man-days**

##### 2.5. **Form and Table Handling Library**
   - **Tasks**:
     - Create libraries in Rust to handle form creation, validation, and table rendering.
     - Use JavaScript frameworks (React/Vue.js) for the front-end, with Rust managing the backend.
     - Include support for file uploads, real-time validation, and pagination.
   - **Estimated Man-Days**: **15 man-days**

##### 2.6. **CRUD Operations Generator Library**
   - **Tasks**:
     - Build a tool in Rust to automatically generate CRUD operations based on model definitions in eTamil.
     - Integrate with the ORM/Database layer.
   - **Estimated Man-Days**: **10 man-days**

##### 2.7. **Resource Management Library**
   - **Tasks**:
     - Develop a library in Rust to manage application resources (models, routes, views).
     - Ensure compatibility with eTamil for defining and managing resources.
   - **Estimated Man-Days**: **8 man-days**

##### 2.8. **Customizable Widgets Library**
   - **Tasks**:
     - Create a library in Rust for building customizable widgets (e.g., charts, tables) for dashboards.
     - Use JavaScript for front-end rendering, with Rust handling the backend data.
   - **Estimated Man-Days**: **12 man-days**

##### 2.9. **Localization Support Library**
   - **Tasks**:
     - Implement localization support in Rust, with eTamil APIs for language and region-specific settings.
     - Include translation files and a translation API.
   - **Estimated Man-Days**: **8 man-days**

##### 2.10. **Notification and Alert System Library**
   - **Tasks**:
     - Develop a notification system in Rust that handles various notification types (email, SMS, in-app).
     - Integrate with eTamil to trigger notifications.
     - Use WebSockets for real-time notifications, with JavaScript handling front-end alerts.
   - **Estimated Man-Days**: **10 man-days**

##### 2.11. **Plugin and Extensibility System**
   - **Tasks**:
     - Create a plugin system in Rust, allowing both Rust and eTamil plugins to extend core functionalities.
     - Develop a plugin manager for installation, updates, and version control.
   - **Estimated Man-Days**: **10 man-days**

---

#### **3. Integration, Testing, and Framework Compilation**

##### 3.1. **Integration of Libraries**
   - **Tasks**:
     - Integrate all the developed libraries into a cohesive framework.
     - Ensure interoperability between Rust and eTamil components.
   - **Estimated Man-Days**: **12 man-days**

##### 3.2. **Testing and Quality Assurance**
   - **Tasks**:
     - Conduct unit and integration tests for each library.
     - Perform load and stress testing.
     - Automate testing using CI/CD pipelines.
   - **Estimated Man-Days**: **12 man-days**

##### 3.3. **Documentation**
   - **Tasks**:
     - Write comprehensive documentation for each library and the overall framework.
     - Provide API references, tutorials, and examples.
   - **Estimated Man-Days**: **10 man-days**

##### 3.4. **Final Review and Deployment**
   - **Tasks**:
     - Perform a final review, code audit, and prepare for public release.
     - Set up deployment pipelines and provide initial support.
   - **Estimated Man-Days**: **8 man-days**

---

### **Estimated Total Duration**
   - **Total Duration**: **~200-205 man-days**

### **Summary**

- **ciRal’s Dual Compatibility**: ciRal will support development in both eTamil and Rust, leveraging Rust’s ecosystem while providing an easy-to-use interface for eTamil developers.
- **Reuse of Existing Rust Libraries**: Where possible, existing Rust libraries (e.g., Actix Web, Diesel ORM) will be adapted or extended to save development time and ensure stability.
- **eTamil Integration**: eTamil will be able to interact with these Rust libraries via FFI or through bindings, allowing the language to leverage Rust's performance and extensive tooling.

This approach ensures modularity, allowing each library to be developed, tested, and iterated independently before being integrated into the full ciRal framework.
