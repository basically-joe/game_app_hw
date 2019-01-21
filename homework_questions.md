1. What is responsible for defining the routes of the `games` resource?

create_router.js

2. What are the the responsibilities of server.js?

Utilising express and mogodb virtual servers on local host also parsing requests to json.

3. What are the responsibilities of the `gamesRouter`?

Passes the specific route address and data into the create_router.js file.

4. What process does the the client (front-end) use to communicate with the server?

HTTP using JSON.

5. What optional second argument does the `fetch` method take? And what is it used for in this application? Hint: See [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) on the MDN docs

An init object that allows control of:

    method: 'POST',
    body: JSON.stringify(payload),
    headers: { 'Content-Type': 'application/json' }

6. Which of the games API routes does the front-end application consume (i.e. make requests to)?

http://localhost:3000/api/game

7. What are we using the [MongoDB Driver](http://mongodb.github.io/node-mongodb-native/) for?

To make callback-based and Promise-based interactions with MongoDB

Why do we need to use [`ObjectId`](https://mongodb.github.io/node-mongodb-native/api-bson-generated/objectid.html) from the MongoDB driver?

This can be useful to save the space needed by an additional timestamp if you wish to track the time of creation of a document.
