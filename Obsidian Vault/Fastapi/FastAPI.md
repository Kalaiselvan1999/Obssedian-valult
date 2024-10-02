- most loved frameworks in the Stack Overflow Developer Survey 2022
- modern features like Asynchronous Server Gateway Interface (ASGI) support and built-in OpenAPI spec (Swagger).
- FastAPI proved to be much faster than traditional frameworks like Flask and Django
- **Asynchronous Support:** Ideal for I/O-bound operations like API calls and database queries.
- **Server-Sent Events (SSE):** Facilitates real-time features.
- **OAuth2 Support:** Simplifies secure authentication.


## Features
1. Dependency Injection - Use this feature for common tasks like database connections or user authentication
2. Response Model - Declare your response structure with Pydantic models. auto-generates your API documentation and validates the response data
3. HTTPException
4. Path Parameters and Converters
5. Background Tasks
6. Query Parameters and String Validations
7. OAuth2 with Password (and hashing), Bearer with JWT tokens
8. Data validation and serialization with Pydantic
9. Testing with Starlette’s TestClient
10. Automatic interactive API documentation with doc and redoc
