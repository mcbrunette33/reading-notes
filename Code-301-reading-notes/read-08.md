# Read 08

## REST

- REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client
- A resource has an identifier, which is a URL that uniquely identifies that resource.
- Clients interact with a service by exchanging representations of resources.
- Many Web APIs use JSON as the exchange as the format. {key: value: } pairs
- REST APIs use a uniform interface, which helps to decouple the client and service implementations.
- REST APIs built on HTTP, the uniform interface includes using standard HTTP verbs to perfomr operators on resources.
- The most common operations are GET, POST, PUT, PATCH, and DELETE

## Web API design

- modern web applications expose APIs that clients can use to interactd with the app
- well designed API should support Platform independence and service evolution

## Organize the API around resources

- focus on the business entities that the web API exposes. 
- resource doesn't have to be based on a single physical data item. 
- the purpose of REST is to model entities and the operations that an application can perform on those entities.
- Adopt a consistent naming convention in URIS- use plural nouns that reference collections.
- Sending an HTTP GET requiest to the collection URI retrieve a list of items in the collection.