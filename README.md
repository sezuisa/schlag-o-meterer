# Schlag-o-meter

```bash
# running the application
nix run

# get the current counter value
ssh -p 23235 127.0.0.1 "get"

# set the new counter value
ssh -p 23235 127.0.0.1 "set 65"

# increment the counter value
ssh -p 23235 127.0.0.1 "incr 10"
```

## Building and running the container image

```bash
# build the container image
nix build .#containerimage

# load the container image into docker
docker load < result

# start the container
docker compose up -d
```
