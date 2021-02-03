# heroku-buildpack-elasticdump

This buildpack enables you to use [elasticdump](https://github.com/elasticsearch-dump/elasticsearch-dump) on heroku.

## Prerequisite
This buildpack uses `npm` command internally. So you need to have [heroku-buildpack-nodejs](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-nodejs) first and it's index should be higher than `heroku-buildpack-elasticdump`.

## Installation
You can add this buildpack to your application with the following command:
```bash
heroku buildpacks:set https://github.com/eyupatis/heroku-buildpack-elasticdump -a my-app
```

## Confirmation
After adding buildpack and deploying your application to Heroku, you can confirm the installation of `elasticdump` by running:
```bash
heroku run which elasticdump
```
