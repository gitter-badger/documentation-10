# Backend

The backend of the system is written using [Connexions](https://github.com/zalando/connexion), which is built on top of the [Flask](http://flask.pocoo.org/) framework. Written in Python, the structure of the backend is based on the logic of the [OpenAPI specification](https://swagger.io/specification/).

## Swagger

The Swagger file follows the OpenAPI specification and describes each API endpoint, as well as the parameters required, as well as the responses expected. Using tools provided by Swagger, documentation and testing can be provided with little to no development work.

### SDK Generation

Swagger tools can generate client side libraries in a number of languages, based on the `YAML` or `JSON` spec files. To generate files, `swagger-codegen` is required and can be used to create SDKs; if it is not supported, client tools can handle many other languages.

### Prequisites

1. PostgreSQL
2. Python 3.6+

### Running

1. `git clone https://github.com/CitizenScienceCenter/cccs-connexion`
2. cd cccs-connexion
3. `virtualenv env` \(ensure Python3\)
4. `source env/bin/activate`
5. `pip install -r requirements.txt`
6. Set your connection string in `config.py`

The backend server will then be running in development on port **8080. **

## TODO

* Oauth support
* Dev and production environments
* Dockerise



