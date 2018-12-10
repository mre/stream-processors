## General architecture

Logstash:

* Inputs
* Codecs
* Filters
* Ouputs
* Events + Metadata

## Plugin system

```
logstash-plugin install logstash-filter-forwarded;
logstash-plugin install logstash-filter-geoip;
logstash-plugin install logstash-output-jdbc;
logstash-plugin install logstash-output-influxdb;
```

## Hot config reload

No system really does that.

## Event object

See [logstash event object][event].
This also contains metadata, which is a hashmap of additional key-value pairs that don't get flushed to the output.
This is convenient for simple bookkeeping tasks. Since this is heap-allocated, it comes with an overhead cost.

## Messaging queue

* persistent queue?
* async / futures-based

## Monitoring

Logstash offers a built-in monitoring API.

## More info

https://www.elastic.co/guide/en/logstash/current/deploying-and-scaling.html


[event]: https://www.elastic.co/guide/en/logstash/current/event-api.html
