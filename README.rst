
Required ::

    $ gem install gstore

_`Configuration file <https://gist.github.com/2045536>` ::

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

https://gist.github.com/2045536
