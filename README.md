# Zoomies POC

Tests a zoomies image idea.

## Setup

Have Node installed. `v18` or higher preferred. `v16` will grouse a bit but appears to work.

To install the dependencies at the versions they last knowingly worked at:

```
$ npm ci
```

To install / update the dependencies with latest minor or patch updates:

```
$ npm install
```

## Coding

`index.html` is the startup page. `src/index.ts` is the startup module. Anything in `public/` will be included in the build output root.

To run the source via local webserver:

```
$ npm run dev
```

The site will be accessible at `localhost:5173`. Code changes should trigger a hot reload.

## Build

```
$ npm run build
```

Output will appear in the `build` folder with the following structure

```
index.html
assets/
  package-name.js
  package-name.css
  package-name.js.map
  possibly bundled chunks from any imported package.json items
anything from public/
```