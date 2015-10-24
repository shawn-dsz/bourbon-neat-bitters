# Sass with plugin - bourbon, neat, bitters

This repo shows how you can structure your sass file to having to be over specfic later down the track.

We include our sass in the following order

- plugins
- base
- modules
- layouts

The later the sass include the more specfic it needs to be in order to overside the base styles.
## Dependencies

Before you can start using sass you need to the following installed

###### [ruby](rubyinstaller.org/)
```sh
> gem install bundler
```
After you've installed **ruby** you can install [**bundler**](bundler.io)

```sh
> gem install sass
```
After you've install bundler you can install [**sass**](sass-lang.com)

## Install sass plugins

Change directory into  ```01-plugins```

```sh
..\css\plugins> bourbon install
..\css\plugins> neat install
..\css\plugins> bitters install 
```

## Install

```
> npm i
```

## Development workflow


- You can host the directory using, this will by default setup a web server on ```localhost:3000/```

```sh
> serve
```

- Now setup watch task for sass to convert your sass to css files

```sh
..\css> sass --watch app.sass:app.css
```

- Lastly you can setup [livereload](https://github.com/livereload/livereload-js) to immdiate view changes made styles without refreshing the browser; this is done by

```sh
> livereload .
```

Also livereload.js needs to added into the html page the needs to reload automatically


That's it you should have a workflow, that allows you write beautify css and view the changes as you dev.
