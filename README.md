# Usage Instructions

## Prerequisites

In order to run this project you'll need to have Docker installed.

## Instructions

### Clone the repo

```bash
git clone https://github.com/jasonswett/my_factory_bot.git
cd my_factory_bot
```

### Start the web service

```bash
docker compose run web
```

### Shell into the container

Run the following command, where `abc123` is the ID of the `web` container.
Instructions for getting the ID are below.

```bash
docker exec -it abc123 /bin/bash
```

If you run `docker container ls`, you should see output similar to the following.

```bash
$ docker container ls
CONTAINER ID   IMAGE            COMMAND                  CREATED             STATUS                    PORTS                      NAMES
bf92c5a5435c   my_factory_bot   "bash -c 'rm -rf /us…"   51 minutes ago      Up 51 minutes                                        my_factory_bot_web_run_b0a93042943b
```

The `bf92c5a5435c` is the part you want to copy.
