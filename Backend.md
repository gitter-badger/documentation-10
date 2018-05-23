# Backend

The backend of the system is written using [Connexions](https://github.com/zalando/connexion), which is built on top of the [Flask](http://flask.pocoo.org/) framework. Written in Python, the structure of the backend is based on the logic of the [OpenAPI specification](https://swagger.io/specification/).

## Swagger

The Swagger file follows the OpenAPI specification and describes each API endpoint, as well as the parameters required, as well as the responses expected. Using tools provided by Swagger, documentation and testing can be provided with little to no development work.

### SDK Generation

Swagger tools can generate client side libraries in a number of languages, based on the `YAML` or `JSON` spec files. 

