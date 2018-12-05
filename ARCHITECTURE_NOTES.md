## General architecture

Logstash:

* Inputs
* Codecs
* Filters
* Ouputs


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

See [logstash event object][event]

## Messaging queue

* persistent queue?
* async / futures-based




[event]: https://www.elastic.co/guide/en/logstash/current/event-api.html
