# Educasuisse.ch

This repository contain the website for [Educasuisse](https://educasuisse.ch/).

It is based on [Hugo](http://gohugo.io/).

## Development

First of all, you can clone the repository:

```sh
git clone git@github.com:educasuisse/educasuisse.ch.git
cd educasuisse.ch
```

### Content and layouts

Make sure to install [Hugo](http://gohugo.io/) first on your computer.

Then you can clone the directory and run the dev server:

```sh
hugo server
open http://localhost:1313/
```

### CSS/SCSS

For convenience, we use the [node-sass](https://github.com/sass/node-sass) binding lib to compile the SCSS into the final CSS (who is also added to git).

To compile your CSS before submitting:

```sh
node-sass --output-style compressed src/scss/main.scss -o static/css/
```

To compile your CSS while developing:

```sh
node-sass -w src/scss/main.scss -o static/css/
```
