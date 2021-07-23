# http-proxy
A simple HTTP Proxy in Go. Useful for networking enhancement, when you need to proxy your requests.

# Installing
```shell
$ go get github.com/wushilin/http-proxy
```
The installed binary will be at $GOPATH/bin/http-proxy

# Executing
```
Usage of $GOPATH/bin/http-proxy:
  -key string
    	path to key file (default "server.key")
  -listen string
    	Listen on this interface and port (default ":8888")
  -pem string
    	path to pem file (default "server.pem")
  -proto string
    	Proxy protocol (http or https) (default "https")
```
# Use cases
* Debug firewall requirement
* Gain access to internet
* Proxy request

# Example
## Start an http proxy on port 8888
```
$ http-proxy
```

## Start an http proxy without ssl
```
$ http-proxy -listen ":8888" -proto http
```

## Start an http proxy with ssl
```
$ http-proxy -key server.key -pem server.pem
```


# Credit
Original author at https://medium.com/@mlowicki/http-s-proxy-in-golang-in-less-than-100-lines-of-code-6a51c2f2c38c

By Michał Łowicki
