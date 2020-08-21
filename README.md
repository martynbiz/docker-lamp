# Moodle-docker

A docker container for Moodle LMS

## Getting started 

First clone this repository and copy/amend the docker-compose.yml file to your liking:

```
$ cp docker-compose.yml-example docker-compose.yml
```

Then from within the project directory:

```
$ docker-compose up
```

You should be able to access the install page at http://localhost:8080 (or whatever port is set to).

Note: set database host to 'mariadb', not 'localhost'