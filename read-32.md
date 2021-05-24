#### Serverless architecture
Serverless architecture (also known as serverless computing or function as a service, FaaS) is a software design pattern where applications are hosted by a third-party service, eliminating the need for server software and hardware management by the developer.


![sa](https://hackernoon.com/hn-images/1*t4O4UXpdG68MQboNKC6bBw.jpeg)

![a](https://hackernoon.com/hn-images/1*x_v5NRC3TTMt1MaYl1gMUg.jpeg)

A Serverless solution consists of a web server, Lambda functions (FaaS), security token service (STS), user authentication and database.

#### AWS Amplify
Amplify facilitates getting started with AWS for web and mobile app development because it is easy to use and flexible. The Amplify libraries accelerate implementation of functionality like user authentication, data storage, analytics, and predictions, using AWS services for the back-end functionality

Use cases - onboarding flows, real-time collaboration, AI/ML, and targeted campaigns.



#### API (GRAPHQL)
GraphQL is a query language and server-side runtime for application programming interfaces (APIs) that prioritizes giving clients exactly the data they request and no more. GraphQL is designed to make APIs fast, flexible, and developer-friendly.
```
type Blog @model {
  id: ID!
  name: String!
  posts: [Post] @connection(name: "BlogPosts")
}
type Post @model {
  id: ID!
  title: String!
  blog: Blog @connection(name: "BlogPosts")
  comments: [Comment] @connection(name: "PostComments")
}
type Comment @model {
  id: ID!
  content: String
  post: Post @connection(name: "PostComments")
}
```
* Objects annotated with @model are stored in Amazon DynamoDB and are capable of being protected via @auth, related to other objects via @connection, and streamed into Amazon Elasticsearch via @searchable.
* @model directive that allows you to easily define top level object types in your API that are backed by Amazon DynamoDB.
