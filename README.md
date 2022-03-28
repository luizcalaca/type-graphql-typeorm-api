# GraphQL APIs with TypeGraphQL and TypeORM

### Run project

```
npm install
npm start
```

## Running Apollo Server

```
mutation CreateBook($data: CreateBookInput!) {
  createBook(data: $data) {
    title
    author
  }
}
```

```
{
  "data": {
    "title": "Hello",
    "author": "Marcos"
  }
}
```

```
query Query {
  books {
    title
  }
}
```

### Dependencies

```
apollo-server type-graphql typeorm reflect-metadata

typescript ts-node nodemon
```

- Apollo Server to build and run our GraphQL server
- TypeGraphQL to generate our schema from TypeScript classes
- TypeORM to interact with our SQL database
- reflect-metadata to work with TypeScript decorators
