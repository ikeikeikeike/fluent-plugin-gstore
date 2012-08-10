

Google Cloud Storage output plugin for the Fluent.
====================================================

[Google Cloud Storage](http://cloud.google.com/products/cloud-storage.html) output plugin for the [Fluent](http://fluentd.org/).


Installation
==============

Configuration

```java
<match pattern>
  type gstore

  gstore_key_id API_ACCESS_KEY
  gstore_sec_key API_SECRET_KEY
  gstore_bucket BUCKET_NAME
  path logs/
  buffer_path /var/log/fluent/gstore

  time_slice_format %Y%m%d-%H
  time_slice_wait 10m
  utc
</match>
```


Setup
=====

```bash
$ gem install fluent-plugin-gstore
```


LICENSE
========

Apache License, Version 2.0
