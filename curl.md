


Flags
=====

* `-d`: send the specified data
* `-d`: send the specified data as binary data ([java - Does curl remove new line characters? - Stack Overflow](http://stackoverflow.com/questions/17456584/does-curl-remove-new-line-characters))
* `-i`: Include the HTTP-header in the  output
* `-L`: If  the  server  reports  that  the requested page has moved to a different location (indicated with a Location: header and a 3XX response code), this option will make curl redo the request on the new place.
* `-O`: Write output to a local file named like the remote file we get.
* `-r` / `--range`: Retrieve a byte range (i.e a partial document) from a HTTP/1.1
* `-s`: Silent or quiet  mode. Don't show progress meter or error messages
* `-v`: verbose



HTTP POST
=========

```
curl -X POST  -d "{\"a\":1}" http://localhost:21318/NTJsonRequestHandler
curl -X POST --data-binary  @file.json http://localhost:21318/NTJsonRequestHandler
```

