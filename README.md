# Docker Compose for ELK - Elasticsearch, Logstash and Kibana

### Send log do Logstash by Command Line

On logstash configuration: ./config-dir:/config-dir
```
input {
  tcp {
    port => 9000
  }
}
```

On client side, send a teste to logstash on tcp port 
```
echo -n '{"teste":"ok"}' | nc [LOGSTASH_IP] [LOGSTASH_PORT]
```
