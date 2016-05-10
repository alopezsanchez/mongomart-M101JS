# mongomart-M101JS
M101JS: MongoDB for Node.js Developers final exam. 

https://university.mongodb.com/

## Prerequisites
 - [Git](https://git-scm.com/)
 - [Node.js and npm](nodejs.org)
 - [MongoDB](https://www.mongodb.com/)
 
## Configuration and Usage
```sh
$ git clone https://github.com/alopezsanchez/mongomart-M101JS.git && cd mongomart-M101JS
$ mongoimport --collection item --db mongomart data/items.json
$ mongoimport --collection cart --db mongomart data/cart.json
$ npm install
$ node mongomart.js
```

You will to create a single text index on the item collection. You can create it in the mongo shell:
```
> db.getCollection('item').createIndex({title: "text", slogan : "text", description : "text"})
```

After, go to `localhost:3000`
