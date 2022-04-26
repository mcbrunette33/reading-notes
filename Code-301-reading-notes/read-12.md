# Read 12

## codes

- 100's = Informational status codes; header part of request recieved and the server will try to comply with a transmission demand of the client.

- 200's = Succes codes; request was accepted. Regarding asynchronous processing of a request (202), this doesn't mean the request was successfully processed only that it met all validation requirements.

- 300's = Redirection Codes. Tells the client that the resource requested isn't available at the expected location anymore.

- 400's = Client Error codes. Invalid requests that a client sent to a server. 

- 500's = Sever Error codes. Overwhelmed server or unreachable servers behind proxies, but sometimes can be related to client requests that trigger error exceptions on the server.

- 202 = his code tells the client that the request was valid, but its processing will finish sometime in the future.

- 308 = This tells the clients to use another URL to access the resource and not use the current URL anymore. It's helpful to have multiple endpoints for one resource.

- 204 = you use if an update didn't return data to a client

- 404 = use if a resource used to exist but no longer does

-403 = Forbidden


