# 本库基于Docker部署XrayR作者原版的一键脚本

# 一键脚本
```bash
bash <(curl -sL https://raw.githubusercontent.com/KKX666/Docker-script/main/xrayr.sh)
```

# 支持

- [x] 仅支持v2board
- [x] 支持V2ray ShadowSocks Trojan
- [x] 支持设置有无证书三种证书申请方式：`dns file http`，其中 `dns` 证书申请仅支持Cloudflare dns
- [x] 支持查看xrayr配置

# Docker-compose 安装XrayR (推荐)
依次执行
```
curl -fsSL https://get.docker.com | bash -s docker
curl -L "https://github.com/docker/compose/releases/download/1.26.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```
