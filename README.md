# Tech Literacy Series Project: Backend

This project is based on [this tutorial by Callicoder](https://www.callicoder.com/node-js-express-mongodb-restful-crud-api-tutorial/).

## Prerequisites

- MongoDB
- NodeJS
- yarn or npm
- Heroku CLI

## Deploy

```
git push heroku master
```

## Test Command

When testing locally, to create a new record, use:

```
curl -d '{"title":"Introduction","content":"Hello World!"}' -H 'Content-Type: application/json' http://localhost:3000/notes
```

If testing in production, use:

```
curl -d '{"title":"Introduction","content":"Hello World!"}' -H 'Content-Type: application/json' https://<URL>/notes
```

**Note:** Replace <URL> with the URL of the Heroku app.