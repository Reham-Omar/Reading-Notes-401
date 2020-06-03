# API Server

## Express: Router Parameters
 - In Express, we already know that parameters in routes can be read
 -  we can run middleware on any route
 - can also run middleware on every request
 - Express lets you run middleware only when certain parameters are present and expected, eliminating that choice.
 
## Sub Documents in Mongoose

- Mongoose is a schema driven ORM, which gives us the opportunity to provide structure to our Mongo documents.
- With the addition of “Sub Documents”, Mongoose gives you the ability to take that a step further and use a schema to describe a deeper part of a data model.

## Joining Data/Documents in Mongo

- noSQL Databases don’t really join, and doing so generally is considered an anti-pattern.
- `populate()` is a method we can use in Mongoose to connect 2 collections
 * Method 1: physically joining using a reference to another collection
 * Method 2: Virtual Population
   - Create a virtual field in a document pointed to a field in another one.
   - In pre('find') you do a collection “on the fly” which can be more efficient than storing the relation.

 * Pre and Post hooks (middleware)
   - Mongoose allows you to inject logic at various points in the lifecycle of a data record.
   - User can perform validation, normalization