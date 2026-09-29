# Blog Pessoal – Front End

> **Study project – Generation Brasil bootcamp (2022).**
> Built while learning React and TypeScript. It is kept here as a record of that work, not as a maintained product.

Single-page front end for the [Blog Pessoal API](https://github.com/AlmeidaaPauloo/BlogPessoal): sign up, log in, and create, edit and delete posts and themes.

## Stack

- React 17 + TypeScript (Create React App)
- React Router 6
- Redux (react-redux) for the auth token
- Axios for API calls
- Material UI

## Structure

```
src/
  components/   navbar, footer, post and theme forms/lists/modals
  paginas/      home, login, sign-up
  models/       TypeScript types (User, Postagem, Tema)
  services/     Axios instance and API helpers
  store/        Redux store and token reducer
```

## Running locally

Requirements: Node.js and Yarn (or npm).

```bash
yarn install
yarn start
```

The app expects the Blog Pessoal API. The original API deploy (Heroku) is no longer online, so to use the app today run the API locally and point `baseURL` in `src/services/Services.ts` to it.

## Status

Create React App is no longer maintained; migrating to Vite would be the first step if this project is revisited.
