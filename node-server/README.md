# Simple node server

## Docker file

Files used: [
"Dockerfile",
"package.json",
"server.js"
]

To build the image execute:

`docker build -t node-server-image .`

> -t (tag/name your image)

To run the image (create a container) execute:

`docker run -d -p 3000:3000 --name node-server-container node-server-image`

> -d run the container in the background \
> -p 3000:3000 map your machine port to the container port

To clean up: \
To force stop and remove the container: `docker rm -f node-server-container` \
To remove image: `docker image rm node-server-image`

## docker-compose.yml file

Files used: [
"docker-compose.yml",
"package.json",
"server.js"
]

Run the next commands in the same folder as the YML file

To start the server service execute:

`docker-compose up -d`

To stop the service execute:

`docker-compose down`
