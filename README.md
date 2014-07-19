## Description

Dockerizing (MediaGoblin)[http://mediagoblin.org/] for easy use and deployment.

## Usage

    sudo ./build.sh
    sudo ./run.sh

`build.sh` will build the Docker image, and `run.sh` will run the image. The resulting container is run interactively; I couldn't seem to get the email verification link in the docker logs when running with `-d`.

**NOTE**: If the running container is stopped, there will be no continuation of the previous sessioni when starting a new container. It will be a completely fresh slate, including having to create a user again.

## TODO

* Setup Postgres as a separate linked container.
* Volume mount configuration file?
* Use (Fig)[https://github.com/orchardup/fig/] make start up easier.
