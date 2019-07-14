## note

typical example, type, mutation, subscription 
```
type Query{
    allPerson(last:Int):[Person!]!
}

type Mutation{
    createPerson(name:String!,age:Int):Person!
}

type Subscription{
    newPerson:Person!
}

type Person{
    name:String!
    age:Int!
    posts:[Post!]!
}
type Post{
    title:String!
    author:Person!
}

```


The essence of GraphQL

GraphQL is a query language that traverses your data graph to produce a query result tree.--taken from [Apollo Blog](https://blog.apollographql.com/the-concepts-of-graphql-bc68bd819be3)