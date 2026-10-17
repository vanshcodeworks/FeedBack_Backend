# Feedback Backend

Express + MongoDB API behind a feedback form: stores submissions and manages
user accounts with session-based authentication.

## Stack

- `express`, `mongoose`
- `passport`, `express-session`, `connect-flash`, `bcrypt`
- `ejs` views, `body-parser`, `cookie-parser`, `morgan`, `debug`

## Layout

```
bin/www       server bootstrap
app.js        Express app, middleware, routes
db/connect.js Mongo connection
models/       Mongoose schemas
routes/       API and form handlers
public/       static assets
```

## Setup

```bash
npm install
cp .env.example .env
node bin/www
```

## Notes

Scaffolded from the Express generator, so the layout still follows the
`bin/www` + `app.js` split rather than a single `server.js`. `morgan` and
`debug` are development-only dependencies.

There is no test suite.