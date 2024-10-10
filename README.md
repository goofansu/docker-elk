docker-elk
===

Playground for [ELK](https://www.elastic.co/what-is/elk-stack) stack.

# Run

```bash
# start ELK stack
docker-compose up

# start filebeat
cd filebeat
./filebeat -c filebeat.yml
```

# Verify the stack is working 

* `touch test.log && echo '{"nickname": "test"}' >> test.log`

* In filebeat stdin, input `{"nickname": "test"}` and return
