## ArbitraryLoads

### Key

- **NSAllowsArbitraryLoads iOS9+**
    - CFURL
    - NSURLConnection
    - NSURLSession
    - UIWebView
    - WKWebView
    - AVFoundation


- **NSAllowsArbitraryLoadsInWebContent iOS10+**
    - UIWebView
    - WKWebView


- **NSAllowsArbitraryLoadsForMediaContent iOS10+**
    - AVFoundation


- **NSAllowsLocalNetworking iOS10+**
    - Local resource
        - 127.0.0.1
        - .local top-level domain


```
    在iOS10+中，一旦设置了NSAllowsArbitraryLoadsInWebContent、NSAllowsArbitraryLoadsForMediaContent或NSAllowsLocalNetworking中的任意一项，都将忽略对NSAllowsArbitraryLoads的设置。这就表明，在iOS10+中，若通过CFURL、NSURLSession或NSURLConnection接口访问网络，则只能访问支持https的站点。
```

**检测服务器是否支持ATS**
```
    nscurl --verbose --ats-diagnostics https://<your_server_domain>
```
