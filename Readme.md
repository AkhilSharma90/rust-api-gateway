# rust-api-gateway

Here, we define a Service struct that represents a backend service, with a name field and a url field. We also define four routes:

/ returns a simple greeting message.
/services returns a list of registered services.
POST /services adds a new service to the list.
DELETE /services/<name> removes a service from the list by name.
In the main() function, we create a vector of initial services and pass it to the Rocket ignite() function as a managed state. We then mount the four routes, register a 404 error catcher, and launch the Rocket server.

