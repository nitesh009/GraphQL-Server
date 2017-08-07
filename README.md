# GraphQL-Server

This repo contains basic GraphQL Server which is developed using Node.js.
About GraphQL-
  1) Application layer query language
  2) Open sourced by Facebook in 2015
  3) Can be used with any type of database
  4) Ability to ask for exactly what you need and nothing more
  5) Get multiple resources in a single request
  
Project Plan for this repo-
  1) Build the back end server
  2) Setup Express with Express-Graphql
  3) Create schema file with queries and mutations
  4) Implement JSON-server
  5) Crud functionality
  6) Test with Graphiql
    
Clone this repo using git clone https://github.com/nitesh009/GraphQL-Server.git

Once you clone the repo, you need to install few dependencies-
npm install express express-graphql --save
npm install graphql --save
npm install json-server --save
npm install nodemon --save
npm install axios --save

After installing above mentioned dependencies, perform below steps-
cd customerbase

-Run JSON-Server (Port 3000)
$ npm run json:server

-Run Server (Port 4000)
$ npm run dev:server
-Visit Graphiql IDE

Go to http://localhost:4000/graphql

After that you can perform any of the CRUD operation mentioned below-
addCustomer:

  mutation{
    addCustomer(name:"XYZ",email:"XYZ@yahoo.com",age:21) {
      id,
      name,
      email
    }
  }
  
  deleteCustomer:
  
  mutation{
    deleteCustomer(id:"3") {
      id,
      name,
      email
    }
  }

Please comment if you face issues while performing any kind of CRUD operation.
