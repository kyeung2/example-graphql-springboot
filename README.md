# example-spring-boot-graphql

## schema generation
![runtime schema creation](src/main/resources/graphql_creation.png)

## build
`gradle clean build`

## test
`gradle test --warning-mode all`

## run
`gradle bootRun`

## usage
- install: [graphql-playground](https://github.com/graphql/graphql-playground)
- URL endpoint: [localhost:8080/graphql](http://localhost:8080/graphql)
- request:
```graphql
{
  bookById(id: "book-1"){
    id
    name
    pageCount
    author {
      firstName
      lastName
    }
  }
}
```

## todo
- initial setup with a simple query with static data
- add a database
- add mutations
- replace spring mvc with spring webflux
- ...
- final, take code in this repo and replace in [previous repo](https://github.com/kyeung2/tutorial-graphql)
- delete this repo, and rename the previous repo to this `example-graphql-springboot`


## links
- [GraphQL getting started](https://www.graphql-java.com/tutorials/getting-started-with-spring-boot/)
