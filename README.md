# MERN-stack-workshop
# Express Static Site — MERN Workshop

I attended a MERN workshop and built this small Express project to practice serving static pages.

## Project overview
- Minimal Express server that serves static HTML pages from the `public/` folder.
- Routes:
  - `/` redirects to `/homepage`
  - `/homepage` — serves `public/home.html`
  - `/aboutpage` — serves `public/about.html`
  - `/contactpage` — serves `public/contact.html`
- Static assets (CSS, images) are in `public/` and served with `express.static`.

## Files added
- `app.js` — Express server and routes.
- `public/home.html`, `public/about.html`, `public/contact.html` — site pages.
- `public/style.css` — basic styling and navbar.
- `public/whatsapp.png` — small placeholder image.
- `package.json` — project dependencies (Express).

## Prerequisites
- Node.js (v14+ recommended)
- npm

## Install
Run from the project root:

```
npm install
```

(If you use `nodemon` for development, install it globally or as a dev dependency.)

## Run
Start the server with:

```
node app.js
```

Then open a browser at `http://localhost:3000/` (it redirects to `/homepage`).

To use automatic reload during development:

```
npm install --save-dev nodemon
npx nodemon app.js
```

## What this demonstrates
- Serving static files with Express.
- Simple routing that returns HTML files.
- Basic site layout and navigation with a sticky navbar.

## Next steps (suggestions for MERN workshop follow-up)
- Replace static pages with a React front-end (create a `client/` app and serve the production build).
- Add API routes in Express to handle data and connect to MongoDB (M in MERN).
- Use Mongoose to create models and persist data.
- Add authentication (JWT) and a RESTful API.

## Notes
This repository is intentionally small to focus on the basics covered during the MERN workshop. If you want, I can scaffold a `client/` React app, add example API endpoints, and wire up MongoDB next.
