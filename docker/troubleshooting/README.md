# Troubleshooting

## Start docker container to verify image state

Override the entrypoint and define an empty one so an interactive session can be started through the terminal using a shell as command.

```sh
docker run --rm --entrypoint "" -it <IMAGE_NAME> <SHELL>
```

For example, assuming *bash* is available:

```sh
docker run --rm --entrypoint "" -it my-image:1.0.0 bash
```
