# Car-ify: A Fastify-based Car API with Swagger and GraphQL

Welcome to the Car-ify project! This repository contains a Node.js application that serves a Car API. The API allows users to fetch details of cars using both RESTful endpoints and GraphQL queries. The API documentation is generated using Swagger, and the application is built using the Fastify framework for its speed, security, and plugin architecture. MongoDB is used as the database, and Mongoose provides a schema-based solution for modeling application data.

## Technologies Used

- **Fastify**: Fastify is a web framework highly focused on providing the best developer experience with the least overhead and a powerful plugin architecture.
- **Mongoose**: Mongoose provides a straightforward, schema-based solution to model application data. It includes built-in type casting, validation, query building, business logic hooks, and more.
- **Swagger**: Swagger documentation generator for Fastify. It uses the schemas declared in routes to generate a Swagger-compliant documentation.
- **GraphQL**: GraphQL is a query language for APIs and a runtime for executing those queries by using a type system defined by the user.
- **fastify-swagger**: Plugin for Fastify to generate Swagger documentation automatically.
- **boom**: Utility library for returning HTTP errors.

## Getting Started

To get started with Car-ify, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/theFutureGuy/Car-ify.git
   ```

2. Install dependencies:

   ```bash
   cd Car-ify
   npm install
   ```

3. Set up environment variables:

   Create a `.env` file in the root of the project and specify the following environment variables:

   ```plaintext
   MONGODB_URI=<your-mongodb-uri>
   PORT=<port-number>
   ```

   Replace `<your-mongodb-uri>` with the connection URI for your MongoDB database, and `<port-number>` with the port number you want the server to listen on.

4. Start the server:

   ```bash
   npm start
   ```

   The server will start running on the specified port, and you can access the API documentation by visiting `http://localhost:<port>/documentation`.

## API Endpoints

### RESTful Endpoints

- `GET /cars`: Get a list of all cars.
- `GET /cars/:id`: Get details of a specific car by ID.
- `POST /cars`: Add a new car.
- `PUT /cars/:id`: Update details of a specific car by ID.
- `DELETE /cars/:id`: Delete a car by ID.

### GraphQL Endpoint

- `POST /graphql`: Send GraphQL queries to retrieve data.

## API Documentation

The API documentation is automatically generated using Swagger. You can access it by visiting `http://localhost:<port>/documentation` when the server is running.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the application.

## License

This project is licensed under the LGPL-2.1 license - see the [LICENSE](LICENSE) file for details.
