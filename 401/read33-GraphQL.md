# API (GraphQL)

* GraphQL is a query language and server-side runtime for application programming interfaces (APIs) 
that prioritizes giving clients exactly the data they request and no more. ... As an alternative to REST,
GraphQL lets developers construct requests that pull data from multiple data sources in a single API call.

### relationships between types

* supports one-to-one,
*  one-to-many,
*  and many-to-one relationships.

### Usage

* Relationships between types are specified by annotating fields on an @model object type with the @connection directive.

* The fields argument can be provided and indicates which fields can be queried by to get connected objects.


#### Has one

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

#### Has many

```
type Post @model {
  id: ID!
  title: String!
  comments: [Comment] @connection(keyName: "byPost", fields: ["id"])
}

type Comment @model
  @key(name: "byPost", fields: ["postID", "content"]) {
  id: ID!
  postID: ID!
  content: String!
}
```

#### Many-to-many connections

```
type Post @model {
  id: ID!
  title: String!
  editors: [PostEditor] @connection(keyName: "byPost", fields: ["id"])
}

# Create a join model and disable queries as you don't need them
# and can query through Post.editors and User.posts
type PostEditor
  @model(queries: null)
  @key(name: "byPost", fields: ["postID", "editorID"])
  @key(name: "byEditor", fields: ["editorID", "postID"]) {
  id: ID!
  postID: ID!
  editorID: ID!
  post: Post! @connection(fields: ["postID"])
  editor: User! @connection(fields: ["editorID"])
}

type User @model {
  id: ID!
  username: String!
  posts: [PostEditor] @connection(keyName: "byEditor", fields: ["id"])
}
```


# Note:

* GraphQL is an alternate option to build APIs in REST. Facebook developed it as an internal technology
 for their versatile applications, and later, publicly released it as open-source. Since then, 
 the software development community has utilized it as one of the favourite technology stacks for developing web services.

