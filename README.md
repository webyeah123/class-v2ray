## v2ray-heroku
[![](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/webyeah123/class-v2ray.git)

### heroku上部署v2ray
- [x] 支持VMess和VLESS两种协议
- [x] 支持自定义websocket路径
- [x] 伪装首页（3D元素周期表）
- [x] HTML5测速
- [x] 使用v2ray最新版构建

请求`/`，返回3D元素周期表

![image](https://cdn.jsdelivr.net/gh/DaoChen6/Heroku-v2ray/doc/1.png)

请求`/speedtest/`，html5-speedtest测速页面

![image](https://cdn.jsdelivr.net/gh/DaoChen6/Heroku-v2ray/doc/2.png)

请求`/test/`，文件下载速度测试

![image](https://cdn.jsdelivr.net/gh/DaoChen6/Heroku-v2ray/doc/3.png)

请求`/ray`（可配置）v2ray websocket路径


```
</details>

### 客户端配置

```
  - name: "yourName"
    type: vmess
    server: yourName.workers.dev
    port: 443
    uuid: yourUuid
    alterId: 0
    cipher: auto
    udp: true
    tls: true
    #skip-cert-verify: true
    servername: yourName.workers.dev
    network: ws
    ws-path: /ray
```
