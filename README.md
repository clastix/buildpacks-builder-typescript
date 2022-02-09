# [Buildpacks](https://buildpacks.io) Typescript builder

## Quickstart

### Create the bulder

```
pack builder create my-builder:heroku-20 --config ./builder.toml
```

### Use the builder

```
pack build hello-world --builder my-builder:heroku-20 --path ./hello-world
```

### Run the app from the built artifact

```
docker run --rm -p 8080:8080 hello-world
```


## Customize

You can edit the stack, and change the **build image** and **run image**.
The configured stack is based on the base image `heroku:20`.
