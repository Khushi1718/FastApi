## API

**API (Application Programming Interface)** = a way for two software systems to **communicate with each other**.

### Before APIs
- Applications were often **monolithic**.
- Frontend, backend, database, and business logic were tightly connected.
- One application directly handled everything.
- If one part changed, the whole application could be affected.
- Harder to scale and maintain.

### Monolithic Architecture
```text
Frontend
   ↓
Backend + Business Logic + Database
   ↓
Everything in one application
```

### After APIs
- Applications can be split into **separate services**.
- Services communicate through **APIs**.
- Frontend does not directly access the database.
- It sends a request to the backend API.
- API processes the request and returns a response.
- Easier to **develop, scale, maintain, and reuse**.

```text
Frontend → API → Backend/Service → Database
             ↓
          Response
```

### Simple Example
```text
GET /users/123
```

Frontend asks the API for user `123`.

API → Backend → Database → API → Frontend

**In short:**  
> **API = a bridge/contract that allows different software components to communicate without knowing how each other works internally.**