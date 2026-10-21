# HAProxy Config Templates (Lite)

## English

Two filled HAProxy configs and the YAML that describes them: an HTTP load balancer and a TCP proxy. You can read or copy the `.cfg` files directly.

Not in this subset: the renderer, TLS termination, the health-check template, and the notes on version-sensitive `http-check send`.

The HTTP file balances `www.example.com` and `api.example.com` to RFC 5737 servers and uses `option httpchk GET /health`. The TCP file is `mode tcp` with a connect check. Bind addresses are `127.0.0.1`. Keyword behavior can change between HAProxy versions. Check upstream docs.

### Deliverables

- `deliverables/templates/http-lb.cfg` — HTTP load balancer
- `deliverables/templates/tcp.cfg` — TCP proxy
- `examples/http-lb.yml` — filled HTTP spec
- `examples/tcp.yml` — filled TCP spec

## 中文

两份已经填好的 HAProxy 配置，以及描述它们的 YAML：一份 HTTP 负载均衡，一份 TCP 代理。`.cfg` 可以直接阅读或拷走。

精简版不含：渲染器、TLS 终结、健康检查模板，以及关于 `http-check send` 跟版本有关的说明。

HTTP 文件把 `www.example.com` 和 `api.example.com` 分到 RFC 5737 服务器，并使用 `option httpchk GET /health`。TCP 文件是 `mode tcp`，带连接检查。监听地址是 `127.0.0.1`。关键字会随 HAProxy 版本变化。以官方文档为准（Check upstream docs）。

### 交付文件

- `deliverables/templates/http-lb.cfg`
- `deliverables/templates/tcp.cfg`
- `examples/http-lb.yml`
- `examples/tcp.yml`

Full version: GUMROAD_URL
