# elk


## Send log do Logstash

On Logstash

```
 {
    tcp {
      port => 9000
    }
 }
```

On client side

```
echo -n '{"teste":"ok"}' | nc LOGSTASH_IP LOGSTASH_PORT
```
