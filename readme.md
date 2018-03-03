# templates
This repository holds a collection of opinionated templates for use with [`scaffy`][semibran/scaffy]. The following directories are included:

```
app
├── src
│   ├── index.html
│   ├── script.js
│   └── style.scss
├── .gitignore
├── license
├── Makefile
├── package.json
├── readme.md
└── rollup.config.js
```

```
module
├── lib
│   └── {{name}}.js
├── license
├── package.json
└── readme.md
```

```
tool
├── bin
│   ├── help.txt
│   └── {{name}}.js
├── .gitignore
├── license
├── package.json
└── readme.md
```

## usage
To use these templates locally, clone this repository and invoke `scaffy` with the data variables `name` and `description`.

```sh
$ git clone git@github.com:semibran/templates
$ scaffy templates/app -o app \
> --name=app \
> --description="an example app"
$ cd app
$ git init
```

[semibran/scaffy]: https://github.com/semibran/scaffy
