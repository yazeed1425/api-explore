## Documenting 201 and 409 Status Codes

### 1. First Attempt (201 Created)
When sending the POST request for the first time, the server successfully creates the resource and returns a `201 Created` status code.

### 2. Second Attempt (409 Conflict)
When sending the exact same POST request again, the server rejects it because the username already exists, returning a `409 Conflict` status code. This means the request could not be completed due to a conflict with the current state of the target resource.
