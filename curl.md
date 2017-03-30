


Flags
=====

* `-d`: send the specified data
* `-I`: print the response headers
* `-L`: If  the  server  reports  that  the requested page has moved to a different location (indicated with a Location: header and a 3XX response code), this option will make curl redo the request on the new place.
* `-O`: Write output to a local file named like the remote file we get.
* `-r` / `--range`: Retrieve a byte range (i.e a partial document) from a HTTP/1.1
* `-v`: verbose



HTTP GET
========

```
curl -v http://localhost:21318/NTJsonRequestHandler
```

HTTP POST
=========

```
curl -v -X POST  -d "{\"a\":1}" http://localhost:21318/NTJsonRequestHandler
```


