# DevmentorLive NextJS Starter Template

## Getting Started

To create an app using this starter

```bash
npx create-next-app your-app-name -e https://github.com/devmentorlive-youtube/next-tailwind-starter
```

## This template uses [TailwindCSS](https://tailwindcss.com/)!

## To run your server (development)

```
cd your-app-name
npm run dev
```

## Folder structure

```bash
src
├── features
├── pages
│   └── index.jsx
├── ui
└── index.jsx
```

This app uses a modified/simplified version of [Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/), better suited for modern web development.


### /ui

This folder is for your "lego blocks", single purpose React components that can be combined together to make more complicated components, known as Features


### /features

This folder is for more complex components, or features. Features are created by composing many UI components and usually, state


### /pages

This folder is for navigable components. A router automagically creates urls for anything in this folder. To create a page, combine features and ui components and put them in a component in this page. Typically state is managed in the feature, and any props that come from the server are passed through pages via the return object from getServerSideProps. Those props are then passed down into features as props, or put into a context.
