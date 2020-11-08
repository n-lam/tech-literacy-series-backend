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

## Usage

1. Clone git repository. You can use the following command: `git clone https://github.com/n-lam/tech-literacy-series-backend.git`
2. Go into the project folder: `cd tech-literacy-series-backend`
3. Install dependencies: `yarn`
4. Start the server: `yarn start`

## Testing

**Note:** Replace `<domain>` with the URL of the Heroku app. If you are testing locally, replace it with `localhost:3000`.

### Insert Record

```
curl -d '{"title":"Introduction","content":"Hello World!"}' -H 'Content-Type: application/json' http://<domain>/notes
```

### Find All Records

```
curl http://<domain>/notes/
```

### Find All Records with a given Title or Content

```
curl http://<domain>/notes/?query=hello
```

### Find One Record

```
curl http://<domain>/notes/<id>
```

### Update Record

```
curl -X PUT -H 'Content-Type: application/json' -d '{"title":"Introduction","content":"Goodbye!"}' http://<domain>/notes/<id>
```

### Delete Record

```
curl -X DELETE http://<domain>/notes/<id>
```
