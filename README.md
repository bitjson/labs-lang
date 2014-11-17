### discourse-locale-override

Add to `discourse/containers/` app YAML file:

```ruby
hooks:
  after_code:
    - exec:
        cd: $home/plugins
        cmd:
          - mkdir -p plugins
          - git clone https://github.com/bitjson/discourse-locale-override.git
```

### License

Copyright 2014 BitPay, Inc.
