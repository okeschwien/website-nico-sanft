# README sanft & steil

## Sass/SCSS + PurgeCSS

### Install Sass

```
brew install sass/sass/sass
```

### Install PurgeCSS

```
npm i -g purgecss
```

### Usage

Watch and compile all Sass/SCSS styles into a minified CSS file:

```
sass --no-source-map --watch scss/index.scss:css/index.min.css scss/about.scss:css/about.min.css scss/detail.scss:css/detail.min.css --style compressed
```

Compile all Sass/SCSS styles into a minified CSS file, then purge and replace the minified CSS file:

```
sass --no-source-map scss/index.scss:css/index.min.css scss/about.scss:css/about.min.css --style compressed && purgecss --css ./css/index.min.css --content ./index.html --output ./css/ && purgecss --css ./css/about.min.css --content ./about.html --output ./css/
```
