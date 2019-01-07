### Demo of Nginx Reverse Proxy Caching

We can run one instance of Nginx in front of another to provide a layer of caching. This requires:
  - create a directory for cached files
  - apply the cache configuration for the server block

It is not necessary to pass the cache status in the response header, but it's helpful in building.

Also, note the pass_through name is special `http://demo_nginx` as this is a Docker project. In a normal server setting, that is an IP address.