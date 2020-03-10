# nnn (File Manager)
Lightweight TUI based file manager for the console ('nnn' Command)

## nnn (Project Info)
[Website](https://github.com/jarun/nnn)

## Docker Hub
[Website](https://hub.docker.com/r/macabees/nnn/)

## Build image
`$ docker build -t macabees/nnn:latest .`

## Docker Push
`$ docker push -t macabees/nnn:latest`

Note: requires `docker login`

## Run image
`$ docker run -it --rm --name nnn macabees/nnn`
(Runs the application in the isolation of the container [no external access to the local filesystem])

`$ docker run -it --rm -v $(pwd):/home/root --name nnn macabees/nnn`
(Note: this command grants access to the current directory on your local filesystem to the 'nnn' application running in the container)

## Help
`$ docker run -it --rm macabees/nnn --help`
