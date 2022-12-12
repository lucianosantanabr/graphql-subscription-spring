## Spring Boot GraphQL Subscription API


Open http://localhost:8080/graphiql for GraphQL introspection.

GraphQL Request
```graphql
subscription {
  stockPrice(symbol:"SAMPLE") {
    price
    symbol
    timestamp
  }
}
```

Response
```graphql
{
  "stockPrice": {
    "price": "0.7490690579285905",
    "symbol": "SAMPLE",
    "timestamp": "2020-05-22T22:16:12.092143"
  }
}
```
