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