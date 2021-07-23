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

# Example

## Start an http proxy without ssl
```
$ http-proxy -listen ":8888" -proto http
```

## Start an http proxy with ssl
```
$ http-proxy -key server.key -pem server.pem
```

