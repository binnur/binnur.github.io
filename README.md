# Notes on Binnur's github.io structure

## About the site
Site uses [Writer Jekyll] (https://themeforest.net/item/writer-a-minimal-blog-for-jekyll/10562560) theme
by adventurethemes.com

## Local development
Local setup uses the latest Jekyll docker image for development and updates.
```sh
$ docker-compose up -d
$ docker-compose down
# restart required when _config.yml updated
$ docker-compose restart
# log dump when running in -d mode
$ docker-compose logs -f
```

Note, docker setup requires `host: 0.0.0.0` in _config.yml
Access: [localhost:4000](http://localhost:4000)

## Basic Workflow
- Start docker for local development
- Update and preview locally
- Push the changes to remote git repo master branch, which is configured for GitHub Pages


