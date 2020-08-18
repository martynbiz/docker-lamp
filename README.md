# Moodle-docker

A docker container for Moodle LMS

## Getting started 

First clone this repository and amend the docker-compose.yml file to your liking, then from within the project directory:

```
$ docker-compose up
```

You should be able to access the install page at http://localhost:8080 (or whatever port is set to)

Note: `service apache reload` is commented out and at this time of writing, needs to be run within the container.