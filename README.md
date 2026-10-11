# MERN Stack REST API

A minimal Express + MongoDB REST API for managing "ninja" records, built while learning the MERN stack.

## About

A small practice project implementing basic CRUD endpoints over a MongoDB collection with Express and Mongoose. Built 2021-07.

## Features

- List, create, update and delete "ninja" documents via a REST API
- Mongoose schema with a nested GeoJSON point field (name, address, availability, age, location)
- Centralized Express error-handling middleware

## Tech stack

- Node.js, Express 4
- MongoDB with Mongoose 5
- body-parser
- nodemon (dev)

## Project structure

```
index.js          # Express app setup, MongoDB connection, error handler
routes/api.js      # /api/ninjas CRUD routes
models/ninja.js     # Mongoose schema/model for ninjas
```

## Getting started

```bash
npm install
npm start   # or: node index.js
```

Requires a local MongoDB instance reachable at `mongodb://localhost/ninjago` (connection string is hardcoded in `index.js`). The server listens on `process.env.port` or `4000`.

API base path: `/api/ninjas` (GET, POST, PUT /:id, DELETE /:id).

## Status

Learning project, not maintained.

## Related projects

- https://github.com/tolgazorlu/mern-blog
- https://github.com/tolgazorlu/mern-todo

## License

MIT, see [LICENSE](LICENSE).
