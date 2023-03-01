Utility container are something which can help you create images and then execute operations on them at runtime

`docker run -it node-util npm init` is running `npm init` command on a node utility container

using bind mount
`docker run -it -v /Users/ashishyd/Desktop/Development/playground/docker-utility-container:/app node-util npm init`

ENTRYPOINT is basically pre-append command

`docker build -t mynpm .`

`docker run -it -v /Users/ashishyd/Desktop/Development/playground/docker-utility-container:/app mynpm init`

Using docker compose 

`docker-compose run npm init` where npm is service name defined in yaml configuration