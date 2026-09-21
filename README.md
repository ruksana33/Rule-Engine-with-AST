# Rule-Engine-with-AST
Non-Functional Considerations:

1.Security:
Implemented input validation and sanitization for user-provided rules to prevent injection attacks or malformed rule strings.
Applied authentication mechanisms for accessing the API endpoints, ensuring that only authorized users can create, modify, or combine rules.
Encrypted sensitive data in transit using HTTPS, providing a secure communication channel between the front-end, API, and backend.

2.Performance:
Optimized the AST structure to minimize the complexity of rule evaluation, ensuring efficient parsing and execution, especially when dealing with complex rules.
Implemented caching mechanisms for frequently used rule evaluations, reducing the need for repeated AST traversals for similar input data.
Designed the database schema with indexing on frequently queried fields to enhance the performance of data retrieval operations.

3.Scalability:
The application architecture supports horizontal scaling, allowing the API layer to handle an increased number of requests by adding more server instances.
The rule engine's design allows for dynamic addition and modification of rules without impacting existing rules, supporting scalability in rule management.

4.Maintainability:
Followed modular coding practices, separating concerns between the AST structure, rule parsing logic, and evaluation engine.
Included comprehensive documentation within the codebase and provided clear instructions in the README for easier setup and modifications.

5.Error Handling & Logging:
Implemented detailed error handling for invalid rule strings, unsupported operations, and data mismatches during evaluation.
Added logging mechanisms for monitoring API calls, rule evaluations, and error scenarios to support debugging and improve user experience.
