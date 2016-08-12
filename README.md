docker-elk
===

Simple dev environment for ELK stack.

Saving test.log into elasticsearch via filebeat and logstash.

# Requirement (macOS)

`brew install filebeat`

# Run

1. `docker-compose up`
2. `filebeat -c filebeat.yml`

# Test

`echo '{"nickname": "goofansu"}' > test.log`
