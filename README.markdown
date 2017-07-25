# Concourse in Docker

This is more or less a manifestation of the [instructions at concourse.ci](https://concourse.ci/docker-repository.html).

# Basic Auth

Instead of storing the basic auth password in this repository, create a new file `secrets.env` with the following content:

```bash
CONCOURSE_BASIC_AUTH_PASSWORD=changeme
```

and replace `changeme` with a real password. You'll need this for `fly` and the web frontend.

# `fly`

```bash
fly -t lite login -c http://$(docker-machine ip):8080
```
