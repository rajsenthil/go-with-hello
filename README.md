# GO microservice example with simple hello world

## Docker build
On project folder
`sudo docker build -t go-hello:v1 . -f kubernetes/docker/Dockerfile`

## Docker run
To run interactively at the port 3000
`sudo docker run -it -p 3000:3000 go-hello:v1`
