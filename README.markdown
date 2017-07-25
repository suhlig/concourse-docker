# Concourse in Docker

This is more or less a manifestation of the [instructions at concourse.ci](https://concourse.ci/docker-repository.html).

# `fly`

```bash
fly -t lite login -c http://$(docker-machine ip):8080
```
