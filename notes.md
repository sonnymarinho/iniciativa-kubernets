## Commands

- `docker container inspect`

  to verify the docker container properties

- `docker container logs -f <key>`

  verify continuously the log records (f = follow)

- `docker image history ubuntu-curl-image`

  Show the history of an image

- `docker image prune`

  Remove all unused images not just dangling ones

## Image naming

```
sonnymarinho/api-conversao:v1
	^             ^         ^
	|             |         |
namespace   repository   version
```

## Docker file

- Separates each process by container
  - ensures granularity
  - ensures scalability

_Obs: uses the `.dockerignore` to avoid unnecessary files and folders_

_Obs: If it will not unzip the files or get them from then internet, uses the `COPY` command instead of `ADD` command._

## Pushing An Image To Docker Hub

After create an image, you can upload them to the docker hub the push them when necessary.

To do this, just generate the desired image locally, and after this push then to the Docker Hub with the command `docker push <image_name:version>`
