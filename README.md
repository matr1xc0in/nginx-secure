# nginx-secure

`Directory` and `branch` structure alignment and info:
- master - a place hodlers for other directories and implementations

Define a file called `common.sh` and define the values at your convinience.
```
#!/bin/bash

set -a
export NGINX_USER=${NGINX_USER:-"nginx"}
export NGINX_UID=${NGINX_UID:-4999}
export NGINX_GID=${NGINX_GID:-5999}
set +a
```

This kicks off the container and you can run command `nginx` to start the web server.
```
./run.sh
```
