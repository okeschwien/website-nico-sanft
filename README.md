# README sanft & steil

## SASS/SCSS + PurgeCSS

### Install SASS

```
brew install sass/sass/sass
```

### Install PurgeCSS

```
npm i -g purgecss
```

### Usage

Watch and compile all SASS/SCSS styles into a minified CSS file:

```
sass --watch scss/index.scss:css/index.min.css --style compressed
```

Compile all SASS/SCSS styles into a minified CSS file, then purge and replace the minified CSS file:

```
sass scss/index.scss:css/index.min.css --style compressed && purgecss --css ./css/index.min.css --content ./index.html --output ./css/
```
