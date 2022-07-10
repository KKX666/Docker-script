# 本库基于Docker部署XrayR作者原版的一键脚本
A Xray backend framework that can easily support many panels.

一个基于Xray的后端框架，支持V2ay,Trojan,Shadowsocks协议，极易扩展，支持多面板对接。

如对脚本不放心，可使用此沙箱先测一遍再使用：https://killercoda.com/playgrounds/scenario/ubuntu

# 官方文档
**[XrayR-project](https://crackair.gitbook.io/xrayr-project)**

# 特点
- 永久开源且免费。
- 支持V2ray，Trojan， Shadowsocks多种协议。
- 支持Vless和XTLS等新特性。
- 支持单实例对接多面板、多节点，无需重复启动。
- 支持限制在线IP
- 支持节点端口级别、用户级别限速。
- 配置简单明了。
- 修改配置自动重启实例。
- 方便编译和升级，可以快速更新核心版本， 支持Xray-core新特性。

# 支持

- [x] 仅支持v2boarb
- [x] 支持V2ray ShadowSocks Trojan
- [x] 支持设置有无证书三种证书申请方式：`dns file http`，其中 `dns` 证书申请仅支持Cloudflare dns
- [x] 支持查看xrayr配置

# 一键脚本
```bash
bash <(curl -sL https://raw.githubusercontent.com/KKX666/Docker-script/main/xrayr.sh)
```

# 安装Docker-compose (推荐)
依次执行
```
curl -fsSL https://get.docker.com | bash -s docker
```
```
curl -L "https://github.com/docker/compose/releases/download/1.26.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
```
chmod +x /usr/local/bin/docker-compose
```

# Docker-compose 安装XrayR
```
git clone https://github.com/KKX666/Docker-script
```
```
cd Docker-script
```
**编辑配置文件：config.yml [配置文件说明](https://crackair.gitbook.io/xrayr-project/xrayr-pei-zhi-wen-jian-shuo-ming/config)**

**启动docker**
```
docker-compose up -d
```

**无法启动docker 请先执行此命令 再执行启动docker命令**
```
systemctl start docker
```
