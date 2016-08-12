docker-elk
===

Simple dev environment for ELK stack.

Saving test.log into elasticsearch via filebeat and logstash.

# Requirement (macOS)

`brew install filebeat`

# Run

Terminal 1: `docker-compose up`
Terminal 2: `filebeat -c filebeat.yml`

# Test

``` bash
echo '{"nickname": "goofansu"}' > test.log
```
