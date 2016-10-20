# ss
Docker image for [shadowsocks](https://github.com/shadowsocks/shadowsocks-go)
# How to use this image
`docker run -d -p 8989:8989 wowlusitong/ss -p 8989 -k 123456789`

You can also use config.json:

`docker run -d -p 8989:8989 -p 9001:9001 wowlusitong/ss -c /config.json`

default [config.json](https://github.com/wowlusitong/ss/blob/master/config.json)
```
 {
   "port_password":{
	    "193":"psnvg.com",
      "8989":"123456789",
    	"9001":"123456789",
	    "9002":"123456789"
    },
    "method":"aes-256-cfb",
    "timeout":600
  }
```

