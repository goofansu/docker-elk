docker-elk
===

Simple dev environment for ELK stack.

Saving test.log into elasticsearch via filebeat and logstash.

# Requirement (macOS)

Use filebeat the same as the ELK version.

# Run

1. `docker-compose -f docker-compose-latest.yml up`
2. `filebeat -c filebeat.yml`

# Test

* `touch test.log && echo '{"nickname": "test"}' >> test.log`
* In filebeat stdin, input `{"nickname": "test"}` and return
