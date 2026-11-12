# REST API Testing with Postman

A Postman collection demonstrating functional API checks against JSONPlaceholder: https://jsonplaceholder.typicode.com/

## Coverage
- GET collection and individual resource
- Status code and response contract checks
- Field type and non-empty validation
- Response-time threshold (network dependent)
- POST request and response validation
- Missing-resource behavior

## Run
1. Import `JSONPlaceholder-QA-Portfolio.postman_collection.json` into Postman.
2. Run the collection using Collection Runner.

Optional CLI:
```bash
npm install -g newman
newman run JSONPlaceholder-QA-Portfolio.postman_collection.json
```

JSONPlaceholder is a mock API. Write operations are simulated and do not persist like a production backend. Response-time checks vary with network conditions. Investigate failures rather than automatically classifying them as defects.
