## API (GRAPHQL)
#### Add relationships between types

A connection is a way to get all of the nodes that are connected to another node in a specific way.
The @connection directive enables you to specify relationships between @model types.

```
directive @connection(keyName: String, fields: [String!]) on FIELD_DEFINITION
```

Example of define a one-to-one connection

```
type Project @model {
  id: ID!
  name: String
  team: Team @connection
}

type Team @model {
  id: ID!
  name: String!
}
```

##### Alternative definition
- directive @connection(name: String, keyField: String, sortField: String, limit: Int) on FIELD_DEFINITION
- Defining index structures using @key and connection resolvers using @connection. There is an older parameterization of @connection that creates indices and connection resolvers that is still functional for backwards compatibility reasons. It is recommended to use @key and the new @connection via the fields argument.
- Limit - The default number of nested objects is 100, and you can override this behavior by setting the limit argument.
