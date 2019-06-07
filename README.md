# elk


## Send log do Logstash by Command Line

On Logstash

```
input {
  tcp {
    port => 9000
  }
}
```

On client side

```
echo -n '{"teste":"ok"}' | nc LOGSTASH_IP LOGSTASH_PORT
```
