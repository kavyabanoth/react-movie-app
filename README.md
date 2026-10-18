# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
# React Movie App

A movie search and favorites app built with React and the TMDB API. Browse popular movies, search by title, and save your favorites.

## Features

- Browse popular movies on the home page
- Search movies by title
- Add and remove movies from a favorites list
- Favorites shared across pages with the Context API
- Client-side routing between Home and Favorites

## Tech Stack

- React (Vite)
- React Router
- Context API (state management)
- TMDB API
- CSS

## Screenshots

![Home page](screenshots/home.png)
![Favorites page](screenshots/favorites.png)

## Getting Started

1. Clone the repo
```bash
   git clone https://github.com/kavyabanoth/react-movie-app.git
   cd react-movie-app
```
2. Install dependencies
```bash
   npm install
```
3. Get a free API key from [TMDB](https://www.themoviedb.org/settings/api) and create a `.env` file in the project root:
```
   VITE_TMDB_API_KEY=your_api_key_here
```
4. Start the dev server
```bash
   npm run dev
```
5. Open `http://localhost:5173`

## Project Structure

```
src/
├── components/   # MovieCard, NavBar
├── contexts/     # MovieContext (favorites state)
├── css/          # Stylesheets
├── pages/        # Home, Favorites
└── services/     # api.js (TMDB requests)
```

## Future Improvements

- Movie recommendations based on favorites
- Genre filters and movie detail pages
- Persist favorites in localStorage

## Author

Kavya Banoth — [GitHub](https://github.com/kavyabanoth)
