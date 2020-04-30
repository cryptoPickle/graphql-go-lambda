### IT is for only POC

![Go](https://github.com/cryptoPickle/graphql-go-lambda/workflows/Go/badge.svg?branch=master)
#### Schema

```
  schema {
		query: Query
	}
	type Person{
		id: ID!
		firstName: String!
		lastName: String
	}
	type Query{
		person(id: ID!): Person
	}
```

#### Example Query: 

```
{
    person(id: 1000){
        lastName
        firstName
    }
}
```

#### Deployment

Before deployment the easiest way to supply credentials is exporting the AWS_SECRET_ACCESS_KEY and AWS_ACCESS_KEY_ID
Second step just run make deploy. Enjoy.  
