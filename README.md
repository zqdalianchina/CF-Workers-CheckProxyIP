# CF-Workers-CheckProxyIP
验证CF ProxyIP可用性

## 项目介绍
该项目使用 Cloudflare Workers 来检查代理 IP 是否可用。

## 使用方法
1. 部署到 Cloudflare Workers 后，在浏览器或命令行访问：
   ```
   GET /check?proxyip=1.2.3.4:443
   ```
2. 若 IP 可用，则会返回成功的 JSON 响应，否则返回错误信息。

## 示例请求
```
curl "https://your-worker-url/check?proxyip=1.2.3.4"
```

## 注意事项
- 不带端口时默认使用 443。
- 可在本地或其他环境使用 fetch、XHR 等方式调用接口。
