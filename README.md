# echo-httpd
An echo HTTP server, to see what you send.

### Setup
```
# docker pull approach0/echo-httpd
# docker run -it -p 8921:8080 hello-httpd node hello.js hello world!
```

### Test
```
$ curl -X POST http://localhost:8921/foo/bar -d '{"key1":"value1", "key2":"value2"}' --header "Content-Type: application/json"
/usr/bin/node /code/hello.js hello world!
 POST /foo/bar
 ["Host","localhost:8921","User-Agent","curl/7.73.0","Accept","*/*","Content-Type","application/json","Content-Length","34"]
 {"key1":"value1", "key2":"value2"}
```
